---
external help file: Microsoft.Graph.Beta.Users.Actions-help.xml
Module Name: Microsoft.Graph.Beta.Users.Actions
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users.actions/invoke-mgbetareplyusermailfoldermessage
schema: 2.0.0
ms.prod: outlook
---

# Invoke-MgBetaReplyUserMailFolderMessage

## SYNOPSIS
Reply to the sender of a message using either JSON or MIME format.
When using JSON format:* Specify either a comment or the body property of the message parameter.
Specifying both will return an HTTP 400 Bad Request error.* If the original message specifies a recipient in the replyTo property, per Internet Message Format (RFC 2822), send the reply to the recipients in replyTo and not the recipient in the from property.
When using MIME format:- Provide the applicable Internet message headers and the MIME content, all encoded in base64 format in the request body.- Add any attachments and S/MIME properties to the MIME content.
This method saves the message in the Sent Items folder.
Alternatively, create a draft to reply to a message, and send it later.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Invoke-MgReplyUserMailFolderMessage](/powershell/module/Microsoft.Graph.Users.Actions/Invoke-MgReplyUserMailFolderMessage?view=graph-powershell-1.0)

## SYNTAX

### ReplyExpanded (Default)
```
Invoke-MgBetaReplyUserMailFolderMessage -MailFolderId <String> -MessageId <String> -UserId <String>
 [-AdditionalProperties <Hashtable>] [-Comment <String>] [-Message <IMicrosoftGraphMessage>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Reply
```
Invoke-MgBetaReplyUserMailFolderMessage -MailFolderId <String> -MessageId <String> -UserId <String>
 -BodyParameter <IPaths6Zjq1HUsersUserIdMailfoldersMailfolderIdMessagesMessageIdMicrosoftGraphReplyPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ReplyViaIdentityExpanded
```
Invoke-MgBetaReplyUserMailFolderMessage -InputObject <IUsersActionsIdentity>
 [-AdditionalProperties <Hashtable>] [-Comment <String>] [-Message <IMicrosoftGraphMessage>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ReplyViaIdentity
```
Invoke-MgBetaReplyUserMailFolderMessage -InputObject <IUsersActionsIdentity>
 -BodyParameter <IPaths6Zjq1HUsersUserIdMailfoldersMailfolderIdMessagesMessageIdMicrosoftGraphReplyPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Reply to the sender of a message using either JSON or MIME format.
When using JSON format:* Specify either a comment or the body property of the message parameter.
Specifying both will return an HTTP 400 Bad Request error.* If the original message specifies a recipient in the replyTo property, per Internet Message Format (RFC 2822), send the reply to the recipients in replyTo and not the recipient in the from property.
When using MIME format:- Provide the applicable Internet message headers and the MIME content, all encoded in base64 format in the request body.- Add any attachments and S/MIME properties to the MIME content.
This method saves the message in the Sent Items folder.
Alternatively, create a draft to reply to a message, and send it later.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Reply in JSON format to an existing message

```powershell
Import-Module Microsoft.Graph.Beta.Users.Actions

$params = @{
	Message = @{
		ToRecipients = @(
			@{
				EmailAddress = @{
					Address = "samanthab@contoso.onmicrosoft.com"
					Name = "Samantha Booth"
				}
			}
			@{
				EmailAddress = @{
					Address = "randiw@contoso.onmicrosoft.com"
					Name = "Randi Welch"
				}
			}
		)
	}
	Comment = "Samantha, Randi, would you name the group please?"
}

# A UPN can also be used as -UserId.
Invoke-MgBetaReplyUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params
```
This example shows how to use the Invoke-MgBetaReplyUserMailFolderMessage Cmdlet.

To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: ReplyExpanded, ReplyViaIdentityExpanded
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
Type: IPaths6Zjq1HUsersUserIdMailfoldersMailfolderIdMessagesMessageIdMicrosoftGraphReplyPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Reply, ReplyViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Comment
.

```yaml
Type: String
Parameter Sets: ReplyExpanded, ReplyViaIdentityExpanded
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
Type: IUsersActionsIdentity
Parameter Sets: ReplyViaIdentityExpanded, ReplyViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -MailFolderId
The unique identifier of mailFolder

```yaml
Type: String
Parameter Sets: ReplyExpanded, Reply
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Message
message
To construct, see NOTES section for MESSAGE properties and create a hash table.

