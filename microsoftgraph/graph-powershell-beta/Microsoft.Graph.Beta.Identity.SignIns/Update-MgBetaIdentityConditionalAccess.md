---
external help file: Microsoft.Graph.Beta.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Beta.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetaidentityconditionalaccess
schema: 2.0.0
---

# Update-MgBetaIdentityConditionalAccess

## SYNOPSIS
Update the navigation property conditionalAccess in identity

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgIdentityConditionalAccess](/powershell/module/Microsoft.Graph.Identity.SignIns/Update-MgIdentityConditionalAccess?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaIdentityConditionalAccess [-AdditionalProperties <Hashtable>]
 [-AuthenticationContextClassReferences <IMicrosoftGraphAuthenticationContextClassReference[]>]
 [-AuthenticationStrength <IMicrosoftGraphAuthenticationStrengthRoot>]
 [-AuthenticationStrengths <IMicrosoftGraphAuthenticationStrengthRoot>] [-Id <String>]
 [-NamedLocations <IMicrosoftGraphNamedLocation[]>] [-Policies <IMicrosoftGraphConditionalAccessPolicy[]>]
 [-Templates <IMicrosoftGraphConditionalAccessTemplate[]>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaIdentityConditionalAccess -BodyParameter <IMicrosoftGraphConditionalAccessRoot> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property conditionalAccess in identity

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

### -AuthenticationContextClassReferences
Read-only.
Nullable.
Returns a collection of the specified authentication context class references.
To construct, see NOTES section for AUTHENTICATIONCONTEXTCLASSREFERENCES properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuthenticationContextClassReference[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AuthenticationStrength
authenticationStrengthRoot
To construct, see NOTES section for AUTHENTICATIONSTRENGTH properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuthenticationStrengthRoot
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AuthenticationStrengths
authenticationStrengthRoot
To construct, see NOTES section for AUTHENTICATIONSTRENGTHS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuthenticationStrengthRoot
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
conditionalAccessRoot
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphConditionalAccessRoot
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

### -NamedLocations
Read-only.
Nullable.
Returns a collection of the specified named locations.
To construct, see NOTES section for NAMEDLOCATIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphNamedLocation[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Policies
Read-only.
Nullable.
Returns a collection of the specified Conditional Access policies.
To construct, see NOTES section for POLICIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphConditionalAccessPolicy[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Templates
Read-only.
Nullable.
Returns a collection of the specified Conditional Access templates.
To construct, see NOTES section for TEMPLATES properties and create a hash table.

```yaml
Type: IMicrosoftGraphConditionalAccessTemplate[]
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphConditionalAccessRoot
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphConditionalAccessRoot
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

AUTHENTICATIONCONTEXTCLASSREFERENCES \<IMicrosoftGraphAuthenticationContextClassReference\[\]\>: Read-only.
Nullable.
Returns a collection of the specified authentication context class references.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[Description \<String\>\]: A short explanation of the policies that are enforced by authenticationContextClassReference.
This value should be used to provide secondary text to describe the authentication context class reference when building user facing admin experiences.
For example, selection UX.
  \[DisplayName \<String\>\]: A friendly name that identifies the authenticationContextClassReference object when building user-facing admin experiences.
For example, a selection UX.
  \[IsAvailable \<Boolean?\>\]: Indicates whether the authenticationContextClassReference has been published by the security admin and is ready for use by apps.
When it's set to false, it shouldn't be shown in selection UX used to tag resources with authentication context class values.
It will still be shown in the Conditional Access policy authoring experience. 
Supports $filter (eq).

AUTHENTICATIONSTRENGTH \<IMicrosoftGraphAuthenticationStrengthRoot\>: authenticationStrengthRoot
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[AuthenticationCombinations \<String\[\]\>\]: A collection of all valid authentication method combinations in the system.
  \[AuthenticationMethodModes \<IMicrosoftGraphAuthenticationMethodModeDetail\[\]\>\]: Names and descriptions of all valid authentication method modes in the system.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[AuthenticationMethod \<String\>\]: baseAuthenticationMethod
    \[DisplayName \<String\>\]: The display name of this mode
  \[Combinations \<String\[\]\>\]: 
  \[Policies \<IMicrosoftGraphAuthenticationStrengthPolicy\[\]\>\]: A collection of authentication strength policies that exist for this tenant, including both built-in and custom policies.
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

AUTHENTICATIONSTRENGTHS \<IMicrosoftGraphAuthenticationStrengthRoot\>: authenticationStrengthRoot
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[AuthenticationCombinations \<String\[\]\>\]: A collection of all valid authentication method combinations in the system.
  \[AuthenticationMethodModes \<IMicrosoftGraphAuthenticationMethodModeDetail\[\]\>\]: Names and descriptions of all valid authentication method modes in the system.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[AuthenticationMethod \<String\>\]: baseAuthenticationMethod
    \[DisplayName \<String\>\]: The display name of this mode
  \[Combinations \<String\[\]\>\]: 
  \[Policies \<IMicrosoftGraphAuthenticationStrengthPolicy\[\]\>\]: A collection of authentication strength policies that exist for this tenant, including both built-in and custom policies.
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

BODYPARAMETER \<IMicrosoftGraphConditionalAccessRoot\>: conditionalAccessRoot
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[AuthenticationContextClassReferences \<IMicrosoftGraphAuthenticationContextClassReference\[\]\>\]: Read-only.
Nullable.
Returns a collection of the specified authentication context class references.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[Description \<String\>\]: A short explanation of the policies that are enforced by authenticationContextClassReference.
This value should be used to provide secondary text to describe the authentication context class reference when building user facing admin experiences.
For example, selection UX.
    \[DisplayName \<String\>\]: A friendly name that identifies the authenticationContextClassReference object when building user-facing admin experiences.
For example, a selection UX.
    \[IsAvailable \<Boolean?\>\]: Indicates whether the authenticationContextClassReference has been published by the security admin and is ready for use by apps.
When it's set to false, it shouldn't be shown in selection UX used to tag resources with authentication context class values.
It will still be shown in the Conditional Access policy authoring experience. 
Supports $filter (eq).
  \[AuthenticationStrength \<IMicrosoftGraphAuthenticationStrengthRoot\>\]: authenticationStrengthRoot
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[AuthenticationCombinations \<String\[\]\>\]: A collection of all valid authentication method combinations in the system.
    \[AuthenticationMethodModes \<IMicrosoftGraphAuthenticationMethodModeDetail\[\]\>\]: Names and descriptions of all valid authentication method modes in the system.
      \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
      \[AuthenticationMethod \<String\>\]: baseAuthenticationMethod
      \[DisplayName \<String\>\]: The display name of this mode
    \[Combinations \<String\[\]\>\]: 
    \[Policies \<IMicrosoftGraphAuthenticationStrengthPolicy\[\]\>\]: A collection of authentication strength policies that exist for this tenant, including both built-in and custom policies.
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
  \[AuthenticationStrengths \<IMicrosoftGraphAuthenticationStrengthRoot\>\]: authenticationStrengthRoot
  \[NamedLocations \<IMicrosoftGraphNamedLocation\[\]\>\]: Read-only.
Nullable.
Returns a collection of the specified named locations.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[CreatedDateTime \<DateTime?\>\]: The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
    \[DisplayName \<String\>\]: Human-readable name of the location.
    \[ModifiedDateTime \<DateTime?\>\]: The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
  \[Policies \<IMicrosoftGraphConditionalAccessPolicy\[\]\>\]: Read-only.
Nullable.
Returns a collection of the specified Conditional Access policies.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[Conditions \<IMicrosoftGraphConditionalAccessConditionSet\>\]: conditionalAccessConditionSet
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Applications \<IMicrosoftGraphConditionalAccessApplications\>\]: conditionalAccessApplications
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[ApplicationFilter \<IMicrosoftGraphConditionalAccessFilter\>\]: conditionalAccessFilter
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[Mode \<String\>\]: filterMode
          \[Rule \<String\>\]: Rule syntax is similar to that used for membership rules for groups in Microsoft Entra ID.
For details, see rules with multiple expressions
        \[ExcludeApplications \<String\[\]\>\]: Can be one of the following:  The list of client IDs (appId) explicitly excluded from the policy.
Office365 - For the list of apps included in Office365, see Conditional Access target apps: Office 365
        \[IncludeApplications \<String\[\]\>\]: Can be one of the following:  The list of client IDs (appId) the policy applies to, unless explicitly excluded (in excludeApplications)  All  Office365 - For the list of apps included in Office365, see Conditional Access target apps: Office 365
        \[IncludeAuthenticationContextClassReferences \<String\[\]\>\]: Authentication context class references include.
Supported values are c1 through c25.
        \[IncludeUserActions \<String\[\]\>\]: User actions to include.
Supported values are urn:user:registersecurityinfo and urn:user:registerdevice
      \[ClientAppTypes \<String\[\]\>\]: Client application types included in the policy.
Possible values are: all, browser, mobileAppsAndDesktopClients, exchangeActiveSync, easSupported, other.
Required. 
The easUnsupported enumeration member will be deprecated in favor of exchangeActiveSync which includes EAS supported and unsupported platforms.
      \[ClientApplications \<IMicrosoftGraphConditionalAccessClientApplications\>\]: conditionalAccessClientApplications
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[ExcludeServicePrincipals \<String\[\]\>\]: Service principal IDs excluded from the policy scope.
        \[IncludeServicePrincipals \<String\[\]\>\]: Service principal IDs included in the policy scope, or ServicePrincipalsInMyTenant.
        \[ServicePrincipalFilter \<IMicrosoftGraphConditionalAccessFilter\>\]: conditionalAccessFilter
      \[DeviceStates \<IMicrosoftGraphConditionalAccessDeviceStates\>\]: conditionalAccessDeviceStates
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[ExcludeStates \<String\[\]\>\]: States excluded from the scope of the policy.
Possible values: Compliant, DomainJoined.
        \[IncludeStates \<String\[\]\>\]: States in the scope of the policy.
All is the only allowed value.
      \[Devices \<IMicrosoftGraphConditionalAccessDevices\>\]: conditionalAccessDevices
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[DeviceFilter \<IMicrosoftGraphConditionalAccessFilter\>\]: conditionalAccessFilter
        \[ExcludeDeviceStates \<String\[\]\>\]: 
        \[ExcludeDevices \<String\[\]\>\]: States excluded from the scope of the policy.
Possible values: Compliant, DomainJoined.
Cannot be set if deviceFIlter is set.
        \[IncludeDeviceStates \<String\[\]\>\]: 
        \[IncludeDevices \<String\[\]\>\]: States in the scope of the policy.
All is the only allowed value.
Cannot be set if deviceFilter is set.
      \[Locations \<IMicrosoftGraphConditionalAccessLocations\>\]: conditionalAccessLocations
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[ExcludeLocations \<String\[\]\>\]: Location IDs excluded from scope of policy.
        \[IncludeLocations \<String\[\]\>\]: Location IDs in scope of policy unless explicitly excluded, All, or AllTrusted.
      \[Platforms \<IMicrosoftGraphConditionalAccessPlatforms\>\]: conditionalAccessPlatforms
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[ExcludePlatforms \<String\[\]\>\]: Possible values are: android, iOS, windows, windowsPhone, macOS, all, unknownFutureValue, linux.
        \[IncludePlatforms \<String\[\]\>\]: Possible values are: android, iOS, windows, windowsPhone, macOS, all, unknownFutureValue,linux.
      \[ServicePrincipalRiskLevels \<String\[\]\>\]: Service principal risk levels included in the policy.
Possible values are: low, medium, high, none, unknownFutureValue.
      \[SignInRiskLevels \<String\[\]\>\]: Sign-in risk levels included in the policy.
Possible values are: low, medium, high, hidden, none, unknownFutureValue.
Required.
      \[UserRiskLevels \<String\[\]\>\]: User risk levels included in the policy.
Possible values are: low, medium, high, hidden, none, unknownFutureValue.
Required.
      \[Users \<IMicrosoftGraphConditionalAccessUsers\>\]: conditionalAccessUsers
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[ExcludeGroups \<String\[\]\>\]: Group IDs excluded from scope of policy.
        \[ExcludeGuestsOrExternalUsers \<IMicrosoftGraphConditionalAccessGuestsOrExternalUsers\>\]: conditionalAccessGuestsOrExternalUsers
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[ExternalTenants \<IMicrosoftGraphConditionalAccessExternalTenants\>\]: conditionalAccessExternalTenants
            \[(Any) \<Object\>\]: This indicates any property can be added to this object.
            \[MembershipKind \<String\>\]: conditionalAccessExternalTenantsMembershipKind
          \[GuestOrExternalUserTypes \<String\>\]: conditionalAccessGuestOrExternalUserTypes
        \[ExcludeRoles \<String\[\]\>\]: Role IDs excluded from scope of policy.
        \[ExcludeUsers \<String\[\]\>\]: User IDs excluded from scope of policy and/or GuestsOrExternalUsers.
        \[IncludeGroups \<String\[\]\>\]: Group IDs in scope of policy unless explicitly excluded.
        \[IncludeGuestsOrExternalUsers \<IMicrosoftGraphConditionalAccessGuestsOrExternalUsers\>\]: conditionalAccessGuestsOrExternalUsers
        \[IncludeRoles \<String\[\]\>\]: Role IDs in scope of policy unless explicitly excluded.
        \[IncludeUsers \<String\[\]\>\]: User IDs in scope of policy unless explicitly excluded, None, All, or GuestsOrExternalUsers.
    \[CreatedDateTime \<DateTime?\>\]: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Readonly.
    \[Description \<String\>\]: Not used.
    \[DisplayName \<String\>\]: Specifies a display name for the conditionalAccessPolicy object.
    \[GrantControls \<IMicrosoftGraphConditionalAccessGrantControls\>\]: conditionalAccessGrantControls
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[AuthenticationStrength \<IMicrosoftGraphAuthenticationStrengthPolicy\>\]: authenticationStrengthPolicy
      \[BuiltInControls \<String\[\]\>\]: List of values of built-in controls required by the policy.
Possible values: block, mfa, compliantDevice, domainJoinedDevice, approvedApplication, compliantApplication, passwordChange, unknownFutureValue.
      \[CustomAuthenticationFactors \<String\[\]\>\]: List of custom controls IDs required by the policy.
To learn more about custom control, see Custom controls (preview).
      \[Operator \<String\>\]: Defines the relationship of the grant controls.
Possible values: AND, OR.
      \[TermsOfUse \<String\[\]\>\]: List of terms of use IDs required by the policy.
    \[ModifiedDateTime \<DateTime?\>\]: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Readonly.
    \[SessionControls \<IMicrosoftGraphConditionalAccessSessionControls\>\]: conditionalAccessSessionControls
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[ApplicationEnforcedRestrictions \<IMicrosoftGraphApplicationEnforcedRestrictionsSessionControl\>\]: applicationEnforcedRestrictionsSessionControl
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[IsEnabled \<Boolean?\>\]: Specifies whether the session control is enabled.
      \[CloudAppSecurity \<IMicrosoftGraphCloudAppSecuritySessionControl\>\]: cloudAppSecuritySessionControl
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[IsEnabled \<Boolean?\>\]: Specifies whether the session control is enabled.
        \[CloudAppSecurityType \<String\>\]: cloudAppSecuritySessionControlType
      \[ContinuousAccessEvaluation \<IMicrosoftGraphContinuousAccessEvaluationSessionControl\>\]: continuousAccessEvaluationSessionControl
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[Mode \<String\>\]: continuousAccessEvaluationMode
      \[DisableResilienceDefaults \<Boolean?\>\]: Session control that determines whether it's acceptable for Microsoft Entra ID to extend existing sessions based on information collected prior to an outage or not.
      \[PersistentBrowser \<IMicrosoftGraphPersistentBrowserSessionControl\>\]: persistentBrowserSessionControl
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[IsEnabled \<Boolean?\>\]: Specifies whether the session control is enabled.
        \[Mode \<String\>\]: persistentBrowserSessionMode
      \[SecureSignInSession \<IMicrosoftGraphSecureSignInSessionControl\>\]: secureSignInSessionControl
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[IsEnabled \<Boolean?\>\]: Specifies whether the session control is enabled.
      \[SignInFrequency \<IMicrosoftGraphSignInFrequencySessionControl\>\]: signInFrequencySessionControl
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[IsEnabled \<Boolean?\>\]: Specifies whether the session control is enabled.
        \[AuthenticationType \<String\>\]: signInFrequencyAuthenticationType
        \[FrequencyInterval \<String\>\]: signInFrequencyInterval
        \[Type \<String\>\]: signinFrequencyType
        \[Value \<Int32?\>\]: The number of days or hours.
    \[State \<String\>\]: conditionalAccessPolicyState
  \[Templates \<IMicrosoftGraphConditionalAccessTemplate\[\]\>\]: Read-only.
Nullable.
Returns a collection of the specified Conditional Access templates.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[Description \<String\>\]: The user-friendly name of the template.
    \[Details \<IMicrosoftGraphConditionalAccessPolicyDetail\>\]: conditionalAccessPolicyDetail
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Conditions \<IMicrosoftGraphConditionalAccessConditionSet\>\]: conditionalAccessConditionSet
      \[GrantControls \<IMicrosoftGraphConditionalAccessGrantControls\>\]: conditionalAccessGrantControls
      \[SessionControls \<IMicrosoftGraphConditionalAccessSessionControls\>\]: conditionalAccessSessionControls
    \[Name \<String\>\]: The user-friendly name of the template.
    \[Scenarios \<String\>\]: templateScenarios

NAMEDLOCATIONS \<IMicrosoftGraphNamedLocation\[\]\>: Read-only.
Nullable.
Returns a collection of the specified named locations.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[CreatedDateTime \<DateTime?\>\]: The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
  \[DisplayName \<String\>\]: Human-readable name of the location.
  \[ModifiedDateTime \<DateTime?\>\]: The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.

POLICIES \<IMicrosoftGraphConditionalAccessPolicy\[\]\>: Read-only.
Nullable.
Returns a collection of the specified Conditional Access policies.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[Conditions \<IMicrosoftGraphConditionalAccessConditionSet\>\]: conditionalAccessConditionSet
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Applications \<IMicrosoftGraphConditionalAccessApplications\>\]: conditionalAccessApplications
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[ApplicationFilter \<IMicrosoftGraphConditionalAccessFilter\>\]: conditionalAccessFilter
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[Mode \<String\>\]: filterMode
        \[Rule \<String\>\]: Rule syntax is similar to that used for membership rules for groups in Microsoft Entra ID.
For details, see rules with multiple expressions
      \[ExcludeApplications \<String\[\]\>\]: Can be one of the following:  The list of client IDs (appId) explicitly excluded from the policy.
Office365 - For the list of apps included in Office365, see Conditional Access target apps: Office 365
      \[IncludeApplications \<String\[\]\>\]: Can be one of the following:  The list of client IDs (appId) the policy applies to, unless explicitly excluded (in excludeApplications)  All  Office365 - For the list of apps included in Office365, see Conditional Access target apps: Office 365
      \[IncludeAuthenticationContextClassReferences \<String\[\]\>\]: Authentication context class references include.
Supported values are c1 through c25.
      \[IncludeUserActions \<String\[\]\>\]: User actions to include.
Supported values are urn:user:registersecurityinfo and urn:user:registerdevice
    \[ClientAppTypes \<String\[\]\>\]: Client application types included in the policy.
Possible values are: all, browser, mobileAppsAndDesktopClients, exchangeActiveSync, easSupported, other.
Required. 
The easUnsupported enumeration member will be deprecated in favor of exchangeActiveSync which includes EAS supported and unsupported platforms.
    \[ClientApplications \<IMicrosoftGraphConditionalAccessClientApplications\>\]: conditionalAccessClientApplications
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[ExcludeServicePrincipals \<String\[\]\>\]: Service principal IDs excluded from the policy scope.
      \[IncludeServicePrincipals \<String\[\]\>\]: Service principal IDs included in the policy scope, or ServicePrincipalsInMyTenant.
      \[ServicePrincipalFilter \<IMicrosoftGraphConditionalAccessFilter\>\]: conditionalAccessFilter
    \[DeviceStates \<IMicrosoftGraphConditionalAccessDeviceStates\>\]: conditionalAccessDeviceStates
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[ExcludeStates \<String\[\]\>\]: States excluded from the scope of the policy.
Possible values: Compliant, DomainJoined.
      \[IncludeStates \<String\[\]\>\]: States in the scope of the policy.
All is the only allowed value.
    \[Devices \<IMicrosoftGraphConditionalAccessDevices\>\]: conditionalAccessDevices
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[DeviceFilter \<IMicrosoftGraphConditionalAccessFilter\>\]: conditionalAccessFilter
      \[ExcludeDeviceStates \<String\[\]\>\]: 
      \[ExcludeDevices \<String\[\]\>\]: States excluded from the scope of the policy.
Possible values: Compliant, DomainJoined.
Cannot be set if deviceFIlter is set.
      \[IncludeDeviceStates \<String\[\]\>\]: 
      \[IncludeDevices \<String\[\]\>\]: States in the scope of the policy.
All is the only allowed value.
Cannot be set if deviceFilter is set.
    \[Locations \<IMicrosoftGraphConditionalAccessLocations\>\]: conditionalAccessLocations
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[ExcludeLocations \<String\[\]\>\]: Location IDs excluded from scope of policy.
      \[IncludeLocations \<String\[\]\>\]: Location IDs in scope of policy unless explicitly excluded, All, or AllTrusted.
    \[Platforms \<IMicrosoftGraphConditionalAccessPlatforms\>\]: conditionalAccessPlatforms
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[ExcludePlatforms \<String\[\]\>\]: Possible values are: android, iOS, windows, windowsPhone, macOS, all, unknownFutureValue, linux.
      \[IncludePlatforms \<String\[\]\>\]: Possible values are: android, iOS, windows, windowsPhone, macOS, all, unknownFutureValue,linux.
    \[ServicePrincipalRiskLevels \<String\[\]\>\]: Service principal risk levels included in the policy.
Possible values are: low, medium, high, none, unknownFutureValue.
    \[SignInRiskLevels \<String\[\]\>\]: Sign-in risk levels included in the policy.
Possible values are: low, medium, high, hidden, none, unknownFutureValue.
Required.
    \[UserRiskLevels \<String\[\]\>\]: User risk levels included in the policy.
Possible values are: low, medium, high, hidden, none, unknownFutureValue.
Required.
    \[Users \<IMicrosoftGraphConditionalAccessUsers\>\]: conditionalAccessUsers
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[ExcludeGroups \<String\[\]\>\]: Group IDs excluded from scope of policy.
      \[ExcludeGuestsOrExternalUsers \<IMicrosoftGraphConditionalAccessGuestsOrExternalUsers\>\]: conditionalAccessGuestsOrExternalUsers
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[ExternalTenants \<IMicrosoftGraphConditionalAccessExternalTenants\>\]: conditionalAccessExternalTenants
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[MembershipKind \<String\>\]: conditionalAccessExternalTenantsMembershipKind
        \[GuestOrExternalUserTypes \<String\>\]: conditionalAccessGuestOrExternalUserTypes
      \[ExcludeRoles \<String\[\]\>\]: Role IDs excluded from scope of policy.
      \[ExcludeUsers \<String\[\]\>\]: User IDs excluded from scope of policy and/or GuestsOrExternalUsers.
      \[IncludeGroups \<String\[\]\>\]: Group IDs in scope of policy unless explicitly excluded.
      \[IncludeGuestsOrExternalUsers \<IMicrosoftGraphConditionalAccessGuestsOrExternalUsers\>\]: conditionalAccessGuestsOrExternalUsers
      \[IncludeRoles \<String\[\]\>\]: Role IDs in scope of policy unless explicitly excluded.
      \[IncludeUsers \<String\[\]\>\]: User IDs in scope of policy unless explicitly excluded, None, All, or GuestsOrExternalUsers.
  \[CreatedDateTime \<DateTime?\>\]: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Readonly.
  \[Description \<String\>\]: Not used.
  \[DisplayName \<String\>\]: Specifies a display name for the conditionalAccessPolicy object.
  \[GrantControls \<IMicrosoftGraphConditionalAccessGrantControls\>\]: conditionalAccessGrantControls
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[AuthenticationStrength \<IMicrosoftGraphAuthenticationStrengthPolicy\>\]: authenticationStrengthPolicy
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
    \[BuiltInControls \<String\[\]\>\]: List of values of built-in controls required by the policy.
Possible values: block, mfa, compliantDevice, domainJoinedDevice, approvedApplication, compliantApplication, passwordChange, unknownFutureValue.
    \[CustomAuthenticationFactors \<String\[\]\>\]: List of custom controls IDs required by the policy.
To learn more about custom control, see Custom controls (preview).
    \[Operator \<String\>\]: Defines the relationship of the grant controls.
Possible values: AND, OR.
    \[TermsOfUse \<String\[\]\>\]: List of terms of use IDs required by the policy.
  \[ModifiedDateTime \<DateTime?\>\]: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Readonly.
  \[SessionControls \<IMicrosoftGraphConditionalAccessSessionControls\>\]: conditionalAccessSessionControls
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[ApplicationEnforcedRestrictions \<IMicrosoftGraphApplicationEnforcedRestrictionsSessionControl\>\]: applicationEnforcedRestrictionsSessionControl
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[IsEnabled \<Boolean?\>\]: Specifies whether the session control is enabled.
    \[CloudAppSecurity \<IMicrosoftGraphCloudAppSecuritySessionControl\>\]: cloudAppSecuritySessionControl
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[IsEnabled \<Boolean?\>\]: Specifies whether the session control is enabled.
      \[CloudAppSecurityType \<String\>\]: cloudAppSecuritySessionControlType
    \[ContinuousAccessEvaluation \<IMicrosoftGraphContinuousAccessEvaluationSessionControl\>\]: continuousAccessEvaluationSessionControl
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Mode \<String\>\]: continuousAccessEvaluationMode
    \[DisableResilienceDefaults \<Boolean?\>\]: Session control that determines whether it's acceptable for Microsoft Entra ID to extend existing sessions based on information collected prior to an outage or not.
    \[PersistentBrowser \<IMicrosoftGraphPersistentBrowserSessionControl\>\]: persistentBrowserSessionControl
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[IsEnabled \<Boolean?\>\]: Specifies whether the session control is enabled.
      \[Mode \<String\>\]: persistentBrowserSessionMode
    \[SecureSignInSession \<IMicrosoftGraphSecureSignInSessionControl\>\]: secureSignInSessionControl
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[IsEnabled \<Boolean?\>\]: Specifies whether the session control is enabled.
    \[SignInFrequency \<IMicrosoftGraphSignInFrequencySessionControl\>\]: signInFrequencySessionControl
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[IsEnabled \<Boolean?\>\]: Specifies whether the session control is enabled.
      \[AuthenticationType \<String\>\]: signInFrequencyAuthenticationType
      \[FrequencyInterval \<String\>\]: signInFrequencyInterval
      \[Type \<String\>\]: signinFrequencyType
      \[Value \<Int32?\>\]: The number of days or hours.
  \[State \<String\>\]: conditionalAccessPolicyState

TEMPLATES \<IMicrosoftGraphConditionalAccessTemplate\[\]\>: Read-only.
Nullable.
Returns a collection of the specified Conditional Access templates.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[Description \<String\>\]: The user-friendly name of the template.
  \[Details \<IMicrosoftGraphConditionalAccessPolicyDetail\>\]: conditionalAccessPolicyDetail
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Conditions \<IMicrosoftGraphConditionalAccessConditionSet\>\]: conditionalAccessConditionSet
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Applications \<IMicrosoftGraphConditionalAccessApplications\>\]: conditionalAccessApplications
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[ApplicationFilter \<IMicrosoftGraphConditionalAccessFilter\>\]: conditionalAccessFilter
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[Mode \<String\>\]: filterMode
          \[Rule \<String\>\]: Rule syntax is similar to that used for membership rules for groups in Microsoft Entra ID.
For details, see rules with multiple expressions
        \[ExcludeApplications \<String\[\]\>\]: Can be one of the following:  The list of client IDs (appId) explicitly excluded from the policy.
Office365 - For the list of apps included in Office365, see Conditional Access target apps: Office 365
        \[IncludeApplications \<String\[\]\>\]: Can be one of the following:  The list of client IDs (appId) the policy applies to, unless explicitly excluded (in excludeApplications)  All  Office365 - For the list of apps included in Office365, see Conditional Access target apps: Office 365
        \[IncludeAuthenticationContextClassReferences \<String\[\]\>\]: Authentication context class references include.
Supported values are c1 through c25.
        \[IncludeUserActions \<String\[\]\>\]: User actions to include.
Supported values are urn:user:registersecurityinfo and urn:user:registerdevice
      \[ClientAppTypes \<String\[\]\>\]: Client application types included in the policy.
Possible values are: all, browser, mobileAppsAndDesktopClients, exchangeActiveSync, easSupported, other.
Required. 
The easUnsupported enumeration member will be deprecated in favor of exchangeActiveSync which includes EAS supported and unsupported platforms.
      \[ClientApplications \<IMicrosoftGraphConditionalAccessClientApplications\>\]: conditionalAccessClientApplications
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[ExcludeServicePrincipals \<String\[\]\>\]: Service principal IDs excluded from the policy scope.
        \[IncludeServicePrincipals \<String\[\]\>\]: Service principal IDs included in the policy scope, or ServicePrincipalsInMyTenant.
        \[ServicePrincipalFilter \<IMicrosoftGraphConditionalAccessFilter\>\]: conditionalAccessFilter
      \[DeviceStates \<IMicrosoftGraphConditionalAccessDeviceStates\>\]: conditionalAccessDeviceStates
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[ExcludeStates \<String\[\]\>\]: States excluded from the scope of the policy.
Possible values: Compliant, DomainJoined.
        \[IncludeStates \<String\[\]\>\]: States in the scope of the policy.
All is the only allowed value.
      \[Devices \<IMicrosoftGraphConditionalAccessDevices\>\]: conditionalAccessDevices
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[DeviceFilter \<IMicrosoftGraphConditionalAccessFilter\>\]: conditionalAccessFilter
        \[ExcludeDeviceStates \<String\[\]\>\]: 
        \[ExcludeDevices \<String\[\]\>\]: States excluded from the scope of the policy.
Possible values: Compliant, DomainJoined.
Cannot be set if deviceFIlter is set.
        \[IncludeDeviceStates \<String\[\]\>\]: 
        \[IncludeDevices \<String\[\]\>\]: States in the scope of the policy.
All is the only allowed value.
Cannot be set if deviceFilter is set.
      \[Locations \<IMicrosoftGraphConditionalAccessLocations\>\]: conditionalAccessLocations
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[ExcludeLocations \<String\[\]\>\]: Location IDs excluded from scope of policy.
        \[IncludeLocations \<String\[\]\>\]: Location IDs in scope of policy unless explicitly excluded, All, or AllTrusted.
      \[Platforms \<IMicrosoftGraphConditionalAccessPlatforms\>\]: conditionalAccessPlatforms
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[ExcludePlatforms \<String\[\]\>\]: Possible values are: android, iOS, windows, windowsPhone, macOS, all, unknownFutureValue, linux.
        \[IncludePlatforms \<String\[\]\>\]: Possible values are: android, iOS, windows, windowsPhone, macOS, all, unknownFutureValue,linux.
      \[ServicePrincipalRiskLevels \<String\[\]\>\]: Service principal risk levels included in the policy.
Possible values are: low, medium, high, none, unknownFutureValue.
      \[SignInRiskLevels \<String\[\]\>\]: Sign-in risk levels included in the policy.
Possible values are: low, medium, high, hidden, none, unknownFutureValue.
Required.
      \[UserRiskLevels \<String\[\]\>\]: User risk levels included in the policy.
Possible values are: low, medium, high, hidden, none, unknownFutureValue.
Required.
      \[Users \<IMicrosoftGraphConditionalAccessUsers\>\]: conditionalAccessUsers
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[ExcludeGroups \<String\[\]\>\]: Group IDs excluded from scope of policy.
        \[ExcludeGuestsOrExternalUsers \<IMicrosoftGraphConditionalAccessGuestsOrExternalUsers\>\]: conditionalAccessGuestsOrExternalUsers
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[ExternalTenants \<IMicrosoftGraphConditionalAccessExternalTenants\>\]: conditionalAccessExternalTenants
            \[(Any) \<Object\>\]: This indicates any property can be added to this object.
            \[MembershipKind \<String\>\]: conditionalAccessExternalTenantsMembershipKind
          \[GuestOrExternalUserTypes \<String\>\]: conditionalAccessGuestOrExternalUserTypes
        \[ExcludeRoles \<String\[\]\>\]: Role IDs excluded from scope of policy.
        \[ExcludeUsers \<String\[\]\>\]: User IDs excluded from scope of policy and/or GuestsOrExternalUsers.
        \[IncludeGroups \<String\[\]\>\]: Group IDs in scope of policy unless explicitly excluded.
        \[IncludeGuestsOrExternalUsers \<IMicrosoftGraphConditionalAccessGuestsOrExternalUsers\>\]: conditionalAccessGuestsOrExternalUsers
        \[IncludeRoles \<String\[\]\>\]: Role IDs in scope of policy unless explicitly excluded.
        \[IncludeUsers \<String\[\]\>\]: User IDs in scope of policy unless explicitly excluded, None, All, or GuestsOrExternalUsers.
    \[GrantControls \<IMicrosoftGraphConditionalAccessGrantControls\>\]: conditionalAccessGrantControls
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[AuthenticationStrength \<IMicrosoftGraphAuthenticationStrengthPolicy\>\]: authenticationStrengthPolicy
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
      \[BuiltInControls \<String\[\]\>\]: List of values of built-in controls required by the policy.
Possible values: block, mfa, compliantDevice, domainJoinedDevice, approvedApplication, compliantApplication, passwordChange, unknownFutureValue.
      \[CustomAuthenticationFactors \<String\[\]\>\]: List of custom controls IDs required by the policy.
To learn more about custom control, see Custom controls (preview).
      \[Operator \<String\>\]: Defines the relationship of the grant controls.
Possible values: AND, OR.
      \[TermsOfUse \<String\[\]\>\]: List of terms of use IDs required by the policy.
    \[SessionControls \<IMicrosoftGraphConditionalAccessSessionControls\>\]: conditionalAccessSessionControls
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[ApplicationEnforcedRestrictions \<IMicrosoftGraphApplicationEnforcedRestrictionsSessionControl\>\]: applicationEnforcedRestrictionsSessionControl
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[IsEnabled \<Boolean?\>\]: Specifies whether the session control is enabled.
      \[CloudAppSecurity \<IMicrosoftGraphCloudAppSecuritySessionControl\>\]: cloudAppSecuritySessionControl
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[IsEnabled \<Boolean?\>\]: Specifies whether the session control is enabled.
        \[CloudAppSecurityType \<String\>\]: cloudAppSecuritySessionControlType
      \[ContinuousAccessEvaluation \<IMicrosoftGraphContinuousAccessEvaluationSessionControl\>\]: continuousAccessEvaluationSessionControl
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[Mode \<String\>\]: continuousAccessEvaluationMode
      \[DisableResilienceDefaults \<Boolean?\>\]: Session control that determines whether it's acceptable for Microsoft Entra ID to extend existing sessions based on information collected prior to an outage or not.
      \[PersistentBrowser \<IMicrosoftGraphPersistentBrowserSessionControl\>\]: persistentBrowserSessionControl
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[IsEnabled \<Boolean?\>\]: Specifies whether the session control is enabled.
        \[Mode \<String\>\]: persistentBrowserSessionMode
      \[SecureSignInSession \<IMicrosoftGraphSecureSignInSessionControl\>\]: secureSignInSessionControl
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[IsEnabled \<Boolean?\>\]: Specifies whether the session control is enabled.
      \[SignInFrequency \<IMicrosoftGraphSignInFrequencySessionControl\>\]: signInFrequencySessionControl
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[IsEnabled \<Boolean?\>\]: Specifies whether the session control is enabled.
        \[AuthenticationType \<String\>\]: signInFrequencyAuthenticationType
        \[FrequencyInterval \<String\>\]: signInFrequencyInterval
        \[Type \<String\>\]: signinFrequencyType
        \[Value \<Int32?\>\]: The number of days or hours.
  \[Name \<String\>\]: The user-friendly name of the template.
  \[Scenarios \<String\>\]: templateScenarios

## RELATED LINKS
[Update-MgIdentityConditionalAccess](/powershell/module/Microsoft.Graph.Identity.SignIns/Update-MgIdentityConditionalAccess?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetaidentityconditionalaccess](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetaidentityconditionalaccess)


