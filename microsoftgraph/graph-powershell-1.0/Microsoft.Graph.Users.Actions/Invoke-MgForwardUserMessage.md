---
external help file: Microsoft.Graph.Users.Actions-help.xml
Module Name: Microsoft.Graph.Users.Actions
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.users.actions/invoke-mgforwardusermessage
schema: 2.0.0
ms.prod: outlook
---

# Invoke-MgForwardUserMessage

## SYNOPSIS
Forward a message using either JSON or MIME format.
When using JSON format, you can:\n- Specify either a comment or the body property of the message parameter.
Specifying both will return an HTTP 400 Bad Request error.\n- Specify either the toRecipients parameter or the toRecipients property of the message parameter.
Specifying both or specifying neither will return an HTTP 400 Bad Request error.
When using MIME format:\n- Provide the applicable Internet message headers and the MIME content, all encoded in base64 format in the request body.\n- Add any attachments and S/MIME properties to the MIME content.
This method saves the message in the Sent Items folder.
Alternatively, create a draft to forward a message, and send it later.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the beta release of this cmdlet, view [Invoke-MgBetaForwardUserMessage](/powershell/module/Microsoft.Graph.Beta.Users.Actions/Invoke-MgBetaForwardUserMessage?view=graph-powershell-beta)

## SYNTAX

### ForwardExpanded (Default)
```
Invoke-MgForwardUserMessage -MessageId <String> -UserId <String> [-AdditionalProperties <Hashtable>]
 [-Comment <String>] [-Message <IMicrosoftGraphMessage>] [-ToRecipients <IMicrosoftGraphRecipient[]>]
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Forward
```
Invoke-MgForwardUserMessage -MessageId <String> -UserId <String>
 -BodyParameter <IPaths3Ta6EnUsersUserIdMessagesMessageIdMicrosoftGraphForwardPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ForwardViaIdentityExpanded
```
Invoke-MgForwardUserMessage -InputObject <IUsersActionsIdentity> [-AdditionalProperties <Hashtable>]
 [-Comment <String>] [-Message <IMicrosoftGraphMessage>] [-ToRecipients <IMicrosoftGraphRecipient[]>]
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ForwardViaIdentity
```
Invoke-MgForwardUserMessage -InputObject <IUsersActionsIdentity>
 -BodyParameter <IPaths3Ta6EnUsersUserIdMessagesMessageIdMicrosoftGraphForwardPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Forward a message using either JSON or MIME format.
When using JSON format, you can:\n- Specify either a comment or the body property of the message parameter.
Specifying both will return an HTTP 400 Bad Request error.\n- Specify either the toRecipients parameter or the toRecipients property of the message parameter.
Specifying both or specifying neither will return an HTTP 400 Bad Request error.
When using MIME format:\n- Provide the applicable Internet message headers and the MIME content, all encoded in base64 format in the request body.\n- Add any attachments and S/MIME properties to the MIME content.
This method saves the message in the Sent Items folder.
Alternatively, create a draft to forward a message, and send it later.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Using the Invoke-MgForwardUserMessage Cmdlet
```powershell
Import-Module Microsoft.Graph.Users.Actions
$params = @{
	Comment = "comment-value"
	ToRecipients = @(
		@{
			EmailAddress = @{
				Name = "name-value"
				Address = "address-value"
			}
		}
	)
}
# A UPN can also be used as -UserId.
Invoke-MgForwardUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params
```
This example shows how to use the Invoke-MgForwardUserMessage Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: ForwardExpanded, ForwardViaIdentityExpanded
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
Type: IPaths3Ta6EnUsersUserIdMessagesMessageIdMicrosoftGraphForwardPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Forward, ForwardViaIdentity
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
Parameter Sets: ForwardExpanded, ForwardViaIdentityExpanded
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
Parameter Sets: ForwardViaIdentityExpanded, ForwardViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Message
message
To construct, see NOTES section for MESSAGE properties and create a hash table.

