---
external help file: Microsoft.Graph.Identity.Governance-help.xml
Module Name: Microsoft.Graph.Identity.Governance
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/get-mgrolemanagementdirectoryroleassignment
schema: 2.0.0
ms.prod: directory-management
ms.prod: directory-management
---

# Get-MgRoleManagementDirectoryRoleAssignment

## SYNOPSIS
Retrieve the properties and relationships of a unifiedRoleAssignment object.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the beta release of this cmdlet, view [Get-MgBetaRoleManagementDirectoryRoleAssignment](/powershell/module/Microsoft.Graph.Beta.Identity.Governance/Get-MgBetaRoleManagementDirectoryRoleAssignment?view=graph-powershell-beta)

## SYNTAX

### List (Default)
```
Get-MgRoleManagementDirectoryRoleAssignment [-ExpandProperty <String[]>] [-Property <String[]>]
 [-Filter <String>] [-Search <String>] [-Skip <Int32>] [-Sort <String[]>] [-Top <Int32>] [-PageSize <Int32>]
 [-All] [-CountVariable <String>] [<CommonParameters>]
```

### Get
```
Get-MgRoleManagementDirectoryRoleAssignment -UnifiedRoleAssignmentId <String> [-ExpandProperty <String[]>]
 [-Property <String[]>] [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgRoleManagementDirectoryRoleAssignment -InputObject <IIdentityGovernanceIdentity>
 [-ExpandProperty <String[]>] [-Property <String[]>] [<CommonParameters>]
```

## DESCRIPTION
Retrieve the properties and relationships of a unifiedRoleAssignment object.
This API is available in the following national cloud deployments.

## PARAMETERS

### -All
List all pages.

```yaml
Type: SwitchParameter
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -CountVariable
Specifies a count of the total number of items in a collection.
By default, this variable will be set in the global scope.

```yaml
Type: String
Parameter Sets: List
Aliases: CV

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExpandProperty
Expand related entities

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Expand

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Filter
Filter items by property values

```yaml
Type: String
Parameter Sets: List
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
Type: IIdentityGovernanceIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PageSize
Sets the page size of results.

```yaml
Type: Int32
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Property
Select properties to be returned

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Select

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Search
Search items by search phrases

```yaml
Type: String
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Sort
Order items by property values

```yaml
Type: String[]
Parameter Sets: List
Aliases: OrderBy

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Top
Show only the first n items

