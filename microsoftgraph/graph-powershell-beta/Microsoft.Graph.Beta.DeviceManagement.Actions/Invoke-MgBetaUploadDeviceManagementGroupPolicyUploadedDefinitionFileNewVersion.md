---
external help file: Microsoft.Graph.Beta.DeviceManagement.Actions-help.xml
Module Name: Microsoft.Graph.Beta.DeviceManagement.Actions
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.actions/invoke-mgbetauploaddevicemanagementgrouppolicyuploadeddefinitionfilenewversion
schema: 2.0.0
---

# Invoke-MgBetaUploadDeviceManagementGroupPolicyUploadedDefinitionFileNewVersion

## SYNOPSIS
Invoke action uploadNewVersion

## SYNTAX

### UploadExpanded (Default)
```
Invoke-MgBetaUploadDeviceManagementGroupPolicyUploadedDefinitionFileNewVersion
 -GroupPolicyUploadedDefinitionFileId <String> [-AdditionalProperties <Hashtable>] [-ContentInputFile <String>]
 [-GroupPolicyUploadedLanguageFiles <IMicrosoftGraphGroupPolicyUploadedLanguageFile[]>] [-PassThru] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Upload
```
Invoke-MgBetaUploadDeviceManagementGroupPolicyUploadedDefinitionFileNewVersion
 -GroupPolicyUploadedDefinitionFileId <String>
 -BodyParameter <IPathsQaczrkDevicemanagementGrouppolicyuploadeddefinitionfilesGrouppolicyuploadeddefinitionfileIdMicrosoftGraphUploadnewversionPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UploadViaIdentityExpanded
```
Invoke-MgBetaUploadDeviceManagementGroupPolicyUploadedDefinitionFileNewVersion
 -InputObject <IDeviceManagementActionsIdentity> [-AdditionalProperties <Hashtable>]
 [-ContentInputFile <String>]
 [-GroupPolicyUploadedLanguageFiles <IMicrosoftGraphGroupPolicyUploadedLanguageFile[]>] [-PassThru] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UploadViaIdentity
```
Invoke-MgBetaUploadDeviceManagementGroupPolicyUploadedDefinitionFileNewVersion
 -InputObject <IDeviceManagementActionsIdentity>
 -BodyParameter <IPathsQaczrkDevicemanagementGrouppolicyuploadeddefinitionfilesGrouppolicyuploadeddefinitionfileIdMicrosoftGraphUploadnewversionPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Invoke action uploadNewVersion

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UploadExpanded, UploadViaIdentityExpanded
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
Type: IPathsQaczrkDevicemanagementGrouppolicyuploadeddefinitionfilesGrouppolicyuploadeddefinitionfileIdMicrosoftGraphUploadnewversionPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Upload, UploadViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ContentInputFile
Input File for Content (.)

```yaml
Type: String
Parameter Sets: UploadExpanded, UploadViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GroupPolicyUploadedDefinitionFileId
The unique identifier of groupPolicyUploadedDefinitionFile

```yaml
Type: String
Parameter Sets: UploadExpanded, Upload
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GroupPolicyUploadedLanguageFiles
.
To construct, see NOTES section for GROUPPOLICYUPLOADEDLANGUAGEFILES properties and create a hash table.

```yaml
Type: IMicrosoftGraphGroupPolicyUploadedLanguageFile[]
Parameter Sets: UploadExpanded, UploadViaIdentityExpanded
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
Type: IDeviceManagementActionsIdentity
Parameter Sets: UploadViaIdentityExpanded, UploadViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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

### Microsoft.Graph.Beta.PowerShell.Models.IDeviceManagementActionsIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IPathsQaczrkDevicemanagementGrouppolicyuploadeddefinitionfilesGrouppolicyuploadeddefinitionfileIdMicrosoftGraphUploadnewversionPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IPathsQaczrkDevicemanagementGrouppolicyuploadeddefinitionfilesGrouppolicyuploadeddefinitionfileIdMicrosoftGraphUploadnewversionPostRequestbodyContentApplicationJsonSchema\>: .
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Content \<Byte\[\]\>\]: 
  \[GroupPolicyUploadedLanguageFiles \<IMicrosoftGraphGroupPolicyUploadedLanguageFile\[\]\>\]: 
    \[Content \<Byte\[\]\>\]: The contents of the uploaded ADML file.
    \[FileName \<String\>\]: The file name of the uploaded ADML file.
    \[Id \<String\>\]: Key of the entity.
    \[LanguageCode \<String\>\]: The language code of the uploaded ADML file.
    \[LastModifiedDateTime \<DateTime?\>\]: The date and time the entity was last modified.

GROUPPOLICYUPLOADEDLANGUAGEFILES \<IMicrosoftGraphGroupPolicyUploadedLanguageFile\[\]\>: .
  \[Content \<Byte\[\]\>\]: The contents of the uploaded ADML file.
  \[FileName \<String\>\]: The file name of the uploaded ADML file.
  \[Id \<String\>\]: Key of the entity.
  \[LanguageCode \<String\>\]: The language code of the uploaded ADML file.
  \[LastModifiedDateTime \<DateTime?\>\]: The date and time the entity was last modified.

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

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.actions/invoke-mgbetauploaddevicemanagementgrouppolicyuploadeddefinitionfilenewversion](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.actions/invoke-mgbetauploaddevicemanagementgrouppolicyuploadeddefinitionfilenewversion)