```yaml
Type: IMicrosoftGraphMessage
Parameter Sets: ForwardExpanded, ForwardViaIdentityExpanded
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
Parameter Sets: ForwardExpanded, Forward
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

### -ToRecipients
.
To construct, see NOTES section for TORECIPIENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphRecipient[]
Parameter Sets: ForwardExpanded, ForwardViaIdentityExpanded
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
Parameter Sets: ForwardExpanded, Forward
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

### Microsoft.Graph.PowerShell.Models.IPaths3Ta6EnUsersUserIdMessagesMessageIdMicrosoftGraphForwardPostRequestbodyContentApplicationJsonSchema
### Microsoft.Graph.PowerShell.Models.IUsersActionsIdentity
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IPaths3Ta6EnUsersUserIdMessagesMessageIdMicrosoftGraphForwardPostRequestbodyContentApplicationJsonSchema\>: .
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Comment \<String\>\]: 
  \[Message \<IMicrosoftGraphMessage\>\]: message
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Categories \<String\[\]\>\]: The categories associated with the item
    \[ChangeKey \<String\>\]: Identifies the version of the item.
Every time the item is changed, changeKey changes as well.
This allows Exchange to apply changes to the correct version of the object.
Read-only.
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
      \[Name \<String\>\]: The attachment's file name.
      \[Size \<Int32?\>\]: The length of the attachment in bytes.
    \[BccRecipients \<IMicrosoftGraphRecipient\[\]\>\]: The Bcc: recipients for the message.
      \[EmailAddress \<IMicrosoftGraphEmailAddress\>\]: emailAddress
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[Address \<String\>\]: The email address of the person or entity.
        \[Name \<String\>\]: The display name of the person or entity.
    \[Body \<IMicrosoftGraphItemBody\>\]: itemBody
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Content \<String\>\]: The content of the item.
      \[ContentType \<String\>\]: bodyType
    \[BodyPreview \<String\>\]: The first 255 characters of the message body.
It is in text format.
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
        \[DateTime \<String\>\]: A single point of time in a combined date and time representation ({date}T{time}; for example, 2017-08-29T04:00:00.0000000).
        \[TimeZone \<String\>\]: Represents a time zone, for example, 'Pacific Standard Time'.
See below for more possible values.
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
    \[WebLink \<String\>\]: 
  \[ToRecipients \<IMicrosoftGraphRecipient\[\]\>\]: 

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

MESSAGE \<IMicrosoftGraphMessage\>: message
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Categories \<String\[\]\>\]: The categories associated with the item
  \[ChangeKey \<String\>\]: Identifies the version of the item.
Every time the item is changed, changeKey changes as well.
This allows Exchange to apply changes to the correct version of the object.
Read-only.
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
    \[Name \<String\>\]: The attachment's file name.
    \[Size \<Int32?\>\]: The length of the attachment in bytes.
  \[BccRecipients \<IMicrosoftGraphRecipient\[\]\>\]: The Bcc: recipients for the message.
    \[EmailAddress \<IMicrosoftGraphEmailAddress\>\]: emailAddress
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Address \<String\>\]: The email address of the person or entity.
      \[Name \<String\>\]: The display name of the person or entity.
  \[Body \<IMicrosoftGraphItemBody\>\]: itemBody
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Content \<String\>\]: The content of the item.
    \[ContentType \<String\>\]: bodyType
  \[BodyPreview \<String\>\]: The first 255 characters of the message body.
It is in text format.
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
      \[DateTime \<String\>\]: A single point of time in a combined date and time representation ({date}T{time}; for example, 2017-08-29T04:00:00.0000000).
      \[TimeZone \<String\>\]: Represents a time zone, for example, 'Pacific Standard Time'.
See below for more possible values.
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
  \[WebLink \<String\>\]: 

TORECIPIENTS \<IMicrosoftGraphRecipient\[\]\>: .
  \[EmailAddress \<IMicrosoftGraphEmailAddress\>\]: emailAddress
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Address \<String\>\]: The email address of the person or entity.
    \[Name \<String\>\]: The display name of the person or entity.

## RELATED LINKS
[Invoke-MgBetaForwardUserMessage](/powershell/module/Microsoft.Graph.Beta.Users.Actions/Invoke-MgBetaForwardUserMessage?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.users.actions/invoke-mgforwardusermessage](https://learn.microsoft.com/powershell/module/microsoft.graph.users.actions/invoke-mgforwardusermessage)

