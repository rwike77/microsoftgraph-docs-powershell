---
external help file: Microsoft.Graph.PersonalContacts-help.xml
Module Name: Microsoft.Graph.PersonalContacts
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.personalcontacts/get-mgusercontactfolderchildfoldercontactphotocontent
schema: 2.0.0
---

# Get-MgUserContactFolderChildFolderContactPhotoContent

## SYNOPSIS
Get media content for the navigation property photo from users

> [!NOTE]
> To view the beta release of this cmdlet, view [Get-MgBetaUserContactFolderChildFolderContactPhotoContent](/powershell/module/Microsoft.Graph.Beta.PersonalContacts/Get-MgBetaUserContactFolderChildFolderContactPhotoContent?view=graph-powershell-beta)

## SYNTAX

### Get (Default)
```
Get-MgUserContactFolderChildFolderContactPhotoContent -ContactFolderId <String> -ContactFolderId1 <String>
 -ContactId <String> -UserId <String> -OutFile <String> [-PassThru] [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgUserContactFolderChildFolderContactPhotoContent -InputObject <IPersonalContactsIdentity>
 -OutFile <String> [-PassThru] [<CommonParameters>]
```

## DESCRIPTION
Get media content for the navigation property photo from users

## PARAMETERS

### -ContactFolderId
The unique identifier of contactFolder

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

### -ContactFolderId1
The unique identifier of contactFolder

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

### -ContactId
The unique identifier of contact

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

### -OutFile
Path to write output file to

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
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

### System.Boolean
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
[Get-MgBetaUserContactFolderChildFolderContactPhotoContent](/powershell/module/Microsoft.Graph.Beta.PersonalContacts/Get-MgBetaUserContactFolderChildFolderContactPhotoContent?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.personalcontacts/get-mgusercontactfolderchildfoldercontactphotocontent](https://learn.microsoft.com/powershell/module/microsoft.graph.personalcontacts/get-mgusercontactfolderchildfoldercontactphotocontent)



