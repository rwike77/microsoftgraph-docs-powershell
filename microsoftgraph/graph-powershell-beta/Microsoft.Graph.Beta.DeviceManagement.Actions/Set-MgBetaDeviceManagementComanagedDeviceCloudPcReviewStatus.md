---
external help file: Microsoft.Graph.Beta.DeviceManagement.Actions-help.xml
Module Name: Microsoft.Graph.Beta.DeviceManagement.Actions
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.actions/set-mgbetadevicemanagementcomanageddevicecloudpcreviewstatus
schema: 2.0.0
ms.prod: cloud-pc
---

# Set-MgBetaDeviceManagementComanagedDeviceCloudPcReviewStatus

## SYNOPSIS
Set the review status of a specific Cloud PC device.
Use this API to set the review status of a Cloud PC to in review if you consider a Cloud PC as suspicious.
After the review is completed, use this API again to set the Cloud PC back to a normal state.
This API is available in the following national cloud deployments.

## SYNTAX

### SetExpanded (Default)
```
Set-MgBetaDeviceManagementComanagedDeviceCloudPcReviewStatus -ManagedDeviceId <String>
 [-AdditionalProperties <Hashtable>] [-ReviewStatus <IMicrosoftGraphCloudPcReviewStatus>] [-PassThru] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Set
```
Set-MgBetaDeviceManagementComanagedDeviceCloudPcReviewStatus -ManagedDeviceId <String>
 -BodyParameter <IPaths17Ydg7DDevicemanagementComanageddevicesManageddeviceIdMicrosoftGraphSetcloudpcreviewstatusPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SetViaIdentityExpanded
```
Set-MgBetaDeviceManagementComanagedDeviceCloudPcReviewStatus -InputObject <IDeviceManagementActionsIdentity>
 [-AdditionalProperties <Hashtable>] [-ReviewStatus <IMicrosoftGraphCloudPcReviewStatus>] [-PassThru] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### SetViaIdentity
```
Set-MgBetaDeviceManagementComanagedDeviceCloudPcReviewStatus -InputObject <IDeviceManagementActionsIdentity>
 -BodyParameter <IPaths17Ydg7DDevicemanagementComanageddevicesManageddeviceIdMicrosoftGraphSetcloudpcreviewstatusPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Set the review status of a specific Cloud PC device.
Use this API to set the review status of a Cloud PC to in review if you consider a Cloud PC as suspicious.
After the review is completed, use this API again to set the Cloud PC back to a normal state.
This API is available in the following national cloud deployments.

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPaths17Ydg7DDevicemanagementComanageddevicesManageddeviceIdMicrosoftGraphSetcloudpcreviewstatusPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Set, SetViaIdentity
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
Type: IDeviceManagementActionsIdentity
Parameter Sets: SetViaIdentityExpanded, SetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ManagedDeviceId
The unique identifier of managedDevice

```yaml
Type: String
Parameter Sets: SetExpanded, Set
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

### -ReviewStatus
cloudPcReviewStatus
To construct, see NOTES section for REVIEWSTATUS properties and create a hash table.

```yaml
Type: IMicrosoftGraphCloudPcReviewStatus
Parameter Sets: SetExpanded, SetViaIdentityExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IDeviceManagementActionsIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IPaths17Ydg7DDevicemanagementComanageddevicesManageddeviceIdMicrosoftGraphSetcloudpcreviewstatusPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IPaths17Ydg7DDevicemanagementComanageddevicesManageddeviceIdMicrosoftGraphSetcloudpcreviewstatusPostRequestbodyContentApplicationJsonSchema\>: .
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[ReviewStatus \<IMicrosoftGraphCloudPcReviewStatus\>\]: cloudPcReviewStatus
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[AzureStorageAccountId \<String\>\]: The resource ID of the Azure Storage account in which the Cloud PC snapshot is being saved.
    \[AzureStorageAccountName \<String\>\]: The name of the Azure Storage account in which the Cloud PC snapshot is being saved.
    \[AzureStorageContainerName \<String\>\]: The name of the container in an Azure Storage account in which the Cloud PC snapshot is being saved.
    \[InReview \<Boolean?\>\]: True if the Cloud PC is set to in review by the administrator.
    \[RestorePointDateTime \<DateTime?\>\]: The specific date and time of the Cloud PC snapshot that was taken and saved automatically, when the Cloud PC is set to in review.
