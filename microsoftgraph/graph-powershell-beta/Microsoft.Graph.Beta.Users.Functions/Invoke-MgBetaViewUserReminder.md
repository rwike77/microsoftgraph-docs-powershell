---
external help file: Microsoft.Graph.Beta.Users.Functions-help.xml
Module Name: Microsoft.Graph.Beta.Users.Functions
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users.functions/invoke-mgbetaviewuserreminder
schema: 2.0.0
---

# Invoke-MgBetaViewUserReminder

## SYNOPSIS
Invoke function reminderView

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Invoke-MgViewUserReminder](/powershell/module/Microsoft.Graph.Users.Functions/Invoke-MgViewUserReminder?view=graph-powershell-1.0)

## SYNTAX

### View (Default)
```
Invoke-MgBetaViewUserReminder -EndDateTime <String> -StartDateTime <String> -UserId <String> [-Count]
 [-Filter <String>] [-Search <String>] [-Skip <Int32>] [-Top <Int32>] [<CommonParameters>]
```

### ViewViaIdentity
```
Invoke-MgBetaViewUserReminder -InputObject <IUsersFunctionsIdentity> [-Count] [-Filter <String>]
 [-Search <String>] [-Skip <Int32>] [-Top <Int32>] [<CommonParameters>]
```

## DESCRIPTION
Invoke function reminderView

## PARAMETERS

### -Count
Include count of items

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

### -EndDateTime
Usage: EndDateTime='{EndDateTime}'

```yaml
Type: String
Parameter Sets: View
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Filter
Filter items by property values

```yaml
Type: String
Parameter Sets: (All)
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
Type: IUsersFunctionsIdentity
Parameter Sets: ViewViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Search
Search items by search phrases

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StartDateTime
Usage: StartDateTime='{StartDateTime}'

```yaml
Type: String
Parameter Sets: View
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Top
Show only the first n items

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: Limit

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserId
The unique identifier of user

```yaml
Type: String
Parameter Sets: View
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Skip
Skip the first n items

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IUsersFunctionsIdentity
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphReminder
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
[Invoke-MgViewUserReminder](/powershell/module/Microsoft.Graph.Users.Functions/Invoke-MgViewUserReminder?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users.functions/invoke-mgbetaviewuserreminder](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users.functions/invoke-mgbetaviewuserreminder)



