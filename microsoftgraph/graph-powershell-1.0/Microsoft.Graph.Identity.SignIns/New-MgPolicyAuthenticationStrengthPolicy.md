---
external help file: Microsoft.Graph.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgpolicyauthenticationstrengthpolicy
schema: 2.0.0
ms.prod: identity-and-sign-in
---

# New-MgPolicyAuthenticationStrengthPolicy

## SYNOPSIS
Create a new custom authenticationStrengthPolicy object.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaPolicyAuthenticationStrengthPolicy](/powershell/module/Microsoft.Graph.Beta.Identity.SignIns/New-MgBetaPolicyAuthenticationStrengthPolicy?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgPolicyAuthenticationStrengthPolicy [-AdditionalProperties <Hashtable>] [-AllowedCombinations <String[]>]
 [-CombinationConfigurations <IMicrosoftGraphAuthenticationCombinationConfiguration[]>]
 [-CreatedDateTime <DateTime>] [-Description <String>] [-DisplayName <String>] [-Id <String>]
 [-ModifiedDateTime <DateTime>] [-PolicyType <String>] [-RequirementsSatisfied <String>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Create
```
New-MgPolicyAuthenticationStrengthPolicy -BodyParameter <IMicrosoftGraphAuthenticationStrengthPolicy> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new custom authenticationStrengthPolicy object.
This API is available in the following national cloud deployments.

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowedCombinations
A collection of authentication method modes that are required be used to satify this authentication strength.

```yaml
Type: String[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
authenticationStrengthPolicy
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuthenticationStrengthPolicy
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CombinationConfigurations
Settings that may be used to require specific types or instances of an authentication method to be used when authenticating with a specified combination of authentication methods.
To construct, see NOTES section for COMBINATIONCONFIGURATIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuthenticationCombinationConfiguration[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CreatedDateTime
The datetime when this policy was created.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
The human-readable description of this policy.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
The human-readable display name of this policy.
Supports $filter (eq, ne, not , and in).

```yaml
Type: String
Parameter Sets: CreateExpanded
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
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ModifiedDateTime
The datetime when this policy was last modified.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PolicyType
authenticationStrengthPolicyType

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RequirementsSatisfied
authenticationStrengthRequirements

```yaml
Type: String
Parameter Sets: CreateExpanded
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAuthenticationStrengthPolicy
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAuthenticationStrengthPolicy
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphAuthenticationStrengthPolicy\>: authenticationStrengthPolicy
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[AllowedCombinations \<String\[\]\>\]: A collection of authentication method modes that are required be used to satify this authentication strength.
  \[CombinationConfigurations \<IMicrosoftGraphAuthenticationCombinationConfiguration\[\]\>\]: Settings that may be used to require specific types or instances of an authentication method to be used when authenticating with a specified combination of authentication methods.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[AppliesToCombinations \<String\[\]\>\]: Which authentication method combinations this configuration applies to.
Must be an allowedCombinations object that's defined for the authenticationStrengthPolicy.
The only possible value for fido2combinationConfigurations is 'fido2'.
  \[CreatedDateTime \<DateTime?\>\]: The datetime when this policy was created.
  \[Description \<String\>\]: The human-readable description of this policy.
  \[DisplayName \<String\>\]: The human-readable display name of this policy.
Supports $filter (eq, ne, not , and in).
  \[ModifiedDateTime \<DateTime?\>\]: The datetime when this policy was last modified.
  \[PolicyType \<String\>\]: authenticationStrengthPolicyType
  \[RequirementsSatisfied \<String\>\]: authenticationStrengthRequirements

COMBINATIONCONFIGURATIONS \<IMicrosoftGraphAuthenticationCombinationConfiguration\[\]\>: Settings that may be used to require specific types or instances of an authentication method to be used when authenticating with a specified combination of authentication methods.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[AppliesToCombinations \<String\[\]\>\]: Which authentication method combinations this configuration applies to.
Must be an allowedCombinations object that's defined for the authenticationStrengthPolicy.
The only possible value for fido2combinationConfigurations is 'fido2'.

## RELATED LINKS
[New-MgBetaPolicyAuthenticationStrengthPolicy](/powershell/module/Microsoft.Graph.Beta.Identity.SignIns/New-MgBetaPolicyAuthenticationStrengthPolicy?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgpolicyauthenticationstrengthpolicy](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgpolicyauthenticationstrengthpolicy)


