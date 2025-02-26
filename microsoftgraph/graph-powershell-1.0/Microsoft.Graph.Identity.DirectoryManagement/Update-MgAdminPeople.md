---
external help file: Microsoft.Graph.Identity.DirectoryManagement-help.xml
Module Name: Microsoft.Graph.Identity.DirectoryManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.directorymanagement/update-mgadminpeople
schema: 2.0.0
---

# Update-MgAdminPeople

## SYNOPSIS
Update the navigation property people in admin

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaAdminPeople](/powershell/module/Microsoft.Graph.Beta.Identity.DirectoryManagement/Update-MgBetaAdminPeople?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgAdminPeople [-AdditionalProperties <Hashtable>] [-Id <String>]
 [-ProfileCardProperties <IMicrosoftGraphProfileCardProperty[]>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgAdminPeople -BodyParameter <IMicrosoftGraphPeopleAdminSettings> [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property people in admin

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
peopleAdminSettings
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphPeopleAdminSettings
Parameter Sets: Update
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Id
The unique identifier for an entity.
Read-only.

```yaml
Type: String
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProfileCardProperties
.
To construct, see NOTES section for PROFILECARDPROPERTIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphProfileCardProperty[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphPeopleAdminSettings
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphPeopleAdminSettings
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphPeopleAdminSettings\>: peopleAdminSettings
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[ProfileCardProperties \<IMicrosoftGraphProfileCardProperty\[\]\>\]: 
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[Annotations \<IMicrosoftGraphProfileCardAnnotation\[\]\>\]: 
      \[DisplayName \<String\>\]: 
      \[Localizations \<IMicrosoftGraphDisplayNameLocalization\[\]\>\]: 
        \[DisplayName \<String\>\]: If present, the value of this field contains the displayName string that has been set for the language present in the languageTag field.
        \[LanguageTag \<String\>\]: Provides the language culture-code and friendly name of the language that the displayName field has been provided in.
    \[DirectoryPropertyName \<String\>\]: 

PROFILECARDPROPERTIES \<IMicrosoftGraphProfileCardProperty\[\]\>: .
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[Annotations \<IMicrosoftGraphProfileCardAnnotation\[\]\>\]: 
    \[DisplayName \<String\>\]: 
    \[Localizations \<IMicrosoftGraphDisplayNameLocalization\[\]\>\]: 
      \[DisplayName \<String\>\]: If present, the value of this field contains the displayName string that has been set for the language present in the languageTag field.
      \[LanguageTag \<String\>\]: Provides the language culture-code and friendly name of the language that the displayName field has been provided in.
  \[DirectoryPropertyName \<String\>\]:

## RELATED LINKS
[Update-MgBetaAdminPeople](/powershell/module/Microsoft.Graph.Beta.Identity.DirectoryManagement/Update-MgBetaAdminPeople?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.directorymanagement/update-mgadminpeople](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.directorymanagement/update-mgadminpeople)


