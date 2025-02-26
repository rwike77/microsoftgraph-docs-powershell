---
external help file: Microsoft.Graph.Beta.Groups-help.xml
Module Name: Microsoft.Graph.Beta.Groups
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.groups/grant-mgbetagroupdriverootpermission
schema: 2.0.0
ms.prod: sharepoint
---

# Grant-MgBetaGroupDriveRootPermission

## SYNOPSIS
Grant users access to a link represented by a permission\]\[\].
This API is available in the following \[national cloud deployments.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Grant-MgGroupDriveRootPermission](/powershell/module/Microsoft.Graph.Groups/Grant-MgGroupDriveRootPermission?view=graph-powershell-1.0)

## SYNTAX

### GrantExpanded (Default)
```
Grant-MgBetaGroupDriveRootPermission -DriveId <String> -GroupId <String> -PermissionId <String>
 [-AdditionalProperties <Hashtable>] [-Recipients <IMicrosoftGraphDriveRecipient[]>] [-Roles <String[]>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Grant
```
Grant-MgBetaGroupDriveRootPermission -DriveId <String> -GroupId <String> -PermissionId <String>
 -BodyParameter <IPathsG3D749GroupsGroupIdDrivesDriveIdRootPermissionsPermissionIdMicrosoftGraphGrantPostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### GrantViaIdentityExpanded
```
Grant-MgBetaGroupDriveRootPermission -InputObject <IGroupsIdentity> [-AdditionalProperties <Hashtable>]
 [-Recipients <IMicrosoftGraphDriveRecipient[]>] [-Roles <String[]>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### GrantViaIdentity
```
Grant-MgBetaGroupDriveRootPermission -InputObject <IGroupsIdentity>
 -BodyParameter <IPathsG3D749GroupsGroupIdDrivesDriveIdRootPermissionsPermissionIdMicrosoftGraphGrantPostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Grant users access to a link represented by a permission\]\[\].
This API is available in the following \[national cloud deployments.

## EXAMPLES
### Example 1: Code snippet

```powershell
Import-Module Microsoft.Graph.Beta.Files

$params = @{
	Recipients = @(
		@{
			Email = "john@contoso.com"
		}
		@{
			Email = "ryan@external.com"
		}
	)
	Roles = @(
		"read"
	)
}

Grant-MgBetaSharePermission -SharedDriveItemId $sharedDriveItemId -BodyParameter $params
```
This example shows how to use the Grant-MgBetaGroupDriveRootPermission Cmdlet.

To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: GrantExpanded, GrantViaIdentityExpanded
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
Type: IPathsG3D749GroupsGroupIdDrivesDriveIdRootPermissionsPermissionIdMicrosoftGraphGrantPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Grant, GrantViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DriveId
The unique identifier of drive

```yaml
Type: String
Parameter Sets: GrantExpanded, Grant
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GroupId
The unique identifier of group

```yaml
Type: String
Parameter Sets: GrantExpanded, Grant
Aliases:

Required: True
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
Parameter Sets: GrantViaIdentityExpanded, GrantViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PermissionId
The unique identifier of permission

```yaml
Type: String
Parameter Sets: GrantExpanded, Grant
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Recipients
.
To construct, see NOTES section for RECIPIENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphDriveRecipient[]
Parameter Sets: GrantExpanded, GrantViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Roles
.

```yaml
Type: String[]
Parameter Sets: GrantExpanded, GrantViaIdentityExpanded
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
### Microsoft.Graph.Beta.PowerShell.Models.IPathsG3D749GroupsGroupIdDrivesDriveIdRootPermissionsPermissionIdMicrosoftGraphGrantPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphPermission
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IPathsG3D749GroupsGroupIdDrivesDriveIdRootPermissionsPermissionIdMicrosoftGraphGrantPostRequestbodyContentApplicationJsonSchema\>: .
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Recipients \<IMicrosoftGraphDriveRecipient\[\]\>\]: 
    \[Alias \<String\>\]: The alias of the domain object, for cases where an email address is unavailable (e.g.
security groups).
    \[Email \<String\>\]: The email address for the recipient, if the recipient has an associated email address.
    \[ObjectId \<String\>\]: The unique identifier for the recipient in the directory.
  \[Roles \<String\[\]\>\]: 

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

RECIPIENTS \<IMicrosoftGraphDriveRecipient\[\]\>: .
  \[Alias \<String\>\]: The alias of the domain object, for cases where an email address is unavailable (e.g.
security groups).
  \[Email \<String\>\]: The email address for the recipient, if the recipient has an associated email address.
  \[ObjectId \<String\>\]: The unique identifier for the recipient in the directory.

## RELATED LINKS
[Grant-MgGroupDriveRootPermission](/powershell/module/Microsoft.Graph.Groups/Grant-MgGroupDriveRootPermission?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.groups/grant-mgbetagroupdriverootpermission](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.groups/grant-mgbetagroupdriverootpermission)