The timestamp is shown in ISO 8601 format and Coordinated Universal Time (UTC).
For example, midnight UTC on Jan 1, 2014 appears as 2014-01-01T00:00:00Z.
    \[ReviewStartDateTime \<DateTime?\>\]: The specific date and time when the Cloud PC was set to in review.
The timestamp is shown in ISO 8601 format and Coordinated Universal Time (UTC).
For example, midnight UTC on Jan 1, 2014 appears as 2014-01-01T00:00:00Z.
    \[SubscriptionId \<String\>\]: The ID of the Azure subscription in which the Cloud PC snapshot is being saved, in GUID format.
    \[SubscriptionName \<String\>\]: The name of the Azure subscription in which the Cloud PC snapshot is being saved.
    \[UserAccessLevel \<String\>\]: cloudPcUserAccessLevel

INPUTOBJECT \<IDeviceManagementActionsIdentity\>: Identity Parameter
  \[AlertRecordId \<String\>\]: The unique identifier of alertRecord
  \[AndroidDeviceOwnerEnrollmentProfileId \<String\>\]: The unique identifier of androidDeviceOwnerEnrollmentProfile
  \[AndroidForWorkEnrollmentProfileId \<String\>\]: The unique identifier of androidForWorkEnrollmentProfile
  \[AppLogCollectionRequestId \<String\>\]: The unique identifier of appLogCollectionRequest
  \[AppleUserInitiatedEnrollmentProfileId \<String\>\]: The unique identifier of appleUserInitiatedEnrollmentProfile
  \[CertificateConnectorDetailsId \<String\>\]: The unique identifier of certificateConnectorDetails
  \[CloudPcDeviceImageId \<String\>\]: The unique identifier of cloudPcDeviceImage
  \[CloudPcId \<String\>\]: The unique identifier of cloudPC
  \[CloudPcOnPremisesConnectionId \<String\>\]: The unique identifier of cloudPcOnPremisesConnection
  \[CloudPcProvisioningPolicyId \<String\>\]: The unique identifier of cloudPcProvisioningPolicy
  \[CloudPcUserSettingId \<String\>\]: The unique identifier of cloudPcUserSetting
  \[DataSharingConsentId \<String\>\]: The unique identifier of dataSharingConsent
  \[DepOnboardingSettingId \<String\>\]: The unique identifier of depOnboardingSetting
  \[DeviceCompliancePolicyId \<String\>\]: The unique identifier of deviceCompliancePolicy
  \[DeviceComplianceScriptId \<String\>\]: The unique identifier of deviceComplianceScript
  \[DeviceConfigurationId \<String\>\]: The unique identifier of deviceConfiguration
  \[DeviceCustomAttributeShellScriptId \<String\>\]: The unique identifier of deviceCustomAttributeShellScript
  \[DeviceEnrollmentConfigurationId \<String\>\]: The unique identifier of deviceEnrollmentConfiguration
  \[DeviceHealthScriptId \<String\>\]: The unique identifier of deviceHealthScript
  \[DeviceLogCollectionResponseId \<String\>\]: The unique identifier of deviceLogCollectionResponse
  \[DeviceManagementCompliancePolicyId \<String\>\]: The unique identifier of deviceManagementCompliancePolicy
  \[DeviceManagementConfigurationPolicyId \<String\>\]: The unique identifier of deviceManagementConfigurationPolicy
  \[DeviceManagementExchangeConnectorId \<String\>\]: The unique identifier of deviceManagementExchangeConnector
  \[DeviceManagementIntentId \<String\>\]: The unique identifier of deviceManagementIntent
  \[DeviceManagementPartnerId \<String\>\]: The unique identifier of deviceManagementPartner
  \[DeviceManagementResourceAccessProfileBaseId \<String\>\]: The unique identifier of deviceManagementResourceAccessProfileBase
  \[DeviceManagementReusablePolicySettingId \<String\>\]: The unique identifier of deviceManagementReusablePolicySetting
  \[DeviceManagementScriptId \<String\>\]: The unique identifier of deviceManagementScript
  \[DeviceManagementTemplateId \<String\>\]: The unique identifier of deviceManagementTemplate
  \[DeviceManagementTemplateId1 \<String\>\]: The unique identifier of deviceManagementTemplate
  \[DeviceShellScriptId \<String\>\]: The unique identifier of deviceShellScript
  \[EmbeddedSimActivationCodePoolId \<String\>\]: The unique identifier of embeddedSIMActivationCodePool
  \[EnrollmentProfileId \<String\>\]: The unique identifier of enrollmentProfile
  \[GroupPolicyConfigurationId \<String\>\]: The unique identifier of groupPolicyConfiguration
  \[GroupPolicyMigrationReportId \<String\>\]: The unique identifier of groupPolicyMigrationReport
  \[GroupPolicyUploadedDefinitionFileId \<String\>\]: The unique identifier of groupPolicyUploadedDefinitionFile
  \[IntuneBrandingProfileId \<String\>\]: The unique identifier of intuneBrandingProfile
  \[ManagedDeviceId \<String\>\]: The unique identifier of managedDevice
  \[MicrosoftTunnelServerId \<String\>\]: The unique identifier of microsoftTunnelServer
  \[MicrosoftTunnelServerLogCollectionResponseId \<String\>\]: The unique identifier of microsoftTunnelServerLogCollectionResponse
  \[MicrosoftTunnelSiteId \<String\>\]: The unique identifier of microsoftTunnelSite
  \[MobileAppTroubleshootingEventId \<String\>\]: The unique identifier of mobileAppTroubleshootingEvent
  \[NotificationMessageTemplateId \<String\>\]: The unique identifier of notificationMessageTemplate
  \[RemoteAssistancePartnerId \<String\>\]: The unique identifier of remoteAssistancePartner
  \[RoleScopeTagId \<String\>\]: The unique identifier of roleScopeTag
  \[WindowsAutopilotDeploymentProfileId \<String\>\]: The unique identifier of windowsAutopilotDeploymentProfile
  \[WindowsAutopilotDeviceIdentityId \<String\>\]: The unique identifier of windowsAutopilotDeviceIdentity
  \[WindowsDriverUpdateProfileId \<String\>\]: The unique identifier of windowsDriverUpdateProfile
  \[WindowsFeatureUpdateProfileId \<String\>\]: The unique identifier of windowsFeatureUpdateProfile
  \[WindowsQualityUpdateProfileId \<String\>\]: The unique identifier of windowsQualityUpdateProfile
  \[ZebraFotaDeploymentId \<String\>\]: The unique identifier of zebraFotaDeployment

