---
external help file: Microsoft.Graph.PersonalContacts-help.xml
Module Name: Microsoft.Graph.PersonalContacts
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.personalcontacts/get-mgusercontactcount
schema: 2.0.0
---

# Get-MgUserContactCount

## SYNOPSIS
Get the number of the resource

> [!NOTE]
> To view the beta release of this cmdlet, view [Get-MgBetaUserContactCount](/powershell/module/Microsoft.Graph.Beta.PersonalContacts/Get-MgBetaUserContactCount?view=graph-powershell-beta)

## SYNTAX

### Get (Default)
```
Get-MgUserContactCount -UserId <String> [-Filter <String>] [-Search <String>] [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgUserContactCount -InputObject <IPersonalContactsIdentity> [-Filter <String>] [-Search <String>]
 [<CommonParameters>]
```

## DESCRIPTION
Get the number of the resource

## PARAMETERS

### -Filter
Filter items by property values

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IPersonalContactsIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Search
Search items by search phrases

```yaml
Type: String
Parameter Sets: (All)
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
Parameter Sets: Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IPersonalContactsIdentity
## OUTPUTS

### System.Int32
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT \<IPersonalContactsIdentity\>: Identity Parameter
  \[ContactFolderId \<String\>\]: The unique identifier of contactFolder
  \[ContactFolderId1 \<String\>\]: The unique identifier of contactFolder
  \[ContactId \<String\>\]: The unique identifier of contact
  \[ExtensionId \<String\>\]: The unique identifier of extension
  \[UserId \<String\>\]: The unique identifier of user

## RELATED LINKS
[Get-MgBetaUserContactCount](/powershell/module/Microsoft.Graph.Beta.PersonalContacts/Get-MgBetaUserContactCount?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.personalcontacts/get-mgusercontactcount](https://learn.microsoft.com/powershell/module/microsoft.graph.personalcontacts/get-mgusercontactcount)