```yaml
Type: IMicrosoftGraphMessage
Parameter Sets: ReplyExpanded, ReplyViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MessageId
The unique identifier of message

```yaml
Type: String
Parameter Sets: ReplyExpanded, Reply
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

### -UserId
The unique identifier of user

```yaml
Type: String
Parameter Sets: ReplyExpanded, Reply
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

### Microsoft.Graph.Beta.PowerShell.Models.IPaths6Zjq1HUsersUserIdMailfoldersMailfolderIdMessagesMessageIdMicrosoftGraphReplyPostRequestbodyContentApplicationJsonSchema
### Microsoft.Graph.Beta.PowerShell.Models.IUsersActionsIdentity
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IPaths6Zjq1HUsersUserIdMailfoldersMailfolderIdMessagesMessageIdMicrosoftGraphReplyPostRequestbodyContentApplicationJsonSchema\>: .
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Comment \<String\>\]: 
  \[Message \<IMicrosoftGraphMessage\>\]: message
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Categories \<String\[\]\>\]: 
    \[ChangeKey \<String\>\]: 
    \[CreatedDateTime \<DateTime?\>\]: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    \[LastModifiedDateTime \<DateTime?\>\]: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[Attachments \<IMicrosoftGraphAttachment\[\]\>\]: The fileAttachment and itemAttachment attachments for the message.
      \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
      \[ContentType \<String\>\]: The MIME type.
      \[IsInline \<Boolean?\>\]: true if the attachment is an inline attachment; otherwise, false.
      \[LastModifiedDateTime \<DateTime?\>\]: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      \[Name \<String\>\]: The display name of the attachment.
This does not need to be the actual file name.
      \[Size \<Int32?\>\]: The length of the attachment in bytes.
    \[BccRecipients \<IMicrosoftGraphRecipient\[\]\>\]: The Bcc: recipients for the message.
      \[EmailAddress \<IMicrosoftGraphEmailAddress\>\]: emailAddress
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[Address \<String\>\]: The email address of an entity instance.
        \[Name \<String\>\]: The display name of an entity instance.
    \[Body \<IMicrosoftGraphItemBody\>\]: itemBody
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Content \<String\>\]: The content of the item.
      \[ContentType \<String\>\]: bodyType
    \[BodyPreview \<String\>\]: The first 255 characters of the message body.
It is in text format.
If the message contains instances of mention, this property would contain a concatenation of these mentions as well.
    \[CcRecipients \<IMicrosoftGraphRecipient\[\]\>\]: The Cc: recipients for the message.
    \[ConversationId \<String\>\]: The ID of the conversation the email belongs to.
    \[ConversationIndex \<Byte\[\]\>\]: Indicates the position of the message within the conversation.
    \[Extensions \<IMicrosoftGraphExtension\[\]\>\]: The collection of open extensions defined for the message.
Nullable.
      \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[Flag \<IMicrosoftGraphFollowupFlag\>\]: followupFlag
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[CompletedDateTime \<IMicrosoftGraphDateTimeZone\>\]: dateTimeTimeZone
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[DateTime \<String\>\]: A single point of time in a combined date and time representation ({date}T{time}).
For example, '2019-04-16T09:00:00'.
        \[TimeZone \<String\>\]: Represents a time zone, for example, 'Pacific Standard Time'.
See below for possible values.
      \[DueDateTime \<IMicrosoftGraphDateTimeZone\>\]: dateTimeTimeZone
      \[FlagStatus \<String\>\]: followupFlagStatus
      \[StartDateTime \<IMicrosoftGraphDateTimeZone\>\]: dateTimeTimeZone
    \[From \<IMicrosoftGraphRecipient\>\]: recipient
    \[HasAttachments \<Boolean?\>\]: Indicates whether the message has attachments.
This property doesn't include inline attachments, so if a message contains only inline attachments, this property is false.
To verify the existence of inline attachments, parse the body property to look for a src attribute, such as \<IMG src='cid:image001.jpg@01D26CD8.6C05F070'\>.
    \[Importance \<String\>\]: importance
    \[InferenceClassification \<String\>\]: inferenceClassificationType
    \[InternetMessageHeaders \<IMicrosoftGraphInternetMessageHeader\[\]\>\]: 
      \[Name \<String\>\]: Represents the key in a key-value pair.
      \[Value \<String\>\]: The value in a key-value pair.
    \[InternetMessageId \<String\>\]: 
    \[IsDeliveryReceiptRequested \<Boolean?\>\]: 
    \[IsDraft \<Boolean?\>\]: 
    \[IsRead \<Boolean?\>\]: 
    \[IsReadReceiptRequested \<Boolean?\>\]: 
    \[Mentions \<IMicrosoftGraphMention\[\]\>\]: A collection of mentions in the message, ordered by the createdDateTime from the newest to the oldest.
By default, a GET /messages does not return this property unless you apply $expand on the property.
      \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
      \[Application \<String\>\]: The name of the application where the mention is created.
Optional.
Not used and defaulted as null for message.
      \[ClientReference \<String\>\]: A unique identifier that represents a parent of the resource instance.
Optional.
Not used and defaulted as null for message.
      \[CreatedBy \<IMicrosoftGraphEmailAddress\>\]: emailAddress
      \[CreatedDateTime \<DateTime?\>\]: The date and time that the mention is created on the client.
      \[DeepLink \<String\>\]: A deep web link to the context of the mention in the resource instance.
Optional.
Not used and defaulted as null for message.
      \[MentionText \<String\>\]: Optional.
Not used and defaulted as null for message.
To get the mentions in a message, see the bodyPreview property of the message instead.
      \[Mentioned \<IMicrosoftGraphEmailAddress\>\]: emailAddress
      \[ServerCreatedDateTime \<DateTime?\>\]: The date and time that the mention is created on the server.
Optional.
Not used and defaulted as null for message.
    \[MentionsPreview \<IMicrosoftGraphMentionsPreview\>\]: mentionsPreview
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[IsMentioned \<Boolean?\>\]: True if the signed-in user is mentioned in the parent resource instance.
Read-only.
Supports filter.
    \[MultiValueExtendedProperties \<IMicrosoftGraphMultiValueLegacyExtendedProperty\[\]\>\]: The collection of multi-value extended properties defined for the message.
Nullable.
      \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
      \[Value \<String\[\]\>\]: A collection of property values.
    \[ParentFolderId \<String\>\]: 
    \[ReceivedDateTime \<DateTime?\>\]: 
    \[ReplyTo \<IMicrosoftGraphRecipient\[\]\>\]: 
    \[Sender \<IMicrosoftGraphRecipient\>\]: recipient
    \[SentDateTime \<DateTime?\>\]: 
    \[SingleValueExtendedProperties \<IMicrosoftGraphSingleValueLegacyExtendedProperty\[\]\>\]: The collection of single-value extended properties defined for the message.
Nullable.
      \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
      \[Value \<String\>\]: A property value.
    \[Subject \<String\>\]: 
    \[ToRecipients \<IMicrosoftGraphRecipient\[\]\>\]: 
    \[UniqueBody \<IMicrosoftGraphItemBody\>\]: itemBody
    \[UnsubscribeData \<String\[\]\>\]: 
    \[UnsubscribeEnabled \<Boolean?\>\]: 
    \[WebLink \<String\>\]: 

INPUTOBJECT \<IUsersActionsIdentity\>: Identity Parameter
  \[AccessReviewInstanceId \<String\>\]: The unique identifier of accessReviewInstance
  \[AccessReviewStageId \<String\>\]: The unique identifier of accessReviewStage
  \[AppLogCollectionRequestId \<String\>\]: The unique identifier of appLogCollectionRequest
  \[AuthenticationMethodId \<String\>\]: The unique identifier of authenticationMethod
  \[CalendarId \<String\>\]: The unique identifier of calendar
  \[ChatId \<String\>\]: The unique identifier of chat
  \[ChatMessageId \<String\>\]: The unique identifier of chatMessage
  \[ChatMessageId1 \<String\>\]: The unique identifier of chatMessage
  \[CloudPcId \<String\>\]: The unique identifier of cloudPC
  \[ContentTypeId \<String\>\]: The unique identifier of contentType
  \[DeviceEnrollmentConfigurationId \<String\>\]: The unique identifier of deviceEnrollmentConfiguration
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
  \[MobileAppTroubleshootingEventId \<String\>\]: The unique identifier of mobileAppTroubleshootingEvent
  \[NotebookId \<String\>\]: The unique identifier of notebook
  \[OnenotePageId \<String\>\]: The unique identifier of onenotePage
  \[OnenoteSectionId \<String\>\]: The unique identifier of onenoteSection
  \[OutlookTaskFolderId \<String\>\]: The unique identifier of outlookTaskFolder
  \[OutlookTaskGroupId \<String\>\]: The unique identifier of outlookTaskGroup
  \[OutlookTaskId \<String\>\]: The unique identifier of outlookTask
  \[PermissionId \<String\>\]: The unique identifier of permission
  \[PlannerPlanId \<String\>\]: The unique identifier of plannerPlan
  \[SensitivityLabelId \<String\>\]: The unique identifier of sensitivityLabel
  \[SubscriptionId \<String\>\]: The unique identifier of subscription
  \[TeamsAppInstallationId \<String\>\]: The unique identifier of teamsAppInstallation
  \[TodoTaskId \<String\>\]: The unique identifier of todoTask
  \[TodoTaskListId \<String\>\]: The unique identifier of todoTaskList
  \[UserId \<String\>\]: The unique identifier of user

MESSAGE \<IMicrosoftGraphMessage\>: message
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Categories \<String\[\]\>\]: 
  \[ChangeKey \<String\>\]: 
  \[CreatedDateTime \<DateTime?\>\]: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  \[LastModifiedDateTime \<DateTime?\>\]: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[Attachments \<IMicrosoftGraphAttachment\[\]\>\]: The fileAttachment and itemAttachment attachments for the message.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[ContentType \<String\>\]: The MIME type.
    \[IsInline \<Boolean?\>\]: true if the attachment is an inline attachment; otherwise, false.
    \[LastModifiedDateTime \<DateTime?\>\]: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    \[Name \<String\>\]: The display name of the attachment.
This does not need to be the actual file name.
    \[Size \<Int32?\>\]: The length of the attachment in bytes.
  \[BccRecipients \<IMicrosoftGraphRecipient\[\]\>\]: The Bcc: recipients for the message.
    \[EmailAddress \<IMicrosoftGraphEmailAddress\>\]: emailAddress
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Address \<String\>\]: The email address of an entity instance.
      \[Name \<String\>\]: The display name of an entity instance.
  \[Body \<IMicrosoftGraphItemBody\>\]: itemBody
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Content \<String\>\]: The content of the item.
    \[ContentType \<String\>\]: bodyType
  \[BodyPreview \<String\>\]: The first 255 characters of the message body.
It is in text format.
If the message contains instances of mention, this property would contain a concatenation of these mentions as well.
  \[CcRecipients \<IMicrosoftGraphRecipient\[\]\>\]: The Cc: recipients for the message.
  \[ConversationId \<String\>\]: The ID of the conversation the email belongs to.
  \[ConversationIndex \<Byte\[\]\>\]: Indicates the position of the message within the conversation.
  \[Extensions \<IMicrosoftGraphExtension\[\]\>\]: The collection of open extensions defined for the message.
Nullable.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[Flag \<IMicrosoftGraphFollowupFlag\>\]: followupFlag
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[CompletedDateTime \<IMicrosoftGraphDateTimeZone\>\]: dateTimeTimeZone
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[DateTime \<String\>\]: A single point of time in a combined date and time representation ({date}T{time}).
For example, '2019-04-16T09:00:00'.
      \[TimeZone \<String\>\]: Represents a time zone, for example, 'Pacific Standard Time'.
See below for possible values.
    \[DueDateTime \<IMicrosoftGraphDateTimeZone\>\]: dateTimeTimeZone
    \[FlagStatus \<String\>\]: followupFlagStatus
    \[StartDateTime \<IMicrosoftGraphDateTimeZone\>\]: dateTimeTimeZone
  \[From \<IMicrosoftGraphRecipient\>\]: recipient
  \[HasAttachments \<Boolean?\>\]: Indicates whether the message has attachments.
This property doesn't include inline attachments, so if a message contains only inline attachments, this property is false.
To verify the existence of inline attachments, parse the body property to look for a src attribute, such as \<IMG src='cid:image001.jpg@01D26CD8.6C05F070'\>.
  \[Importance \<String\>\]: importance
  \[InferenceClassification \<String\>\]: inferenceClassificationType
  \[InternetMessageHeaders \<IMicrosoftGraphInternetMessageHeader\[\]\>\]: 
    \[Name \<String\>\]: Represents the key in a key-value pair.
    \[Value \<String\>\]: The value in a key-value pair.
  \[InternetMessageId \<String\>\]: 
  \[IsDeliveryReceiptRequested \<Boolean?\>\]: 
  \[IsDraft \<Boolean?\>\]: 
  \[IsRead \<Boolean?\>\]: 
  \[IsReadReceiptRequested \<Boolean?\>\]: 
  \[Mentions \<IMicrosoftGraphMention\[\]\>\]: A collection of mentions in the message, ordered by the createdDateTime from the newest to the oldest.
By default, a GET /messages does not return this property unless you apply $expand on the property.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[Application \<String\>\]: The name of the application where the mention is created.
Optional.
Not used and defaulted as null for message.
    \[ClientReference \<String\>\]: A unique identifier that represents a parent of the resource instance.
Optional.
Not used and defaulted as null for message.
    \[CreatedBy \<IMicrosoftGraphEmailAddress\>\]: emailAddress
    \[CreatedDateTime \<DateTime?\>\]: The date and time that the mention is created on the client.
    \[DeepLink \<String\>\]: A deep web link to the context of the mention in the resource instance.
Optional.
Not used and defaulted as null for message.
    \[MentionText \<String\>\]: Optional.
Not used and defaulted as null for message.
To get the mentions in a message, see the bodyPreview property of the message instead.
    \[Mentioned \<IMicrosoftGraphEmailAddress\>\]: emailAddress
    \[ServerCreatedDateTime \<DateTime?\>\]: The date and time that the mention is created on the server.
Optional.
Not used and defaulted as null for message.
  \[MentionsPreview \<IMicrosoftGraphMentionsPreview\>\]: mentionsPreview
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[IsMentioned \<Boolean?\>\]: True if the signed-in user is mentioned in the parent resource instance.
Read-only.
Supports filter.
  \[MultiValueExtendedProperties \<IMicrosoftGraphMultiValueLegacyExtendedProperty\[\]\>\]: The collection of multi-value extended properties defined for the message.
Nullable.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[Value \<String\[\]\>\]: A collection of property values.
  \[ParentFolderId \<String\>\]: 
  \[ReceivedDateTime \<DateTime?\>\]: 
  \[ReplyTo \<IMicrosoftGraphRecipient\[\]\>\]: 
  \[Sender \<IMicrosoftGraphRecipient\>\]: recipient
  \[SentDateTime \<DateTime?\>\]: 
  \[SingleValueExtendedProperties \<IMicrosoftGraphSingleValueLegacyExtendedProperty\[\]\>\]: The collection of single-value extended properties defined for the message.
Nullable.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[Value \<String\>\]: A property value.
  \[Subject \<String\>\]: 
  \[ToRecipients \<IMicrosoftGraphRecipient\[\]\>\]: 
  \[UniqueBody \<IMicrosoftGraphItemBody\>\]: itemBody
  \[UnsubscribeData \<String\[\]\>\]: 
  \[UnsubscribeEnabled \<Boolean?\>\]: 
  \[WebLink \<String\>\]:

## RELATED LINKS
[Invoke-MgReplyUserMailFolderMessage](/powershell/module/Microsoft.Graph.Users.Actions/Invoke-MgReplyUserMailFolderMessage?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users.actions/invoke-mgbetareplyusermailfoldermessage](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users.actions/invoke-mgbetareplyusermailfoldermessage)


