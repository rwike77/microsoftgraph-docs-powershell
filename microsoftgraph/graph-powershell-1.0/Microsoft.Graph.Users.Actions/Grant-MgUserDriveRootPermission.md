---
external help file: Microsoft.Graph.Users.Actions-help.xml
Module Name: Microsoft.Graph.Users.Actions
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.users.actions/grant-mguserdriverootpermission
schema: 2.0.0
ms.prod: sharepoint
---

# Grant-MgUserDriveRootPermission

## SYNOPSIS
Grant users access to a link represented by a permission\]\[\].
This API is available in the following \[national cloud deployments.

> [!NOTE]
> To view the beta release of this cmdlet, view [Grant-MgBetaUserDriveRootPermission](/powershell/module/Microsoft.Graph.Beta.Users.Actions/Grant-MgBetaUserDriveRootPermission?view=graph-powershell-beta)

## SYNTAX

### GrantExpanded (Default)
```
Grant-MgUserDriveRootPermission -DriveId <String> -PermissionId <String> -UserId <String>
 [-AdditionalProperties <Hashtable>] [-Recipients <IMicrosoftGraphDriveRecipient[]>] [-Roles <String[]>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Grant
```
Grant-MgUserDriveRootPermission -DriveId <String> -PermissionId <String> -UserId <String>
 -BodyParameter <IPathsQisc3SUsersUserIdDrivesDriveIdRootPermissionsPermissionIdMicrosoftGraphGrantPostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### GrantViaIdentityExpanded
```
Grant-MgUserDriveRootPermission -InputObject <IUsersActionsIdentity> [-AdditionalProperties <Hashtable>]
 [-Recipients <IMicrosoftGraphDriveRecipient[]>] [-Roles <String[]>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### GrantViaIdentity
```
Grant-MgUserDriveRootPermission -InputObject <IUsersActionsIdentity>
 -BodyParameter <IPathsQisc3SUsersUserIdDrivesDriveIdRootPermissionsPermissionIdMicrosoftGraphGrantPostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Grant users access to a link represented by a permission\]\[\].
This API is available in the following \[national cloud deployments.

## EXAMPLES
### Example 1: Code snippet

```powershell
Import-Module Microsoft.Graph.Files

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

Grant-MgSharePermission -SharedDriveItemId $sharedDriveItemId -BodyParameter $params
```
This example shows how to use the Grant-MgUserDriveRootPermission Cmdlet.

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
Type: IPathsQisc3SUsersUserIdDrivesDriveIdRootPermissionsPermissionIdMicrosoftGraphGrantPostRequestbodyContentApplicationJsonSchema
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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IUsersActionsIdentity
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

### -UserId
The unique identifier of user

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

### Microsoft.Graph.PowerShell.Models.IPathsQisc3SUsersUserIdDrivesDriveIdRootPermissionsPermissionIdMicrosoftGraphGrantPostRequestbodyContentApplicationJsonSchema
### Microsoft.Graph.PowerShell.Models.IUsersActionsIdentity
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphPermission
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IPathsQisc3SUsersUserIdDrivesDriveIdRootPermissionsPermissionIdMicrosoftGraphGrantPostRequestbodyContentApplicationJsonSchema\>: .
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Recipients \<IMicrosoftGraphDriveRecipient\[\]\>\]: 
    \[Alias \<String\>\]: The alias of the domain object, for cases where an email address is unavailable (e.g.
security groups).
    \[Email \<String\>\]: The email address for the recipient, if the recipient has an associated email address.
    \[ObjectId \<String\>\]: The unique identifier for the recipient in the directory.
  \[Roles \<String\[\]\>\]: 

INPUTOBJECT \<IUsersActionsIdentity\>: Identity Parameter
  \[AuthenticationMethodId \<String\>\]: The unique identifier of authenticationMethod
  \[CalendarId \<String\>\]: The unique identifier of calendar
  \[ChatId \<String\>\]: The unique identifier of chat
  \[ChatMessageId \<String\>\]: The unique identifier of chatMessage
  \[ChatMessageId1 \<String\>\]: The unique identifier of chatMessage
  \[ContentTypeId \<String\>\]: The unique identifier of contentType
  \[DeviceLogCollectionResponseId \<String\>\]: The unique identifier of deviceLogCollectionResponse
  \[DocumentSetVersionId \<String\>\]: The unique identifier of documentSetVersion
  \[DriveId \<String\>\]: The unique identifier of drive
  \[DriveItemId \<String\>\]: The unique identifier of driveItem
  \[DriveItemVersionId \<String\>\]: The unique identifier of driveItemVersion
  \[EventId \<String\>\]: The unique identifier of event
  \[EventId1 \<String\>\]: The unique identifier of event
  \[ListItemId \<String\>\]: The unique identifier of listItem
  \[ListItemVersionId \<String\>\]: The unique identifier of listItemVersion
  \[MailFolderId \<String\>\]: The unique identifier of mailFolder
  \[MailFolderId1 \<String\>\]: The unique identifier of mailFolder
  \[ManagedDeviceId \<String\>\]: The unique identifier of managedDevice
  \[MessageId \<String\>\]: The unique identifier of message
  \[NotebookId \<String\>\]: The unique identifier of notebook
  \[OnenotePageId \<String\>\]: The unique identifier of onenotePage
  \[OnenoteSectionId \<String\>\]: The unique identifier of onenoteSection
  \[PermissionId \<String\>\]: The unique identifier of permission
  \[PhoneAuthenticationMethodId \<String\>\]: The unique identifier of phoneAuthenticationMethod
  \[SubscriptionId \<String\>\]: The unique identifier of subscription
  \[TeamsAppInstallationId \<String\>\]: The unique identifier of teamsAppInstallation
  \[TodoTaskId \<String\>\]: The unique identifier of todoTask
  \[TodoTaskListId \<String\>\]: The unique identifier of todoTaskList
  \[UserId \<String\>\]: The unique identifier of user

RECIPIENTS \<IMicrosoftGraphDriveRecipient\[\]\>: .
  \[Alias \<String\>\]: The alias of the domain object, for cases where an email address is unavailable (e.g.
security groups).
  \[Email \<String\>\]: The email address for the recipient, if the recipient has an associated email address.
  \[ObjectId \<String\>\]: The unique identifier for the recipient in the directory.

## RELATED LINKS
[Grant-MgBetaUserDriveRootPermission](/powershell/module/Microsoft.Graph.Beta.Users.Actions/Grant-MgBetaUserDriveRootPermission?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.users.actions/grant-mguserdriverootpermission](https://learn.microsoft.com/powershell/module/microsoft.graph.users.actions/grant-mguserdriverootpermission)

