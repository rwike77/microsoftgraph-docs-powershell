---
external help file: Microsoft.Graph.Devices.ServiceAnnouncement-help.xml
Module Name: Microsoft.Graph.Devices.ServiceAnnouncement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.devices.serviceannouncement/new-mgserviceannouncementhealthoverviewissue
schema: 2.0.0
---

# New-MgServiceAnnouncementHealthOverviewIssue

## SYNOPSIS
Create new navigation property to issues for admin

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaServiceAnnouncementHealthOverviewIssue](/powershell/module/Microsoft.Graph.Beta.Devices.ServiceAnnouncement/New-MgBetaServiceAnnouncementHealthOverviewIssue?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgServiceAnnouncementHealthOverviewIssue -ServiceHealthId <String> [-AdditionalProperties <Hashtable>]
 [-Classification <String>] [-Details <IMicrosoftGraphKeyValuePair[]>] [-EndDateTime <DateTime>]
 [-Feature <String>] [-FeatureGroup <String>] [-Id <String>] [-ImpactDescription <String>] [-IsResolved]
 [-LastModifiedDateTime <DateTime>] [-Origin <String>] [-Posts <IMicrosoftGraphServiceHealthIssuePost[]>]
 [-Service <String>] [-StartDateTime <DateTime>] [-Status <String>] [-Title <String>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Create
```
New-MgServiceAnnouncementHealthOverviewIssue -ServiceHealthId <String>
 -BodyParameter <IMicrosoftGraphServiceHealthIssue> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgServiceAnnouncementHealthOverviewIssue -InputObject <IDevicesServiceAnnouncementIdentity>
 [-AdditionalProperties <Hashtable>] [-Classification <String>] [-Details <IMicrosoftGraphKeyValuePair[]>]
 [-EndDateTime <DateTime>] [-Feature <String>] [-FeatureGroup <String>] [-Id <String>]
 [-ImpactDescription <String>] [-IsResolved] [-LastModifiedDateTime <DateTime>] [-Origin <String>]
 [-Posts <IMicrosoftGraphServiceHealthIssuePost[]>] [-Service <String>] [-StartDateTime <DateTime>]
 [-Status <String>] [-Title <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgServiceAnnouncementHealthOverviewIssue -InputObject <IDevicesServiceAnnouncementIdentity>
 -BodyParameter <IMicrosoftGraphServiceHealthIssue> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to issues for admin

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
serviceHealthIssue
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphServiceHealthIssue
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Classification
serviceHealthClassificationType

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

### -Details
More details about service event.
This property doesn't support filters.
To construct, see NOTES section for DETAILS properties and create a hash table.

```yaml
Type: IMicrosoftGraphKeyValuePair[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EndDateTime
The end time of the service event.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Feature
The feature name of the service issue.

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

### -FeatureGroup
The feature group name of the service issue.

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

### -ImpactDescription
The description of the service issue impact.

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
Type: IDevicesServiceAnnouncementIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IsResolved
Indicates whether the issue is resolved.

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastModifiedDateTime
The last modified time of the service event.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Origin
serviceHealthOrigin

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

### -Posts
Collection of historical posts for the service issue.
To construct, see NOTES section for POSTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphServiceHealthIssuePost[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Service
Indicates the service affected by the issue.

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

### -ServiceHealthId
The unique identifier of serviceHealth

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

### -StartDateTime
The start time of the service event.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Status
serviceHealthStatus

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

### -Title
The title of the service event.

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

### Microsoft.Graph.PowerShell.Models.IDevicesServiceAnnouncementIdentity
### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphServiceHealthIssue
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphServiceHealthIssue
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphServiceHealthIssue\>: serviceHealthIssue
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Details \<IMicrosoftGraphKeyValuePair\[\]\>\]: More details about service event.
This property doesn't support filters.
    \[Name \<String\>\]: Name for this key-value pair
    \[Value \<String\>\]: Value for this key-value pair
  \[EndDateTime \<DateTime?\>\]: The end time of the service event.
  \[LastModifiedDateTime \<DateTime?\>\]: The last modified time of the service event.
  \[StartDateTime \<DateTime?\>\]: The start time of the service event.
  \[Title \<String\>\]: The title of the service event.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[Classification \<String\>\]: serviceHealthClassificationType
  \[Feature \<String\>\]: The feature name of the service issue.
  \[FeatureGroup \<String\>\]: The feature group name of the service issue.
  \[ImpactDescription \<String\>\]: The description of the service issue impact.
  \[IsResolved \<Boolean?\>\]: Indicates whether the issue is resolved.
  \[Origin \<String\>\]: serviceHealthOrigin
  \[Posts \<IMicrosoftGraphServiceHealthIssuePost\[\]\>\]: Collection of historical posts for the service issue.
    \[CreatedDateTime \<DateTime?\>\]: The published time of the post.
    \[Description \<IMicrosoftGraphItemBody\>\]: itemBody
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Content \<String\>\]: The content of the item.
      \[ContentType \<String\>\]: bodyType
    \[PostType \<String\>\]: postType
  \[Service \<String\>\]: Indicates the service affected by the issue.
  \[Status \<String\>\]: serviceHealthStatus

DETAILS \<IMicrosoftGraphKeyValuePair\[\]\>: More details about service event.
This property doesn't support filters.
  \[Name \<String\>\]: Name for this key-value pair
  \[Value \<String\>\]: Value for this key-value pair

INPUTOBJECT \<IDevicesServiceAnnouncementIdentity\>: Identity Parameter
  \[ServiceAnnouncementAttachmentId \<String\>\]: The unique identifier of serviceAnnouncementAttachment
  \[ServiceHealthId \<String\>\]: The unique identifier of serviceHealth
  \[ServiceHealthIssueId \<String\>\]: The unique identifier of serviceHealthIssue
  \[ServiceUpdateMessageId \<String\>\]: The unique identifier of serviceUpdateMessage

POSTS \<IMicrosoftGraphServiceHealthIssuePost\[\]\>: Collection of historical posts for the service issue.
  \[CreatedDateTime \<DateTime?\>\]: The published time of the post.
  \[Description \<IMicrosoftGraphItemBody\>\]: itemBody
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Content \<String\>\]: The content of the item.
    \[ContentType \<String\>\]: bodyType
  \[PostType \<String\>\]: postType

## RELATED LINKS
[New-MgBetaServiceAnnouncementHealthOverviewIssue](/powershell/module/Microsoft.Graph.Beta.Devices.ServiceAnnouncement/New-MgBetaServiceAnnouncementHealthOverviewIssue?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.devices.serviceannouncement/new-mgserviceannouncementhealthoverviewissue](https://learn.microsoft.com/powershell/module/microsoft.graph.devices.serviceannouncement/new-mgserviceannouncementhealthoverviewissue)


