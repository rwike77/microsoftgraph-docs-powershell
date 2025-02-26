---
external help file: Microsoft.Graph.Applications-help.xml
Module Name: Microsoft.Graph.Applications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.applications/new-mgserviceprincipalremotedesktopsecurityconfigurationtargetdevicegroup
schema: 2.0.0
---

# New-MgServicePrincipalRemoteDesktopSecurityConfigurationTargetDeviceGroup

## SYNOPSIS
Create new navigation property to targetDeviceGroups for servicePrincipals

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaServicePrincipalRemoteDesktopSecurityConfigurationTargetDeviceGroup](/powershell/module/Microsoft.Graph.Beta.Applications/New-MgBetaServicePrincipalRemoteDesktopSecurityConfigurationTargetDeviceGroup?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgServicePrincipalRemoteDesktopSecurityConfigurationTargetDeviceGroup -ServicePrincipalId <String>
 [-AdditionalProperties <Hashtable>] [-DisplayName <String>] [-Id <String>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Create
```
New-MgServicePrincipalRemoteDesktopSecurityConfigurationTargetDeviceGroup -ServicePrincipalId <String>
 -BodyParameter <IMicrosoftGraphTargetDeviceGroup> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgServicePrincipalRemoteDesktopSecurityConfigurationTargetDeviceGroup -InputObject <IApplicationsIdentity>
 [-AdditionalProperties <Hashtable>] [-DisplayName <String>] [-Id <String>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgServicePrincipalRemoteDesktopSecurityConfigurationTargetDeviceGroup -InputObject <IApplicationsIdentity>
 -BodyParameter <IMicrosoftGraphTargetDeviceGroup> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to targetDeviceGroups for servicePrincipals

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
targetDeviceGroup
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphTargetDeviceGroup
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DisplayName
.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Type: IApplicationsIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ServicePrincipalId
The unique identifier of servicePrincipal

```yaml
Type: String
Parameter Sets: CreateExpanded, Create
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

### Microsoft.Graph.PowerShell.Models.IApplicationsIdentity
### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphTargetDeviceGroup
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphTargetDeviceGroup
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphTargetDeviceGroup\>: targetDeviceGroup
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[DisplayName \<String\>\]: 

INPUTOBJECT \<IApplicationsIdentity\>: Identity Parameter
  \[AppId \<String\>\]: Alternate key of application
  \[AppManagementPolicyId \<String\>\]: The unique identifier of appManagementPolicy
  \[AppRoleAssignmentId \<String\>\]: The unique identifier of appRoleAssignment
  \[ApplicationId \<String\>\]: The unique identifier of application
  \[ApplicationTemplateId \<String\>\]: The unique identifier of applicationTemplate
  \[ClaimsMappingPolicyId \<String\>\]: The unique identifier of claimsMappingPolicy
  \[DelegatedPermissionClassificationId \<String\>\]: The unique identifier of delegatedPermissionClassification
  \[DirectoryDefinitionId \<String\>\]: The unique identifier of directoryDefinition
  \[DirectoryObjectId \<String\>\]: The unique identifier of directoryObject
  \[EndpointId \<String\>\]: The unique identifier of endpoint
  \[ExtensionPropertyId \<String\>\]: The unique identifier of extensionProperty
  \[FederatedIdentityCredentialId \<String\>\]: The unique identifier of federatedIdentityCredential
  \[GroupId \<String\>\]: The unique identifier of group
  \[HomeRealmDiscoveryPolicyId \<String\>\]: The unique identifier of homeRealmDiscoveryPolicy
  \[OAuth2PermissionGrantId \<String\>\]: The unique identifier of oAuth2PermissionGrant
  \[ServicePrincipalId \<String\>\]: The unique identifier of servicePrincipal
  \[SynchronizationJobId \<String\>\]: The unique identifier of synchronizationJob
  \[SynchronizationTemplateId \<String\>\]: The unique identifier of synchronizationTemplate
  \[TargetDeviceGroupId \<String\>\]: The unique identifier of targetDeviceGroup
  \[TokenIssuancePolicyId \<String\>\]: The unique identifier of tokenIssuancePolicy
  \[TokenLifetimePolicyId \<String\>\]: The unique identifier of tokenLifetimePolicy
  \[UserId \<String\>\]: The unique identifier of user

## RELATED LINKS
[New-MgBetaServicePrincipalRemoteDesktopSecurityConfigurationTargetDeviceGroup](/powershell/module/Microsoft.Graph.Beta.Applications/New-MgBetaServicePrincipalRemoteDesktopSecurityConfigurationTargetDeviceGroup?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.applications/new-mgserviceprincipalremotedesktopsecurityconfigurationtargetdevicegroup](https://learn.microsoft.com/powershell/module/microsoft.graph.applications/new-mgserviceprincipalremotedesktopsecurityconfigurationtargetdevicegroup)




