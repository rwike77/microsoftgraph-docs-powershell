---
external help file: Microsoft.Graph.Beta.Groups-help.xml
Module Name: Microsoft.Graph.Beta.Groups
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.groups/new-mgbetagroupsetting
schema: 2.0.0
---

# New-MgBetaGroupSetting

## SYNOPSIS
Create a new setting based on the templates available in directorySettingTemplates.
These settings can be at the tenant-level or at the group level.
Group settings apply to only Microsoft 365 groups.
The template named Group.Unified can be used to configure tenant-wide Microsoft 365 group settings, while the template named Group.Unified.Guest can be used to configure group-specific settings.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgGroupSetting](/powershell/module/Microsoft.Graph.Groups/New-MgGroupSetting?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaGroupSetting -GroupId <String> [-AdditionalProperties <Hashtable>] [-DisplayName <String>]
 [-Id <String>] [-TemplateId <String>] [-Values <IMicrosoftGraphSettingValue[]>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Create
```
New-MgBetaGroupSetting -GroupId <String> -BodyParameter <IMicrosoftGraphDirectorySetting> [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgBetaGroupSetting -InputObject <IGroupsIdentity> [-AdditionalProperties <Hashtable>]
 [-DisplayName <String>] [-Id <String>] [-TemplateId <String>] [-Values <IMicrosoftGraphSettingValue[]>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgBetaGroupSetting -InputObject <IGroupsIdentity> -BodyParameter <IMicrosoftGraphDirectorySetting>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new setting based on the templates available in directorySettingTemplates.
These settings can be at the tenant-level or at the group level.
Group settings apply to only Microsoft 365 groups.
The template named Group.Unified can be used to configure tenant-wide Microsoft 365 group settings, while the template named Group.Unified.Guest can be used to configure group-specific settings.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Create a setting to block guests for a specific Microsoft 365 group

```powershell
Import-Module Microsoft.Graph.Beta.Groups

$params = @{
	templateId = "08d542b9-071f-4e16-94b0-74abb372e3d9"
	values = @(
		@{
			name = "AllowToAddGuests"
			value = "false"
		}
	)
}

New-MgBetaGroupSetting -GroupId $groupId -BodyParameter $params
```
This example shows how to use the New-MgBetaGroupSetting Cmdlet.

To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).


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
directorySetting
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphDirectorySetting
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DisplayName
Display name of this group of settings, which comes from the associated template.
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

### -GroupId
The unique identifier of group

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
Type: IGroupsIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -TemplateId
Unique identifier for the template used to create this group of settings.
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

### -Values
Collection of name-value pairs corresponding to the name and defaultValue properties in the referenced directorySettingTemplates object.
To construct, see NOTES section for VALUES properties and create a hash table.

```yaml
Type: IMicrosoftGraphSettingValue[]
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

### Microsoft.Graph.Beta.PowerShell.Models.IGroupsIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphDirectorySetting
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphDirectorySetting
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphDirectorySetting\>: directorySetting
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[DisplayName \<String\>\]: Display name of this group of settings, which comes from the associated template.
Read-only.
  \[TemplateId \<String\>\]: Unique identifier for the template used to create this group of settings.
Read-only.
  \[Values \<IMicrosoftGraphSettingValue\[\]\>\]: Collection of name-value pairs corresponding to the name and defaultValue properties in the referenced directorySettingTemplates object.
    \[Name \<String\>\]: Name of the setting (as defined by the directorySettingTemplate).
    \[Value \<String\>\]: Value of the setting.

INPUTOBJECT \<IGroupsIdentity\>: Identity Parameter
  \[AttachmentId \<String\>\]: The unique identifier of attachment
  \[ContentTypeId \<String\>\]: The unique identifier of contentType
  \[ConversationId \<String\>\]: The unique identifier of conversation
  \[ConversationThreadId \<String\>\]: The unique identifier of conversationThread
  \[DirectoryObjectId \<String\>\]: The unique identifier of directoryObject
  \[DirectorySettingId \<String\>\]: The unique identifier of directorySetting
  \[DocumentSetVersionId \<String\>\]: The unique identifier of documentSetVersion
  \[DriveId \<String\>\]: The unique identifier of drive
  \[DriveItemId \<String\>\]: The unique identifier of driveItem
  \[DriveItemVersionId \<String\>\]: The unique identifier of driveItemVersion
  \[EndDateTime \<String\>\]: Usage: endDateTime='{endDateTime}'
  \[EndpointId \<String\>\]: The unique identifier of endpoint
  \[EventId \<String\>\]: The unique identifier of event
  \[ExtensionId \<String\>\]: The unique identifier of extension
  \[GroupId \<String\>\]: The unique identifier of group
  \[GroupLifecyclePolicyId \<String\>\]: The unique identifier of groupLifecyclePolicy
  \[IncludePersonalNotebooks \<Boolean?\>\]: Usage: includePersonalNotebooks={includePersonalNotebooks}
  \[Interval \<String\>\]: Usage: interval='{interval}'
  \[ListId \<String\>\]: The unique identifier of list
  \[ListItemId \<String\>\]: The unique identifier of listItem
  \[ListItemVersionId \<String\>\]: The unique identifier of listItemVersion
  \[MentionId \<String\>\]: The unique identifier of mention
  \[NotebookId \<String\>\]: The unique identifier of notebook
  \[OnenotePageId \<String\>\]: The unique identifier of onenotePage
  \[OnenoteSectionId \<String\>\]: The unique identifier of onenoteSection
  \[Path \<String\>\]: Usage: path='{path}'
  \[PermissionId \<String\>\]: The unique identifier of permission
  \[PlannerBucketId \<String\>\]: The unique identifier of plannerBucket
  \[PlannerPlanId \<String\>\]: The unique identifier of plannerPlan
  \[PostId \<String\>\]: The unique identifier of post
  \[ProfilePhotoId \<String\>\]: The unique identifier of profilePhoto
  \[Q \<String\>\]: Usage: q='{q}'
  \[ResourceSpecificPermissionGrantId \<String\>\]: The unique identifier of resourceSpecificPermissionGrant
  \[SensitivityLabelId \<String\>\]: The unique identifier of sensitivityLabel
  \[SiteId \<String\>\]: The unique identifier of site
  \[StartDateTime \<String\>\]: Usage: startDateTime='{startDateTime}'
  \[SubscriptionId \<String\>\]: The unique identifier of subscription
  \[Token \<String\>\]: Usage: token='{token}'
  \[UniqueName \<String\>\]: Alternate key of group
  \[User \<String\>\]: Usage: User='{User}'
  \[UserId \<String\>\]: The unique identifier of user

VALUES \<IMicrosoftGraphSettingValue\[\]\>: Collection of name-value pairs corresponding to the name and defaultValue properties in the referenced directorySettingTemplates object.
  \[Name \<String\>\]: Name of the setting (as defined by the directorySettingTemplate).
  \[Value \<String\>\]: Value of the setting.

## RELATED LINKS
[New-MgGroupSetting](/powershell/module/Microsoft.Graph.Groups/New-MgGroupSetting?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.groups/new-mgbetagroupsetting](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.groups/new-mgbetagroupsetting)

