---
external help file: Microsoft.Graph.Beta.Users.Functions-help.xml
Module Name: Microsoft.Graph.Beta.Users.Functions
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users.functions/test-mgbetauserdrivelistcontenttypepublished
schema: 2.0.0
---

# Test-MgBetaUserDriveListContentTypePublished

## SYNOPSIS
Invoke function isPublished

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Test-MgUserDriveListContentTypePublished](/powershell/module/Microsoft.Graph.Users.Functions/Test-MgUserDriveListContentTypePublished?view=graph-powershell-1.0)

## SYNTAX

### Is (Default)
```
Test-MgBetaUserDriveListContentTypePublished -ContentTypeId <String> -DriveId <String> -UserId <String>
 [<CommonParameters>]
```

### IsViaIdentity
```
Test-MgBetaUserDriveListContentTypePublished -InputObject <IUsersFunctionsIdentity> [<CommonParameters>]
```

## DESCRIPTION
Invoke function isPublished

## PARAMETERS

### -ContentTypeId
The unique identifier of contentType

```yaml
Type: String
Parameter Sets: Is
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DriveId
The unique identifier of drive

```yaml
Type: String
Parameter Sets: Is
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
Type: IUsersFunctionsIdentity
Parameter Sets: IsViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -UserId
The unique identifier of user

```yaml
Type: String
Parameter Sets: Is
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IUsersFunctionsIdentity
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT \<IUsersFunctionsIdentity\>: Identity Parameter
  \[AccessReviewInstanceId \<String\>\]: The unique identifier of accessReviewInstance
  \[AppConsentRequestId \<String\>\]: The unique identifier of appConsentRequest
  \[CalendarId \<String\>\]: The unique identifier of calendar
  \[ChatId \<String\>\]: The unique identifier of chat
  \[ChatMessageId \<String\>\]: The unique identifier of chatMessage
  \[CloudPcId \<String\>\]: The unique identifier of cloudPC
  \[ContactFolderId \<String\>\]: The unique identifier of contactFolder
  \[ContactFolderId1 \<String\>\]: The unique identifier of contactFolder
  \[ContentTypeId \<String\>\]: The unique identifier of contentType
  \[DriveId \<String\>\]: The unique identifier of drive
  \[DriveItemId \<String\>\]: The unique identifier of driveItem
  \[EndDateTime \<String\>\]: Usage: endDateTime='{endDateTime}'
  \[EventId \<String\>\]: The unique identifier of event
  \[GroupId \<String\>\]: Usage: groupId='{groupId}'
  \[IncludePersonalNotebooks \<Boolean?\>\]: Usage: includePersonalNotebooks={includePersonalNotebooks}
  \[Interval \<String\>\]: Usage: interval='{interval}'
  \[ListItemId \<String\>\]: The unique identifier of listItem
  \[MailFolderId \<String\>\]: The unique identifier of mailFolder
  \[MailFolderId1 \<String\>\]: The unique identifier of mailFolder
  \[ManagedDeviceId \<String\>\]: The unique identifier of managedDevice
  \[On \<String\>\]: Usage: on='{on}'
  \[OnenotePageId \<String\>\]: The unique identifier of onenotePage
  \[OnlineMeetingId \<String\>\]: The unique identifier of onlineMeeting
  \[PlannerBucketId \<String\>\]: The unique identifier of plannerBucket
  \[PlannerPlanId \<String\>\]: The unique identifier of plannerPlan
  \[Q \<String\>\]: Usage: q='{q}'
  \[RoomList \<String\>\]: Usage: RoomList='{RoomList}'
  \[ServicePlanId \<String\>\]: Usage: servicePlanId='{servicePlanId}'
  \[Skip \<Int32?\>\]: Usage: skip={skip}
  \[StartDateTime \<String\>\]: Usage: startDateTime='{startDateTime}'
  \[TimeZoneStandard \<String\>\]: Usage: TimeZoneStandard='{TimeZoneStandard}'
  \[TodoTaskListId \<String\>\]: The unique identifier of todoTaskList
  \[Token \<String\>\]: Usage: token='{token}'
  \[Top \<Int32?\>\]: Usage: top={top}
  \[Upn \<String\>\]: Usage: upn='{upn}'
  \[User \<String\>\]: Usage: User='{User}'
  \[UserId \<String\>\]: The unique identifier of user

## RELATED LINKS
[Test-MgUserDriveListContentTypePublished](/powershell/module/Microsoft.Graph.Users.Functions/Test-MgUserDriveListContentTypePublished?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users.functions/test-mgbetauserdrivelistcontenttypepublished](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users.functions/test-mgbetauserdrivelistcontenttypepublished)



