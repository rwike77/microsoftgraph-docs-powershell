---
external help file: Microsoft.Graph.Mail-help.xml
Module Name: Microsoft.Graph.Mail
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.mail/update-mguserinferenceclassificationoverride
schema: 2.0.0
ms.prod: mail
---

# Update-MgUserInferenceClassificationOverride

## SYNOPSIS
Change the classifyAs field of an override as specified.
You cannot use PATCH to change any other fields in an inferenceClassificationOverride instance.
If an override exists for a sender and the sender changes his/her display name, you can use POST to force an update to the name field in the existing override.
If an override exists for a sender and the sender changes his/her SMTP address, deleting the existing override and creating a new one withthe new SMTP address is the only way to 'update' the override for this sender.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaUserInferenceClassificationOverride](/powershell/module/Microsoft.Graph.Beta.Mail/Update-MgBetaUserInferenceClassificationOverride?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgUserInferenceClassificationOverride -InferenceClassificationOverrideId <String> -UserId <String>
 [-AdditionalProperties <Hashtable>] [-ClassifyAs <String>] [-Id <String>]
 [-SenderEmailAddress <IMicrosoftGraphEmailAddress>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgUserInferenceClassificationOverride -InferenceClassificationOverrideId <String> -UserId <String>
 -BodyParameter <IMicrosoftGraphInferenceClassificationOverride> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgUserInferenceClassificationOverride -InputObject <IMailIdentity> [-AdditionalProperties <Hashtable>]
 [-ClassifyAs <String>] [-Id <String>] [-SenderEmailAddress <IMicrosoftGraphEmailAddress>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgUserInferenceClassificationOverride -InputObject <IMailIdentity>
 -BodyParameter <IMicrosoftGraphInferenceClassificationOverride> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Change the classifyAs field of an override as specified.
You cannot use PATCH to change any other fields in an inferenceClassificationOverride instance.
If an override exists for a sender and the sender changes his/her display name, you can use POST to force an update to the name field in the existing override.
If an override exists for a sender and the sender changes his/her SMTP address, deleting the existing override and creating a new one withthe new SMTP address is the only way to 'update' the override for this sender.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Code snippet

```powershell
Import-Module Microsoft.Graph.Mail

$params = @{
	classifyAs = "focused"
}

# A UPN can also be used as -UserId.
Update-MgUserInferenceClassificationOverride -UserId $userId -InferenceClassificationOverrideId $inferenceClassificationOverrideId -BodyParameter $params
```
This example shows how to use the Update-MgUserInferenceClassificationOverride Cmdlet.

To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
inferenceClassificationOverride
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphInferenceClassificationOverride
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ClassifyAs
inferenceClassificationType

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
The unique identifier for an entity.
Read-only.

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InferenceClassificationOverrideId
The unique identifier of inferenceClassificationOverride

```yaml
Type: String
Parameter Sets: UpdateExpanded, Update
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IMailIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -SenderEmailAddress
emailAddress
To construct, see NOTES section for SENDEREMAILADDRESS properties and create a hash table.

```yaml
Type: IMicrosoftGraphEmailAddress
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserId
The unique identifier of user

```yaml
Type: String
Parameter Sets: UpdateExpanded, Update
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IMailIdentity
### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphInferenceClassificationOverride
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphInferenceClassificationOverride
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphInferenceClassificationOverride\>: inferenceClassificationOverride
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[ClassifyAs \<String\>\]: inferenceClassificationType
  \[SenderEmailAddress \<IMicrosoftGraphEmailAddress\>\]: emailAddress
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Address \<String\>\]: The email address of the person or entity.
    \[Name \<String\>\]: The display name of the person or entity.

INPUTOBJECT \<IMailIdentity\>: Identity Parameter
  \[AttachmentId \<String\>\]: The unique identifier of attachment
  \[ExtensionId \<String\>\]: The unique identifier of extension
  \[InferenceClassificationOverrideId \<String\>\]: The unique identifier of inferenceClassificationOverride
  \[MailFolderId \<String\>\]: The unique identifier of mailFolder
  \[MailFolderId1 \<String\>\]: The unique identifier of mailFolder
  \[MessageId \<String\>\]: The unique identifier of message
  \[MessageRuleId \<String\>\]: The unique identifier of messageRule
  \[UserId \<String\>\]: The unique identifier of user

SENDEREMAILADDRESS \<IMicrosoftGraphEmailAddress\>: emailAddress
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Address \<String\>\]: The email address of the person or entity.
  \[Name \<String\>\]: The display name of the person or entity.

## RELATED LINKS
[Update-MgBetaUserInferenceClassificationOverride](/powershell/module/Microsoft.Graph.Beta.Mail/Update-MgBetaUserInferenceClassificationOverride?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.mail/update-mguserinferenceclassificationoverride](https://learn.microsoft.com/powershell/module/microsoft.graph.mail/update-mguserinferenceclassificationoverride)


