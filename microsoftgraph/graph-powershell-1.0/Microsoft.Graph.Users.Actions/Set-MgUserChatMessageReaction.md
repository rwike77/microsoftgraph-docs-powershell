---
external help file: Microsoft.Graph.Users.Actions-help.xml
Module Name: Microsoft.Graph.Users.Actions
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.users.actions/set-mguserchatmessagereaction
schema: 2.0.0
---

# Set-MgUserChatMessageReaction

## SYNOPSIS
Invoke action setReaction

> [!NOTE]
> To view the beta release of this cmdlet, view [Set-MgBetaUserChatMessageReaction](/powershell/module/Microsoft.Graph.Beta.Users.Actions/Set-MgBetaUserChatMessageReaction?view=graph-powershell-beta)

## SYNTAX

### SetExpanded (Default)
```
Set-MgUserChatMessageReaction -ChatId <String> -ChatMessageId <String> -UserId <String>
 [-AdditionalProperties <Hashtable>] [-ReactionType <String>] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Set
```
Set-MgUserChatMessageReaction -ChatId <String> -ChatMessageId <String> -UserId <String>
 -BodyParameter <IPathsI6BvuqUsersUserIdChatsChatIdMessagesChatmessageIdMicrosoftGraphSetreactionPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SetViaIdentityExpanded
```
Set-MgUserChatMessageReaction -InputObject <IUsersActionsIdentity> [-AdditionalProperties <Hashtable>]
 [-ReactionType <String>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SetViaIdentity
```
Set-MgUserChatMessageReaction -InputObject <IUsersActionsIdentity>
 -BodyParameter <IPathsI6BvuqUsersUserIdChatsChatIdMessagesChatmessageIdMicrosoftGraphSetreactionPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Invoke action setReaction

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
Type: IPathsI6BvuqUsersUserIdChatsChatIdMessagesChatmessageIdMicrosoftGraphSetreactionPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Set, SetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ChatId
The unique identifier of chat

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

### -ChatMessageId
The unique identifier of chatMessage

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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IUsersActionsIdentity
Parameter Sets: SetViaIdentityExpanded, SetViaIdentity
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

### -ReactionType
.

```yaml
Type: String
Parameter Sets: SetExpanded, SetViaIdentityExpanded
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
Parameter Sets: SetExpanded, Set
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

### Microsoft.Graph.PowerShell.Models.IPathsI6BvuqUsersUserIdChatsChatIdMessagesChatmessageIdMicrosoftGraphSetreactionPostRequestbodyContentApplicationJsonSchema
### Microsoft.Graph.PowerShell.Models.IUsersActionsIdentity
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IPathsI6BvuqUsersUserIdChatsChatIdMessagesChatmessageIdMicrosoftGraphSetreactionPostRequestbodyContentApplicationJsonSchema\>: .
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[ReactionType \<String\>\]: 

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

## RELATED LINKS
[Set-MgBetaUserChatMessageReaction](/powershell/module/Microsoft.Graph.Beta.Users.Actions/Set-MgBetaUserChatMessageReaction?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.users.actions/set-mguserchatmessagereaction](https://learn.microsoft.com/powershell/module/microsoft.graph.users.actions/set-mguserchatmessagereaction)



