---
external help file: Microsoft.Graph.Groups-help.xml
Module Name: Microsoft.Graph.Groups
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.groups/invoke-mgcheckingroupdriveroot
schema: 2.0.0
ms.prod: sharepoint
---

# Invoke-MgCheckinGroupDriveRoot

## SYNOPSIS
Check in a checked out driveItem resource, which makes the version of the document available to others.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the beta release of this cmdlet, view [Invoke-MgBetaCheckinGroupDriveRoot](/powershell/module/Microsoft.Graph.Beta.Groups/Invoke-MgBetaCheckinGroupDriveRoot?view=graph-powershell-beta)

## SYNTAX

### CheckinExpanded (Default)
```
Invoke-MgCheckinGroupDriveRoot -DriveId <String> -GroupId <String> [-AdditionalProperties <Hashtable>]
 [-CheckInAs <String>] [-Comment <String>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Checkin
```
Invoke-MgCheckinGroupDriveRoot -DriveId <String> -GroupId <String>
 -Body <IPathsD0Tb1DGroupsGroupIdDrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CheckinViaIdentityExpanded
```
Invoke-MgCheckinGroupDriveRoot -InputObject <IGroupsIdentity> [-AdditionalProperties <Hashtable>]
 [-CheckInAs <String>] [-Comment <String>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CheckinViaIdentity
```
Invoke-MgCheckinGroupDriveRoot -InputObject <IGroupsIdentity>
 -BodyParameter <IPathsD0Tb1DGroupsGroupIdDrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Check in a checked out driveItem resource, which makes the version of the document available to others.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Code snippet

```powershell
Import-Module Microsoft.Graph.Files

$params = @{
	Comment = "Updating the latest guidelines"
}

Invoke-MgCheckinDriveItem -DriveId $driveId -DriveItemId $driveItemId -BodyParameter $params
```
This example shows how to use the Invoke-MgCheckinGroupDriveRoot Cmdlet.

To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CheckinExpanded, CheckinViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Body
.
To construct, see NOTES section for BODY properties and create a hash table.

```yaml
Type: IPathsD0Tb1DGroupsGroupIdDrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Checkin
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -BodyParameter
.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPathsD0Tb1DGroupsGroupIdDrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema
Parameter Sets: CheckinViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CheckInAs
.

```yaml
Type: String
Parameter Sets: CheckinExpanded, CheckinViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Comment
.

```yaml
Type: String
Parameter Sets: CheckinExpanded, CheckinViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DriveId
The unique identifier of drive

```yaml
Type: String
Parameter Sets: CheckinExpanded, Checkin
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GroupId
The unique identifier of group

```yaml
Type: String
Parameter Sets: CheckinExpanded, Checkin
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
Type: IGroupsIdentity
Parameter Sets: CheckinViaIdentityExpanded, CheckinViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PassThru
Returns true when the command succeeds

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
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

### Microsoft.Graph.PowerShell.Models.IGroupsIdentity
### Microsoft.Graph.PowerShell.Models.IPathsD0Tb1DGroupsGroupIdDrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODY \<IPathsD0Tb1DGroupsGroupIdDrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema\>: .
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[CheckInAs \<String\>\]: 
  \[Comment \<String\>\]: 

BODYPARAMETER \<IPathsD0Tb1DGroupsGroupIdDrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema\>: .
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[CheckInAs \<String\>\]: 
  \[Comment \<String\>\]: 

INPUTOBJECT \<IGroupsIdentity\>: Identity Parameter
  \[AttachmentId \<String\>\]: The unique identifier of attachment
  \[ContentTypeId \<String\>\]: The unique identifier of contentType
  \[ConversationId \<String\>\]: The unique identifier of conversation
  \[ConversationThreadId \<String\>\]: The unique identifier of conversationThread
  \[DirectoryObjectId \<String\>\]: The unique identifier of directoryObject
  \[DocumentSetVersionId \<String\>\]: The unique identifier of documentSetVersion
  \[DriveId \<String\>\]: The unique identifier of drive
  \[DriveItemId \<String\>\]: The unique identifier of driveItem
  \[DriveItemVersionId \<String\>\]: The unique identifier of driveItemVersion
  \[EndDateTime \<String\>\]: Usage: endDateTime='{endDateTime}'
  \[EventId \<String\>\]: The unique identifier of event
  \[ExtensionId \<String\>\]: The unique identifier of extension
  \[GroupId \<String\>\]: The unique identifier of group
  \[GroupLifecyclePolicyId \<String\>\]: The unique identifier of groupLifecyclePolicy
  \[GroupSettingId \<String\>\]: The unique identifier of groupSetting
  \[GroupSettingTemplateId \<String\>\]: The unique identifier of groupSettingTemplate
  \[IncludePersonalNotebooks \<Boolean?\>\]: Usage: includePersonalNotebooks={includePersonalNotebooks}
  \[Interval \<String\>\]: Usage: interval='{interval}'
  \[ListId \<String\>\]: The unique identifier of list
  \[ListItemId \<String\>\]: The unique identifier of listItem
  \[ListItemVersionId \<String\>\]: The unique identifier of listItemVersion
  \[NotebookId \<String\>\]: The unique identifier of notebook
  \[OnenotePageId \<String\>\]: The unique identifier of onenotePage
  \[OnenoteSectionId \<String\>\]: The unique identifier of onenoteSection
  \[Path \<String\>\]: Usage: path='{path}'
  \[PermissionId \<String\>\]: The unique identifier of permission
  \[PostId \<String\>\]: The unique identifier of post
  \[ProfilePhotoId \<String\>\]: The unique identifier of profilePhoto
  \[Q \<String\>\]: Usage: q='{q}'
  \[ResourceSpecificPermissionGrantId \<String\>\]: The unique identifier of resourceSpecificPermissionGrant
  \[SiteId \<String\>\]: The unique identifier of site
  \[StartDateTime \<String\>\]: Usage: startDateTime='{startDateTime}'
  \[SubscriptionId \<String\>\]: The unique identifier of subscription
  \[Token \<String\>\]: Usage: token='{token}'
  \[User \<String\>\]: Usage: User='{User}'

## RELATED LINKS
[Invoke-MgBetaCheckinGroupDriveRoot](/powershell/module/Microsoft.Graph.Beta.Groups/Invoke-MgBetaCheckinGroupDriveRoot?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.groups/invoke-mgcheckingroupdriveroot](https://learn.microsoft.com/powershell/module/microsoft.graph.groups/invoke-mgcheckingroupdriveroot)


