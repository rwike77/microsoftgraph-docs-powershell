---
external help file: Microsoft.Graph.DeviceManagement-help.xml
Module Name: Microsoft.Graph.DeviceManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement/update-mgdevicemanagementuserexperienceanalyticapphealthdevicemodelperformance
schema: 2.0.0
---

# Update-MgDeviceManagementUserExperienceAnalyticAppHealthDeviceModelPerformance

## SYNOPSIS
Update the navigation property userExperienceAnalyticsAppHealthDeviceModelPerformance in deviceManagement

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaDeviceManagementUserExperienceAnalyticAppHealthDeviceModelPerformance](/powershell/module/Microsoft.Graph.Beta.DeviceManagement/Update-MgBetaDeviceManagementUserExperienceAnalyticAppHealthDeviceModelPerformance?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgDeviceManagementUserExperienceAnalyticAppHealthDeviceModelPerformance
 -UserExperienceAnalyticsAppHealthDeviceModelPerformanceId <String> [-ActiveDeviceCount <Int32>]
 [-AdditionalProperties <Hashtable>] [-DeviceManufacturer <String>] [-DeviceModel <String>]
 [-HealthStatus <UserExperienceAnalyticsHealthState>] [-Id <String>] [-MeanTimeToFailureInMinutes <Int32>]
 [-ModelAppHealthScore <Double>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgDeviceManagementUserExperienceAnalyticAppHealthDeviceModelPerformance
 -UserExperienceAnalyticsAppHealthDeviceModelPerformanceId <String>
 -BodyParameter <IMicrosoftGraphUserExperienceAnalyticsAppHealthDeviceModelPerformance> [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgDeviceManagementUserExperienceAnalyticAppHealthDeviceModelPerformance
 -InputObject <IDeviceManagementIdentity> [-ActiveDeviceCount <Int32>] [-AdditionalProperties <Hashtable>]
 [-DeviceManufacturer <String>] [-DeviceModel <String>] [-HealthStatus <UserExperienceAnalyticsHealthState>]
 [-Id <String>] [-MeanTimeToFailureInMinutes <Int32>] [-ModelAppHealthScore <Double>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgDeviceManagementUserExperienceAnalyticAppHealthDeviceModelPerformance
 -InputObject <IDeviceManagementIdentity>
 -BodyParameter <IMicrosoftGraphUserExperienceAnalyticsAppHealthDeviceModelPerformance> [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property userExperienceAnalyticsAppHealthDeviceModelPerformance in deviceManagement

## PARAMETERS

### -ActiveDeviceCount
The number of active devices for the model.
Valid values 0 to 2147483647.
Supports: $filter, $select, $OrderBy.
Read-only.
Valid values -2147483648 to 2147483647

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
The user experience analytics device model performance entity contains device model performance details.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphUserExperienceAnalyticsAppHealthDeviceModelPerformance
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DeviceManufacturer
The manufacturer name of the device.
Supports: $select, $OrderBy.
Read-only.

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceModel
The model name of the device.
Supports: $select, $OrderBy.
Read-only.

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HealthStatus
userExperienceAnalyticsHealthState

```yaml
Type: UserExperienceAnalyticsHealthState
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Type: IDeviceManagementIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -MeanTimeToFailureInMinutes
The mean time to failure for the application in minutes.
Valid values 0 to 2147483647.
Supports: $filter, $select, $OrderBy.
Read-only.
Valid values -2147483648 to 2147483647

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -ModelAppHealthScore
The application health score of the device model.
Valid values 0 to 100.
Supports: $filter, $select, $OrderBy.
Read-only.
Valid values -1.79769313486232E+308 to 1.79769313486232E+308

```yaml
Type: Double
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserExperienceAnalyticsAppHealthDeviceModelPerformanceId
The unique identifier of userExperienceAnalyticsAppHealthDeviceModelPerformance

```yaml
Type: String
Parameter Sets: UpdateExpanded, Update
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

### Microsoft.Graph.PowerShell.Models.IDeviceManagementIdentity
### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphUserExperienceAnalyticsAppHealthDeviceModelPerformance
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphUserExperienceAnalyticsAppHealthDeviceModelPerformance
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphUserExperienceAnalyticsAppHealthDeviceModelPerformance\>: The user experience analytics device model performance entity contains device model performance details.
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[ActiveDeviceCount \<Int32?\>\]: The number of active devices for the model.
Valid values 0 to 2147483647.
Supports: $filter, $select, $OrderBy.
Read-only.
Valid values -2147483648 to 2147483647
  \[DeviceManufacturer \<String\>\]: The manufacturer name of the device.
Supports: $select, $OrderBy.
Read-only.
  \[DeviceModel \<String\>\]: The model name of the device.
Supports: $select, $OrderBy.
Read-only.
  \[HealthStatus \<UserExperienceAnalyticsHealthState?\>\]: userExperienceAnalyticsHealthState
  \[MeanTimeToFailureInMinutes \<Int32?\>\]: The mean time to failure for the application in minutes.
Valid values 0 to 2147483647.
Supports: $filter, $select, $OrderBy.
Read-only.
Valid values -2147483648 to 2147483647
  \[ModelAppHealthScore \<Double?\>\]: The application health score of the device model.
Valid values 0 to 100.
Supports: $filter, $select, $OrderBy.
Read-only.
Valid values -1.79769313486232E+308 to 1.79769313486232E+308

INPUTOBJECT \<IDeviceManagementIdentity\>: Identity Parameter
  \[AppLogCollectionRequestId \<String\>\]: The unique identifier of appLogCollectionRequest
  \[BrowserSharedCookieId \<String\>\]: The unique identifier of browserSharedCookie
  \[BrowserSiteId \<String\>\]: The unique identifier of browserSite
  \[BrowserSiteListId \<String\>\]: The unique identifier of browserSiteList
  \[DetectedAppId \<String\>\]: The unique identifier of detectedApp
  \[DeviceCategoryId \<String\>\]: The unique identifier of deviceCategory
  \[DeviceComplianceActionItemId \<String\>\]: The unique identifier of deviceComplianceActionItem
  \[DeviceComplianceDeviceStatusId \<String\>\]: The unique identifier of deviceComplianceDeviceStatus
  \[DeviceCompliancePolicyAssignmentId \<String\>\]: The unique identifier of deviceCompliancePolicyAssignment
  \[DeviceCompliancePolicyId \<String\>\]: The unique identifier of deviceCompliancePolicy
  \[DeviceCompliancePolicySettingStateSummaryId \<String\>\]: The unique identifier of deviceCompliancePolicySettingStateSummary
  \[DeviceCompliancePolicyStateId \<String\>\]: The unique identifier of deviceCompliancePolicyState
  \[DeviceComplianceScheduledActionForRuleId \<String\>\]: The unique identifier of deviceComplianceScheduledActionForRule
  \[DeviceComplianceSettingStateId \<String\>\]: The unique identifier of deviceComplianceSettingState
  \[DeviceComplianceUserStatusId \<String\>\]: The unique identifier of deviceComplianceUserStatus
  \[DeviceConfigurationAssignmentId \<String\>\]: The unique identifier of deviceConfigurationAssignment
  \[DeviceConfigurationDeviceStatusId \<String\>\]: The unique identifier of deviceConfigurationDeviceStatus
  \[DeviceConfigurationId \<String\>\]: The unique identifier of deviceConfiguration
  \[DeviceConfigurationStateId \<String\>\]: The unique identifier of deviceConfigurationState
  \[DeviceConfigurationUserStatusId \<String\>\]: The unique identifier of deviceConfigurationUserStatus
  \[DeviceLogCollectionResponseId \<String\>\]: The unique identifier of deviceLogCollectionResponse
  \[DeviceManagementTroubleshootingEventId \<String\>\]: The unique identifier of deviceManagementTroubleshootingEvent
  \[LocalizedNotificationMessageId \<String\>\]: The unique identifier of localizedNotificationMessage
  \[MalwareStateForWindowsDeviceId \<String\>\]: The unique identifier of malwareStateForWindowsDevice
  \[ManagedDeviceId \<String\>\]: The unique identifier of managedDevice
  \[MobileAppTroubleshootingEventId \<String\>\]: The unique identifier of mobileAppTroubleshootingEvent
  \[NotificationMessageTemplateId \<String\>\]: The unique identifier of notificationMessageTemplate
  \[SettingStateDeviceSummaryId \<String\>\]: The unique identifier of settingStateDeviceSummary
  \[UserExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetailsId \<String\>\]: The unique identifier of userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails
  \[UserExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId \<String\>\]: The unique identifier of userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId
  \[UserExperienceAnalyticsAppHealthAppPerformanceByOSVersionId \<String\>\]: The unique identifier of userExperienceAnalyticsAppHealthAppPerformanceByOSVersion
  \[UserExperienceAnalyticsAppHealthApplicationPerformanceId \<String\>\]: The unique identifier of userExperienceAnalyticsAppHealthApplicationPerformance
  \[UserExperienceAnalyticsAppHealthDeviceModelPerformanceId \<String\>\]: The unique identifier of userExperienceAnalyticsAppHealthDeviceModelPerformance
  \[UserExperienceAnalyticsAppHealthDevicePerformanceDetailsId \<String\>\]: The unique identifier of userExperienceAnalyticsAppHealthDevicePerformanceDetails
  \[UserExperienceAnalyticsAppHealthDevicePerformanceId \<String\>\]: The unique identifier of userExperienceAnalyticsAppHealthDevicePerformance
  \[UserExperienceAnalyticsAppHealthOSVersionPerformanceId \<String\>\]: The unique identifier of userExperienceAnalyticsAppHealthOSVersionPerformance
  \[UserExperienceAnalyticsBaselineId \<String\>\]: The unique identifier of userExperienceAnalyticsBaseline
  \[UserExperienceAnalyticsCategoryId \<String\>\]: The unique identifier of userExperienceAnalyticsCategory
  \[UserExperienceAnalyticsDevicePerformanceId \<String\>\]: The unique identifier of userExperienceAnalyticsDevicePerformance
  \[UserExperienceAnalyticsDeviceScoresId \<String\>\]: The unique identifier of userExperienceAnalyticsDeviceScores
  \[UserExperienceAnalyticsDeviceStartupHistoryId \<String\>\]: The unique identifier of userExperienceAnalyticsDeviceStartupHistory
  \[UserExperienceAnalyticsDeviceStartupProcessId \<String\>\]: The unique identifier of userExperienceAnalyticsDeviceStartupProcess
  \[UserExperienceAnalyticsDeviceStartupProcessPerformanceId \<String\>\]: The unique identifier of userExperienceAnalyticsDeviceStartupProcessPerformance
  \[UserExperienceAnalyticsMetricHistoryId \<String\>\]: The unique identifier of userExperienceAnalyticsMetricHistory
  \[UserExperienceAnalyticsMetricId \<String\>\]: The unique identifier of userExperienceAnalyticsMetric
  \[UserExperienceAnalyticsModelScoresId \<String\>\]: The unique identifier of userExperienceAnalyticsModelScores
  \[UserExperienceAnalyticsScoreHistoryId \<String\>\]: The unique identifier of userExperienceAnalyticsScoreHistory
  \[UserExperienceAnalyticsWorkFromAnywhereDeviceId \<String\>\]: The unique identifier of userExperienceAnalyticsWorkFromAnywhereDevice
  \[UserExperienceAnalyticsWorkFromAnywhereMetricId \<String\>\]: The unique identifier of userExperienceAnalyticsWorkFromAnywhereMetric
  \[UserExperienceAnalyticsWorkFromAnywhereModelPerformanceId \<String\>\]: The unique identifier of userExperienceAnalyticsWorkFromAnywhereModelPerformance
  \[WindowsDeviceMalwareStateId \<String\>\]: The unique identifier of windowsDeviceMalwareState
  \[WindowsInformationProtectionAppLearningSummaryId \<String\>\]: The unique identifier of windowsInformationProtectionAppLearningSummary
  \[WindowsInformationProtectionNetworkLearningSummaryId \<String\>\]: The unique identifier of windowsInformationProtectionNetworkLearningSummary
  \[WindowsMalwareInformationId \<String\>\]: The unique identifier of windowsMalwareInformation

## RELATED LINKS
[Update-MgBetaDeviceManagementUserExperienceAnalyticAppHealthDeviceModelPerformance](/powershell/module/Microsoft.Graph.Beta.DeviceManagement/Update-MgBetaDeviceManagementUserExperienceAnalyticAppHealthDeviceModelPerformance?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement/update-mgdevicemanagementuserexperienceanalyticapphealthdevicemodelperformance](https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement/update-mgdevicemanagementuserexperienceanalyticapphealthdevicemodelperformance)