```yaml
Type: Int32
Parameter Sets: List
Aliases: Limit

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -UnifiedRoleAssignmentId
The unique identifier of unifiedRoleAssignment

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

### -Skip
Skip the first n items

```yaml
Type: Int32
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IIdentityGovernanceIdentity
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphUnifiedRoleAssignment
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT \<IIdentityGovernanceIdentity\>: Identity Parameter
  \[AccessPackageAssignmentId \<String\>\]: The unique identifier of accessPackageAssignment
  \[AccessPackageAssignmentPolicyId \<String\>\]: The unique identifier of accessPackageAssignmentPolicy
  \[AccessPackageAssignmentRequestId \<String\>\]: The unique identifier of accessPackageAssignmentRequest
  \[AccessPackageCatalogId \<String\>\]: The unique identifier of accessPackageCatalog
  \[AccessPackageId \<String\>\]: The unique identifier of accessPackage
  \[AccessPackageId1 \<String\>\]: The unique identifier of accessPackage
  \[AccessPackageQuestionId \<String\>\]: The unique identifier of accessPackageQuestion
  \[AccessPackageResourceEnvironmentId \<String\>\]: The unique identifier of accessPackageResourceEnvironment
  \[AccessPackageResourceId \<String\>\]: The unique identifier of accessPackageResource
  \[AccessPackageResourceRequestId \<String\>\]: The unique identifier of accessPackageResourceRequest
  \[AccessPackageResourceRoleId \<String\>\]: The unique identifier of accessPackageResourceRole
  \[AccessPackageResourceRoleId1 \<String\>\]: The unique identifier of accessPackageResourceRole
  \[AccessPackageResourceRoleScopeId \<String\>\]: The unique identifier of accessPackageResourceRoleScope
  \[AccessPackageResourceScopeId \<String\>\]: The unique identifier of accessPackageResourceScope
  \[AccessPackageResourceScopeId1 \<String\>\]: The unique identifier of accessPackageResourceScope
  \[AccessReviewHistoryDefinitionId \<String\>\]: The unique identifier of accessReviewHistoryDefinition
  \[AccessReviewHistoryInstanceId \<String\>\]: The unique identifier of accessReviewHistoryInstance
  \[AccessReviewInstanceDecisionItemId \<String\>\]: The unique identifier of accessReviewInstanceDecisionItem
  \[AccessReviewInstanceId \<String\>\]: The unique identifier of accessReviewInstance
  \[AccessReviewReviewerId \<String\>\]: The unique identifier of accessReviewReviewer
  \[AccessReviewScheduleDefinitionId \<String\>\]: The unique identifier of accessReviewScheduleDefinition
  \[AccessReviewStageId \<String\>\]: The unique identifier of accessReviewStage
  \[AgreementAcceptanceId \<String\>\]: The unique identifier of agreementAcceptance
  \[AgreementFileLocalizationId \<String\>\]: The unique identifier of agreementFileLocalization
  \[AgreementFileVersionId \<String\>\]: The unique identifier of agreementFileVersion
  \[AgreementId \<String\>\]: The unique identifier of agreement
  \[AppConsentRequestId \<String\>\]: The unique identifier of appConsentRequest
  \[ApprovalId \<String\>\]: The unique identifier of approval
  \[ApprovalStageId \<String\>\]: The unique identifier of approvalStage
  \[ConnectedOrganizationId \<String\>\]: The unique identifier of connectedOrganization
  \[CustomCalloutExtensionId \<String\>\]: The unique identifier of customCalloutExtension
  \[CustomExtensionStageSettingId \<String\>\]: The unique identifier of customExtensionStageSetting
  \[CustomTaskExtensionId \<String\>\]: The unique identifier of customTaskExtension
  \[DirectoryObjectId \<String\>\]: The unique identifier of directoryObject
  \[EndDateTime \<DateTime?\>\]: Usage: endDateTime={endDateTime}
  \[GovernanceInsightId \<String\>\]: The unique identifier of governanceInsight
  \[GroupId \<String\>\]: The unique identifier of group
  \[IncompatibleAccessPackageId \<String\>\]: Usage: incompatibleAccessPackageId='{incompatibleAccessPackageId}'
  \[On \<String\>\]: Usage: on='{on}'
  \[PrivilegedAccessGroupAssignmentScheduleId \<String\>\]: The unique identifier of privilegedAccessGroupAssignmentSchedule
  \[PrivilegedAccessGroupAssignmentScheduleInstanceId \<String\>\]: The unique identifier of privilegedAccessGroupAssignmentScheduleInstance
  \[PrivilegedAccessGroupAssignmentScheduleRequestId \<String\>\]: The unique identifier of privilegedAccessGroupAssignmentScheduleRequest
  \[PrivilegedAccessGroupEligibilityScheduleId \<String\>\]: The unique identifier of privilegedAccessGroupEligibilitySchedule
  \[PrivilegedAccessGroupEligibilityScheduleInstanceId \<String\>\]: The unique identifier of privilegedAccessGroupEligibilityScheduleInstance
  \[PrivilegedAccessGroupEligibilityScheduleRequestId \<String\>\]: The unique identifier of privilegedAccessGroupEligibilityScheduleRequest
  \[RunId \<String\>\]: The unique identifier of run
  \[StartDateTime \<DateTime?\>\]: Usage: startDateTime={startDateTime}
  \[TaskDefinitionId \<String\>\]: The unique identifier of taskDefinition
  \[TaskId \<String\>\]: The unique identifier of task
  \[TaskProcessingResultId \<String\>\]: The unique identifier of taskProcessingResult
  \[TaskReportId \<String\>\]: The unique identifier of taskReport
  \[UnifiedRbacResourceActionId \<String\>\]: The unique identifier of unifiedRbacResourceAction
  \[UnifiedRbacResourceNamespaceId \<String\>\]: The unique identifier of unifiedRbacResourceNamespace
  \[UnifiedRoleAssignmentId \<String\>\]: The unique identifier of unifiedRoleAssignment
  \[UnifiedRoleAssignmentScheduleId \<String\>\]: The unique identifier of unifiedRoleAssignmentSchedule
  \[UnifiedRoleAssignmentScheduleInstanceId \<String\>\]: The unique identifier of unifiedRoleAssignmentScheduleInstance
  \[UnifiedRoleAssignmentScheduleRequestId \<String\>\]: The unique identifier of unifiedRoleAssignmentScheduleRequest
  \[UnifiedRoleDefinitionId \<String\>\]: The unique identifier of unifiedRoleDefinition
  \[UnifiedRoleDefinitionId1 \<String\>\]: The unique identifier of unifiedRoleDefinition
  \[UnifiedRoleEligibilityScheduleId \<String\>\]: The unique identifier of unifiedRoleEligibilitySchedule
  \[UnifiedRoleEligibilityScheduleInstanceId \<String\>\]: The unique identifier of unifiedRoleEligibilityScheduleInstance
  \[UnifiedRoleEligibilityScheduleRequestId \<String\>\]: The unique identifier of unifiedRoleEligibilityScheduleRequest
  \[UserConsentRequestId \<String\>\]: The unique identifier of userConsentRequest
  \[UserId \<String\>\]: The unique identifier of user
  \[UserProcessingResultId \<String\>\]: The unique identifier of userProcessingResult
  \[WorkflowId \<String\>\]: The unique identifier of workflow
  \[WorkflowTemplateId \<String\>\]: The unique identifier of workflowTemplate
  \[WorkflowVersionNumber \<Int32?\>\]: The unique identifier of workflowVersion

## RELATED LINKS
[Get-MgBetaRoleManagementDirectoryRoleAssignment](/powershell/module/Microsoft.Graph.Beta.Identity.Governance/Get-MgBetaRoleManagementDirectoryRoleAssignment?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/get-mgrolemanagementdirectoryroleassignment](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/get-mgrolemanagementdirectoryroleassignment)



