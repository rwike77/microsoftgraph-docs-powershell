---
external help file: Microsoft.Graph.Beta.Identity.DirectoryManagement-help.xml
Module Name: Microsoft.Graph.Beta.Identity.DirectoryManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/invoke-mgbetatenantrelationshipmanagedtenantoffboard
schema: 2.0.0
---

# Invoke-MgBetaTenantRelationshipManagedTenantOffboard

## SYNOPSIS
Carries out the appropriate procedures to remove a managed tenant from the multitenant management platform.
No relationships, such as commerce and delegate administrative privileges, will be impacted.
The only change made by invoking this action is the tenant will be deprovisioned from the multitenant management platform.
This API is available in the following national cloud deployments.

## SYNTAX

### Tenant (Default)
```
Invoke-MgBetaTenantRelationshipManagedTenantOffboard -TenantId <String> [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### TenantViaIdentity
```
Invoke-MgBetaTenantRelationshipManagedTenantOffboard -InputObject <IIdentityDirectoryManagementIdentity>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Carries out the appropriate procedures to remove a managed tenant from the multitenant management platform.
No relationships, such as commerce and delegate administrative privileges, will be impacted.
The only change made by invoking this action is the tenant will be deprovisioned from the multitenant management platform.
This API is available in the following national cloud deployments.

## PARAMETERS

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IIdentityDirectoryManagementIdentity
Parameter Sets: TenantViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -TenantId
The unique identifier of tenant

```yaml
Type: String
Parameter Sets: Tenant
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

### Microsoft.Graph.Beta.PowerShell.Models.IIdentityDirectoryManagementIdentity
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphManagedTenantsTenant
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT \<IIdentityDirectoryManagementIdentity\>: Identity Parameter
  \[AdministrativeUnitId \<String\>\]: The unique identifier of administrativeUnit
  \[AllowedValueId \<String\>\]: The unique identifier of allowedValue
  \[AttributeSetId \<String\>\]: The unique identifier of attributeSet
  \[CertificateAuthorityAsEntityId \<String\>\]: The unique identifier of certificateAuthorityAsEntity
  \[CertificateBasedApplicationConfigurationId \<String\>\]: The unique identifier of certificateBasedApplicationConfiguration
  \[CommandId \<String\>\]: The unique identifier of command
  \[CompanySubscriptionId \<String\>\]: The unique identifier of companySubscription
  \[ContractId \<String\>\]: The unique identifier of contract
  \[CustomSecurityAttributeDefinitionId \<String\>\]: The unique identifier of customSecurityAttributeDefinition
  \[DeviceId \<String\>\]: The unique identifier of device
  \[DeviceLocalCredentialInfoId \<String\>\]: The unique identifier of deviceLocalCredentialInfo
  \[DirectoryObjectId \<String\>\]: The unique identifier of directoryObject
  \[DirectoryRoleId \<String\>\]: The unique identifier of directoryRole
  \[DirectoryRoleTemplateId \<String\>\]: The unique identifier of directoryRoleTemplate
  \[DirectorySettingId \<String\>\]: The unique identifier of directorySetting
  \[DirectorySettingTemplateId \<String\>\]: The unique identifier of directorySettingTemplate
  \[DomainDnsRecordId \<String\>\]: The unique identifier of domainDnsRecord
  \[DomainId \<String\>\]: The unique identifier of domain
  \[ExtensionId \<String\>\]: The unique identifier of extension
  \[FeatureRolloutPolicyId \<String\>\]: The unique identifier of featureRolloutPolicy
  \[IdentityProviderBaseId \<String\>\]: The unique identifier of identityProviderBase
  \[ImpactedResourceId \<String\>\]: The unique identifier of impactedResource
  \[InboundSharedUserProfileUserId \<String\>\]: The unique identifier of inboundSharedUserProfile
  \[InternalDomainFederationId \<String\>\]: The unique identifier of internalDomainFederation
  \[ManagedTenantAlertId \<String\>\]: The unique identifier of managedTenantAlert
  \[ManagementActionId \<String\>\]: The unique identifier of managementAction
  \[OnPremisesDirectorySynchronizationId \<String\>\]: The unique identifier of onPremisesDirectorySynchronization
  \[OrgContactId \<String\>\]: The unique identifier of orgContact
  \[OrganizationId \<String\>\]: The unique identifier of organization
  \[OrganizationalBrandingLocalizationId \<String\>\]: The unique identifier of organizationalBrandingLocalization
  \[OutboundSharedUserProfileUserId \<String\>\]: The unique identifier of outboundSharedUserProfile
  \[ProfileCardPropertyId \<String\>\]: The unique identifier of profileCardProperty
  \[RecommendationId \<String\>\]: The unique identifier of recommendation
  \[RoleTemplateId \<String\>\]: Alternate key of directoryRole
  \[ScopedRoleMembershipId \<String\>\]: The unique identifier of scopedRoleMembership
  \[SharedEmailDomainId \<String\>\]: The unique identifier of sharedEmailDomain
  \[SharedEmailDomainInvitationId \<String\>\]: The unique identifier of sharedEmailDomainInvitation
  \[SubscribedSkuId \<String\>\]: The unique identifier of subscribedSku
  \[TenantId \<String\>\]: The unique identifier of tenant
  \[TenantReferenceTenantId \<String\>\]: The unique identifier of tenantReference
  \[TenantTagId \<String\>\]: The unique identifier of tenantTag
  \[UsageRightId \<String\>\]: The unique identifier of usageRight
  \[UserId \<String\>\]: The unique identifier of user

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/invoke-mgbetatenantrelationshipmanagedtenantoffboard](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/invoke-mgbetatenantrelationshipmanagedtenantoffboard)



