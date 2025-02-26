---
external help file: Microsoft.Graph.Applications-help.xml
Module Name: Microsoft.Graph.Applications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.applications/remove-mgapplicationpassword
schema: 2.0.0
ms.prod: applications
---

# Remove-MgApplicationPassword

## SYNOPSIS
Remove a password from an application.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the beta release of this cmdlet, view [Remove-MgBetaApplicationPassword](/powershell/module/Microsoft.Graph.Beta.Applications/Remove-MgBetaApplicationPassword?view=graph-powershell-beta)

## SYNTAX

### RemoveExpanded (Default)
```
Remove-MgApplicationPassword -ApplicationId <String> [-AdditionalProperties <Hashtable>] [-KeyId <String>]
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Remove
```
Remove-MgApplicationPassword -ApplicationId <String>
 -BodyParameter <IPathsHv033BApplicationsApplicationIdMicrosoftGraphRemovepasswordPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### RemoveViaIdentityExpanded
```
Remove-MgApplicationPassword -InputObject <IApplicationsIdentity> [-AdditionalProperties <Hashtable>]
 [-KeyId <String>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### RemoveViaIdentity
```
Remove-MgApplicationPassword -InputObject <IApplicationsIdentity>
 -BodyParameter <IPathsHv033BApplicationsApplicationIdMicrosoftGraphRemovepasswordPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Remove a password from an application.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Using the Remove-MgApplicationPassword Cmdlet
```powershell
Import-Module Microsoft.Graph.Applications
$params = @{
	KeyId = "f0b0b335-1d71-4883-8f98-567911bfdca6"
}
Remove-MgApplicationPassword -ApplicationId $applicationId -BodyParameter $params
```
This example shows how to use the Remove-MgApplicationPassword Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: RemoveExpanded, RemoveViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ApplicationId
The unique identifier of application

```yaml
Type: String
Parameter Sets: RemoveExpanded, Remove
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPathsHv033BApplicationsApplicationIdMicrosoftGraphRemovepasswordPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Remove, RemoveViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IApplicationsIdentity
Parameter Sets: RemoveViaIdentityExpanded, RemoveViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -KeyId
.

```yaml
Type: String
Parameter Sets: RemoveExpanded, RemoveViaIdentityExpanded
Aliases:

Required: False
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
### Microsoft.Graph.PowerShell.Models.IPathsHv033BApplicationsApplicationIdMicrosoftGraphRemovepasswordPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IPathsHv033BApplicationsApplicationIdMicrosoftGraphRemovepasswordPostRequestbodyContentApplicationJsonSchema\>: .
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[KeyId \<String\>\]: 

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
[Remove-MgBetaApplicationPassword](/powershell/module/Microsoft.Graph.Beta.Applications/Remove-MgBetaApplicationPassword?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.applications/remove-mgapplicationpassword](https://learn.microsoft.com/powershell/module/microsoft.graph.applications/remove-mgapplicationpassword)