REVIEWSTATUS \<IMicrosoftGraphCloudPcReviewStatus\>: cloudPcReviewStatus
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[AzureStorageAccountId \<String\>\]: The resource ID of the Azure Storage account in which the Cloud PC snapshot is being saved.
  \[AzureStorageAccountName \<String\>\]: The name of the Azure Storage account in which the Cloud PC snapshot is being saved.
  \[AzureStorageContainerName \<String\>\]: The name of the container in an Azure Storage account in which the Cloud PC snapshot is being saved.
  \[InReview \<Boolean?\>\]: True if the Cloud PC is set to in review by the administrator.
  \[RestorePointDateTime \<DateTime?\>\]: The specific date and time of the Cloud PC snapshot that was taken and saved automatically, when the Cloud PC is set to in review.
The timestamp is shown in ISO 8601 format and Coordinated Universal Time (UTC).
For example, midnight UTC on Jan 1, 2014 appears as 2014-01-01T00:00:00Z.
  \[ReviewStartDateTime \<DateTime?\>\]: The specific date and time when the Cloud PC was set to in review.
The timestamp is shown in ISO 8601 format and Coordinated Universal Time (UTC).
For example, midnight UTC on Jan 1, 2014 appears as 2014-01-01T00:00:00Z.
  \[SubscriptionId \<String\>\]: The ID of the Azure subscription in which the Cloud PC snapshot is being saved, in GUID format.
  \[SubscriptionName \<String\>\]: The name of the Azure subscription in which the Cloud PC snapshot is being saved.
  \[UserAccessLevel \<String\>\]: cloudPcUserAccessLevel

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.actions/set-mgbetadevicemanagementcomanageddevicecloudpcreviewstatus](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.actions/set-mgbetadevicemanagementcomanageddevicecloudpcreviewstatus)



