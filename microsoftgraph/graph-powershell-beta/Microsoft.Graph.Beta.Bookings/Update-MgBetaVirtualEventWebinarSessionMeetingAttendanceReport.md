---
external help file: Microsoft.Graph.Beta.Bookings-help.xml
Module Name: Microsoft.Graph.Beta.Bookings
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.bookings/update-mgbetavirtualeventwebinarsessionmeetingattendancereport
schema: 2.0.0
---

# Update-MgBetaVirtualEventWebinarSessionMeetingAttendanceReport

## SYNOPSIS
Update the navigation property meetingAttendanceReport in solutions

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaVirtualEventWebinarSessionMeetingAttendanceReport -VirtualEventSessionId <String>
 -VirtualEventWebinarId <String> [-AdditionalProperties <Hashtable>]
 [-AttendanceRecords <IMicrosoftGraphAttendanceRecord[]>] [-Id <String>] [-MeetingEndDateTime <DateTime>]
 [-MeetingStartDateTime <DateTime>] [-TotalParticipantCount <Int32>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaVirtualEventWebinarSessionMeetingAttendanceReport -VirtualEventSessionId <String>
 -VirtualEventWebinarId <String> -BodyParameter <IMicrosoftGraphMeetingAttendanceReport> [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaVirtualEventWebinarSessionMeetingAttendanceReport -InputObject <IBookingsIdentity>
 [-AdditionalProperties <Hashtable>] [-AttendanceRecords <IMicrosoftGraphAttendanceRecord[]>] [-Id <String>]
 [-MeetingEndDateTime <DateTime>] [-MeetingStartDateTime <DateTime>] [-TotalParticipantCount <Int32>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaVirtualEventWebinarSessionMeetingAttendanceReport -InputObject <IBookingsIdentity>
 -BodyParameter <IMicrosoftGraphMeetingAttendanceReport> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property meetingAttendanceReport in solutions

## PARAMETERS

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

### -AttendanceRecords
List of attendance records of an attendance report.
Read-only.
To construct, see NOTES section for ATTENDANCERECORDS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAttendanceRecord[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
meetingAttendanceReport
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphMeetingAttendanceReport
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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
Type: IBookingsIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -MeetingEndDateTime
UTC time when the meeting ended.
Read-only.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MeetingStartDateTime
UTC time when the meeting started.
Read-only.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TotalParticipantCount
Total number of participants.
Read-only.

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

### -VirtualEventSessionId
The unique identifier of virtualEventSession

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

### -VirtualEventWebinarId
The unique identifier of virtualEventWebinar

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

### Microsoft.Graph.Beta.PowerShell.Models.IBookingsIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphMeetingAttendanceReport
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphMeetingAttendanceReport
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ATTENDANCERECORDS \<IMicrosoftGraphAttendanceRecord\[\]\>: List of attendance records of an attendance report.
Read-only.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[AttendanceIntervals \<IMicrosoftGraphAttendanceInterval\[\]\>\]: List of time periods between joining and leaving a meeting.
    \[DurationInSeconds \<Int32?\>\]: Duration of the meeting interval in seconds; that is, the difference between joinDateTime and leaveDateTime.
    \[JoinDateTime \<DateTime?\>\]: The time the attendee joined in UTC.
    \[LeaveDateTime \<DateTime?\>\]: The time the attendee left in UTC.
  \[EmailAddress \<String\>\]: Email address of the user associated with this attendance record.
  \[Identity \<IMicrosoftGraphIdentity\>\]: identity
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[DisplayName \<String\>\]: The display name of the identity.
This might not always be available or up to date.
For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
    \[Id \<String\>\]: Unique identifier for the identity.
  \[RegistrantId \<String\>\]: Unique identifier of a meetingRegistrant.
Presents when the participant has registered for the meeting.
  \[Role \<String\>\]: Role of the attendee.
Possible values are: None, Attendee, Presenter, and Organizer.
  \[TotalAttendanceInSeconds \<Int32?\>\]: Total duration of the attendances in seconds.

BODYPARAMETER \<IMicrosoftGraphMeetingAttendanceReport\>: meetingAttendanceReport
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[AttendanceRecords \<IMicrosoftGraphAttendanceRecord\[\]\>\]: List of attendance records of an attendance report.
Read-only.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[AttendanceIntervals \<IMicrosoftGraphAttendanceInterval\[\]\>\]: List of time periods between joining and leaving a meeting.
      \[DurationInSeconds \<Int32?\>\]: Duration of the meeting interval in seconds; that is, the difference between joinDateTime and leaveDateTime.
      \[JoinDateTime \<DateTime?\>\]: The time the attendee joined in UTC.
      \[LeaveDateTime \<DateTime?\>\]: The time the attendee left in UTC.
    \[EmailAddress \<String\>\]: Email address of the user associated with this attendance record.
    \[Identity \<IMicrosoftGraphIdentity\>\]: identity
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[DisplayName \<String\>\]: The display name of the identity.
This might not always be available or up to date.
For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
      \[Id \<String\>\]: Unique identifier for the identity.
    \[RegistrantId \<String\>\]: Unique identifier of a meetingRegistrant.
Presents when the participant has registered for the meeting.
    \[Role \<String\>\]: Role of the attendee.
Possible values are: None, Attendee, Presenter, and Organizer.
    \[TotalAttendanceInSeconds \<Int32?\>\]: Total duration of the attendances in seconds.
  \[MeetingEndDateTime \<DateTime?\>\]: UTC time when the meeting ended.
Read-only.
  \[MeetingStartDateTime \<DateTime?\>\]: UTC time when the meeting started.
Read-only.
  \[TotalParticipantCount \<Int32?\>\]: Total number of participants.
Read-only.

INPUTOBJECT \<IBookingsIdentity\>: Identity Parameter
  \[AttendanceRecordId \<String\>\]: The unique identifier of attendanceRecord
  \[BookingAppointmentId \<String\>\]: The unique identifier of bookingAppointment
  \[BookingBusinessId \<String\>\]: The unique identifier of bookingBusiness
  \[BookingCurrencyId \<String\>\]: The unique identifier of bookingCurrency
  \[BookingCustomQuestionId \<String\>\]: The unique identifier of bookingCustomQuestion
  \[BookingCustomerId \<String\>\]: The unique identifier of bookingCustomer
  \[BookingServiceId \<String\>\]: The unique identifier of bookingService
  \[BookingStaffMemberId \<String\>\]: The unique identifier of bookingStaffMember
  \[BusinessScenarioId \<String\>\]: The unique identifier of businessScenario
  \[BusinessScenarioTaskId \<String\>\]: The unique identifier of businessScenarioTask
  \[CallRecordingId \<String\>\]: The unique identifier of callRecording
  \[CallTranscriptId \<String\>\]: The unique identifier of callTranscript
  \[MeetingAttendanceReportId \<String\>\]: The unique identifier of meetingAttendanceReport
  \[MeetingRegistrantBaseId \<String\>\]: The unique identifier of meetingRegistrantBase
  \[MeetingRegistrationQuestionId \<String\>\]: The unique identifier of meetingRegistrationQuestion
  \[PlannerPlanConfigurationLocalizationId \<String\>\]: The unique identifier of plannerPlanConfigurationLocalization
  \[Role \<String\>\]: Usage: role='{role}'
  \[UserId \<String\>\]: Usage: userId='{userId}'
  \[VirtualEventId \<String\>\]: The unique identifier of virtualEvent
  \[VirtualEventPresenterId \<String\>\]: The unique identifier of virtualEventPresenter
  \[VirtualEventRegistrationId \<String\>\]: The unique identifier of virtualEventRegistration
  \[VirtualEventSessionId \<String\>\]: The unique identifier of virtualEventSession
  \[VirtualEventWebinarId \<String\>\]: The unique identifier of virtualEventWebinar

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.bookings/update-mgbetavirtualeventwebinarsessionmeetingattendancereport](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.bookings/update-mgbetavirtualeventwebinarsessionmeetingattendancereport)


