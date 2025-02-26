---
external help file: Microsoft.Graph.Beta.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Beta.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetapolicydefaultappmanagementpolicy
schema: 2.0.0
ms.prod: identity-and-sign-in
---

# Update-MgBetaPolicyDefaultAppManagementPolicy

## SYNOPSIS
Update the properties of a tenantAppManagementPolicy object.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgPolicyDefaultAppManagementPolicy](/powershell/module/Microsoft.Graph.Identity.SignIns/Update-MgPolicyDefaultAppManagementPolicy?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaPolicyDefaultAppManagementPolicy [-AdditionalProperties <Hashtable>]
 [-ApplicationRestrictions <IMicrosoftGraphAppManagementConfiguration>] [-DeletedDateTime <DateTime>]
 [-Description <String>] [-DisplayName <String>] [-Id <String>] [-IsEnabled]
 [-ServicePrincipalRestrictions <IMicrosoftGraphAppManagementConfiguration>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Update
```
Update-MgBetaPolicyDefaultAppManagementPolicy -BodyParameter <IMicrosoftGraphTenantAppManagementPolicy>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the properties of a tenantAppManagementPolicy object.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Code snippet

```powershell
Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	isEnabled = $true
	applicationRestrictions = @{
		passwordCredentials = @(
			@{
				restrictionType = "passwordAddition"
				maxLifetime = $null
				restrictForAppsCreatedAfterDateTime = [System.DateTime]::Parse("2021-01-01T10:37:00Z")
			}
			@{
				restrictionType = "passwordLifetime"
				maxLifetime = "P4DT12H30M5S"
				restrictForAppsCreatedAfterDateTime = [System.DateTime]::Parse("2017-01-01T10:37:00Z")
			}
			@{
				restrictionType = "symmetricKeyAddition"
				maxLifetime = $null
				restrictForAppsCreatedAfterDateTime = [System.DateTime]::Parse("2021-01-01T10:37:00Z")
			}
			@{
				restrictionType = "customPasswordAddition"
				maxLifetime = $null
				restrictForAppsCreatedAfterDateTime = [System.DateTime]::Parse("2015-01-01T10:37:00Z")
			}
			@{
				restrictionType = "symmetricKeyLifetime"
				maxLifetime = "P40D"
				restrictForAppsCreatedAfterDateTime = [System.DateTime]::Parse("2015-01-01T10:37:00Z")
			}
		)
		keyCredentials = @(
			@{
				restrictionType = "asymmetricKeyLifetime"
				maxLifetime = "P30D"
				restrictForAppsCreatedAfterDateTime = [System.DateTime]::Parse("2015-01-01T10:37:00Z")
			}
		)
	}
}

Update-MgBetaPolicyDefaultAppManagementPolicy -BodyParameter $params
```
This example shows how to use the Update-MgBetaPolicyDefaultAppManagementPolicy Cmdlet.

To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).


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

### -ApplicationRestrictions
appManagementConfiguration
To construct, see NOTES section for APPLICATIONRESTRICTIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAppManagementConfiguration
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
tenantAppManagementPolicy
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphTenantAppManagementPolicy
Parameter Sets: Update
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DeletedDateTime
Date and time when this object was deleted.
Always null when the object hasn't been deleted.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
Description for this policy.
Required.

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

### -DisplayName
Display name for this policy.
Required.

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

### -IsEnabled
Denotes whether the policy is enabled.
Default value is false.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServicePrincipalRestrictions
appManagementConfiguration
To construct, see NOTES section for SERVICEPRINCIPALRESTRICTIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAppManagementConfiguration
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphTenantAppManagementPolicy
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphTenantAppManagementPolicy
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

APPLICATIONRESTRICTIONS \<IMicrosoftGraphAppManagementConfiguration\>: appManagementConfiguration
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[KeyCredentials \<IMicrosoftGraphKeyCredentialConfiguration\[\]\>\]: Collection of keyCredential restrictions settings to be applied to an application or service principal.
    \[CertificateBasedApplicationConfigurationIds \<String\[\]\>\]: Collection of GUIDs that point to the certificateBasedApplicationConfiguration that contains the collection of allowed root and intermediate certificate authorities.
    \[MaxLifetime \<TimeSpan?\>\]: 
    \[RestrictForAppsCreatedAfterDateTime \<DateTime?\>\]: Timestamp when the policy is enforced for all apps created on or after the specified date.
For existing applications, the enforcement date would be back dated.
To apply to all applications regardless of their creation date, this property would be null.
Nullable.
    \[RestrictionType \<String\>\]: appKeyCredentialRestrictionType
  \[PasswordCredentials \<IMicrosoftGraphPasswordCredentialConfiguration\[\]\>\]: Collection of password restrictions settings to be applied to an application or service principal.
    \[MaxLifetime \<TimeSpan?\>\]: 
    \[RestrictForAppsCreatedAfterDateTime \<DateTime?\>\]: Enforces the policy for an app created on or after the enforcement date.
For existing applications, the enforcement date would be backdated.
To apply to all applications, this date would be null.
    \[RestrictionType \<String\>\]: appCredentialRestrictionType

BODYPARAMETER \<IMicrosoftGraphTenantAppManagementPolicy\>: tenantAppManagementPolicy
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Description \<String\>\]: Description for this policy.
Required.
  \[DisplayName \<String\>\]: Display name for this policy.
Required.
  \[DeletedDateTime \<DateTime?\>\]: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[ApplicationRestrictions \<IMicrosoftGraphAppManagementConfiguration\>\]: appManagementConfiguration
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[KeyCredentials \<IMicrosoftGraphKeyCredentialConfiguration\[\]\>\]: Collection of keyCredential restrictions settings to be applied to an application or service principal.
      \[CertificateBasedApplicationConfigurationIds \<String\[\]\>\]: Collection of GUIDs that point to the certificateBasedApplicationConfiguration that contains the collection of allowed root and intermediate certificate authorities.
      \[MaxLifetime \<TimeSpan?\>\]: 
      \[RestrictForAppsCreatedAfterDateTime \<DateTime?\>\]: Timestamp when the policy is enforced for all apps created on or after the specified date.
For existing applications, the enforcement date would be back dated.
To apply to all applications regardless of their creation date, this property would be null.
Nullable.
      \[RestrictionType \<String\>\]: appKeyCredentialRestrictionType
    \[PasswordCredentials \<IMicrosoftGraphPasswordCredentialConfiguration\[\]\>\]: Collection of password restrictions settings to be applied to an application or service principal.
      \[MaxLifetime \<TimeSpan?\>\]: 
      \[RestrictForAppsCreatedAfterDateTime \<DateTime?\>\]: Enforces the policy for an app created on or after the enforcement date.
For existing applications, the enforcement date would be backdated.
To apply to all applications, this date would be null.
      \[RestrictionType \<String\>\]: appCredentialRestrictionType
  \[IsEnabled \<Boolean?\>\]: Denotes whether the policy is enabled.
Default value is false.
  \[ServicePrincipalRestrictions \<IMicrosoftGraphAppManagementConfiguration\>\]: appManagementConfiguration

SERVICEPRINCIPALRESTRICTIONS \<IMicrosoftGraphAppManagementConfiguration\>: appManagementConfiguration
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[KeyCredentials \<IMicrosoftGraphKeyCredentialConfiguration\[\]\>\]: Collection of keyCredential restrictions settings to be applied to an application or service principal.
    \[CertificateBasedApplicationConfigurationIds \<String\[\]\>\]: Collection of GUIDs that point to the certificateBasedApplicationConfiguration that contains the collection of allowed root and intermediate certificate authorities.
    \[MaxLifetime \<TimeSpan?\>\]: 
    \[RestrictForAppsCreatedAfterDateTime \<DateTime?\>\]: Timestamp when the policy is enforced for all apps created on or after the specified date.
For existing applications, the enforcement date would be back dated.
To apply to all applications regardless of their creation date, this property would be null.
Nullable.
    \[RestrictionType \<String\>\]: appKeyCredentialRestrictionType
  \[PasswordCredentials \<IMicrosoftGraphPasswordCredentialConfiguration\[\]\>\]: Collection of password restrictions settings to be applied to an application or service principal.
    \[MaxLifetime \<TimeSpan?\>\]: 
    \[RestrictForAppsCreatedAfterDateTime \<DateTime?\>\]: Enforces the policy for an app created on or after the enforcement date.
For existing applications, the enforcement date would be backdated.
To apply to all applications, this date would be null.
    \[RestrictionType \<String\>\]: appCredentialRestrictionType

## RELATED LINKS
[Update-MgPolicyDefaultAppManagementPolicy](/powershell/module/Microsoft.Graph.Identity.SignIns/Update-MgPolicyDefaultAppManagementPolicy?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetapolicydefaultappmanagementpolicy](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetapolicydefaultappmanagementpolicy)


