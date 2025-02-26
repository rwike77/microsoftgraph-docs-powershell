---
external help file: Microsoft.Graph.Beta.Bookings-help.xml
Module Name: Microsoft.Graph.Beta.Bookings
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.bookings/new-mgbetabookingbusinessservice
schema: 2.0.0
ms.prod: bookings
---

# New-MgBetaBookingBusinessService

## SYNOPSIS
Create a new bookingService for the specified bookingBusiness.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgBookingBusinessService](/powershell/module/Microsoft.Graph.Bookings/New-MgBookingBusinessService?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaBookingBusinessService -BookingBusinessId <String> [-AdditionalInformation <String>]
 [-AdditionalProperties <Hashtable>] [-CustomQuestions <IMicrosoftGraphBookingQuestionAssignment[]>]
 [-DefaultDuration <TimeSpan>] [-DefaultLocation <IMicrosoftGraphLocation>] [-DefaultPrice <Double>]
 [-DefaultPriceType <BookingPriceType>] [-DefaultReminders <IMicrosoftGraphBookingReminder[]>]
 [-Description <String>] [-DisplayName <String>] [-Id <String>] [-IsAnonymousJoinEnabled]
 [-IsHiddenFromCustomers] [-IsLocationOnline] [-LanguageTag <String>] [-MaximumAttendeesCount <Int32>]
 [-Notes <String>] [-PostBuffer <TimeSpan>] [-PreBuffer <TimeSpan>]
 [-SchedulingPolicy <IMicrosoftGraphBookingSchedulingPolicy>] [-SmsNotificationsEnabled]
 [-StaffMemberIds <String[]>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaBookingBusinessService -BookingBusinessId <String> -BodyParameter <IMicrosoftGraphBookingService>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgBetaBookingBusinessService -InputObject <IBookingsIdentity> [-AdditionalInformation <String>]
 [-AdditionalProperties <Hashtable>] [-CustomQuestions <IMicrosoftGraphBookingQuestionAssignment[]>]
 [-DefaultDuration <TimeSpan>] [-DefaultLocation <IMicrosoftGraphLocation>] [-DefaultPrice <Double>]
 [-DefaultPriceType <BookingPriceType>] [-DefaultReminders <IMicrosoftGraphBookingReminder[]>]
 [-Description <String>] [-DisplayName <String>] [-Id <String>] [-IsAnonymousJoinEnabled]
 [-IsHiddenFromCustomers] [-IsLocationOnline] [-LanguageTag <String>] [-MaximumAttendeesCount <Int32>]
 [-Notes <String>] [-PostBuffer <TimeSpan>] [-PreBuffer <TimeSpan>]
 [-SchedulingPolicy <IMicrosoftGraphBookingSchedulingPolicy>] [-SmsNotificationsEnabled]
 [-StaffMemberIds <String[]>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgBetaBookingBusinessService -InputObject <IBookingsIdentity>
 -BodyParameter <IMicrosoftGraphBookingService> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new bookingService for the specified bookingBusiness.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Using the New-MgBetaBookingBusinessService Cmdlet
```powershell
Import-Module Microsoft.Graph.Beta.Bookings
$params = @{
	"@odata.type" = "#microsoft.graph.bookingService"
	DefaultDuration = "PT1H30M"
	DefaultLocation = @{
		"@odata.type" = "#microsoft.graph.location"
		Address = @{
			"@odata.type" = "#microsoft.graph.physicalAddress"
			City = "Buffalo"
			CountryOrRegion = "USA"
			PostalCode = "98052"
			PostOfficeBox = $null
			State = "NY"
			Street = "4567 First Street"
			"Type@odata.type" = "#microsoft.graph.physicalAddressType"
			Type = $null
		}
		Coordinates = $null
		DisplayName = "Contoso Lunch Delivery"
		LocationEmailAddress = $null
		"LocationType@odata.type" = "#microsoft.graph.locationType"
		LocationType = $null
		LocationUri = $null
		UniqueId = $null
		"UniqueIdType@odata.type" = "#microsoft.graph.locationUniqueIdType"
		UniqueIdType = $null
	}
	DefaultPrice = 10
	"DefaultPriceType@odata.type" = "#microsoft.graph.bookingPriceType"
	DefaultPriceType = "fixedPrice"
	"DefaultReminders@odata.type" = "#Collection(microsoft.graph.bookingReminder)"
	DefaultReminders = @(
		@{
			"@odata.type" = "#microsoft.graph.bookingReminder"
			Message = "Please be reminded that this service is tomorrow."
			Offset = "P1D"
			"Recipients@odata.type" = "#microsoft.graph.bookingReminderRecipients"
			Recipients = "allAttendees"
		}
	)
	Description = "Individual bento box lunch delivery"
	DisplayName = "Bento"
	IsLocationOnline = $true
	SmsNotificationsEnabled = $true
	LanguageTag = "en-US"
	IsHiddenFromCustomers = $false
	Notes = "Home-cooked special"
	PostBuffer = "PT10M"
	PreBuffer = "PT5M"
	SchedulingPolicy = @{
		"@odata.type" = "#microsoft.graph.bookingSchedulingPolicy"
		AllowStaffSelection = $true
		MaximumAdvance = "P10D"
		MinimumLeadTime = "PT10H"
		SendConfirmationsToOwner = $true
		TimeSlotInterval = "PT1H"
	}
	"StaffMemberIds@odata.type" = "#Collection(String)"
	StaffMemberIds = @(
		"d90d1e8c-5cfe-48cf-a2d5-966267375b6a"
		"2f5f8794-0b29-45b5-b56a-2eb5ff7aa880"
	)
	IsAnonymousJoinEnabled = $false
}
New-MgBetaBookingBusinessService -BookingBusinessId $bookingBusinessId -BodyParameter $params
```
This example shows how to use the New-MgBetaBookingBusinessService Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalInformation
Additional information that is sent to the customer when an appointment is confirmed.

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
Represents a particular service offered by a booking business.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphBookingService
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -BookingBusinessId
The unique identifier of bookingBusiness

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

### -CustomQuestions
Contains the set of custom questions associated with a particular service.
To construct, see NOTES section for CUSTOMQUESTIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphBookingQuestionAssignment[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DefaultDuration
The default length of the service, represented in numbers of days, hours, minutes, and seconds.
For example, P11D23H59M59.999999999999S.

```yaml
Type: TimeSpan
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DefaultLocation
location
To construct, see NOTES section for DEFAULTLOCATION properties and create a hash table.

```yaml
Type: IMicrosoftGraphLocation
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DefaultPrice
The default monetary price for the service.

```yaml
Type: Double
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -DefaultPriceType
Represents the type of pricing of a booking service.

```yaml
Type: BookingPriceType
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DefaultReminders
The default set of reminders for an appointment of this service.
The value of this property is available only when reading this bookingService by its ID.
To construct, see NOTES section for DEFAULTREMINDERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphBookingReminder[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
A text description for the service.

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

### -DisplayName
A name for the derived entity, which interfaces with customers.

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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IBookingsIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IsAnonymousJoinEnabled
True if an anonymousJoinWebUrl(webrtcUrl) will be generated for the appointment booked for this service.

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

### -IsHiddenFromCustomers
True means this service isn't available to customers for booking.

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

### -IsLocationOnline
True indicates that the appointments for the service will be held online.
Default value is false.

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

### -LanguageTag
The language of the self service booking page.

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

### -MaximumAttendeesCount
The maximum number of customers allowed in a service.
If maximumAttendeesCount of the service is greater than 1, pass valid customer IDs while creating or updating an appointment.
To create a customer, use the Create bookingCustomer operation.

```yaml
Type: Int32
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Notes
Additional information about this service.

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

### -PostBuffer
The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.

```yaml
Type: TimeSpan
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PreBuffer
The time to buffer before an appointment for this service can start.

```yaml
Type: TimeSpan
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SchedulingPolicy
This type represents the set of policies that dictate how bookings can be created in a Booking Calendar.
To construct, see NOTES section for SCHEDULINGPOLICY properties and create a hash table.

```yaml
Type: IMicrosoftGraphBookingSchedulingPolicy
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SmsNotificationsEnabled
True indicates SMS notifications can be sent to the customers for the appointment of the service.
Default value is false.

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

### -StaffMemberIds
Represents those staff members who provide this service.

```yaml
Type: String[]
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

### Microsoft.Graph.Beta.PowerShell.Models.IBookingsIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphBookingService
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphBookingService
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphBookingService\>: Represents a particular service offered by a booking business.
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[DisplayName \<String\>\]: A name for the derived entity, which interfaces with customers.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[AdditionalInformation \<String\>\]: Additional information that is sent to the customer when an appointment is confirmed.
  \[CustomQuestions \<IMicrosoftGraphBookingQuestionAssignment\[\]\>\]: Contains the set of custom questions associated with a particular service.
    \[IsRequired \<Boolean?\>\]: Indicates whether it's mandatory to answer the custom question.
    \[QuestionId \<String\>\]: If it's mandatory to answer the custom question.
  \[DefaultDuration \<TimeSpan?\>\]: The default length of the service, represented in numbers of days, hours, minutes, and seconds.
For example, P11D23H59M59.999999999999S.
  \[DefaultLocation \<IMicrosoftGraphLocation\>\]: location
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Address \<IMicrosoftGraphPhysicalAddress\>\]: physicalAddress
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[City \<String\>\]: The city.
      \[CountryOrRegion \<String\>\]: The country or region.
It's a free-format string value, for example, 'United States'.
      \[PostOfficeBox \<String\>\]: The post office box number.
      \[PostalCode \<String\>\]: The postal code.
      \[State \<String\>\]: The state.
      \[Street \<String\>\]: The street.
      \[Type \<String\>\]: physicalAddressType
    \[Coordinates \<IMicrosoftGraphOutlookGeoCoordinates\>\]: outlookGeoCoordinates
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Accuracy \<Double?\>\]: The accuracy of the latitude and longitude.
As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.
      \[Altitude \<Double?\>\]: The altitude of the location.
      \[AltitudeAccuracy \<Double?\>\]: The accuracy of the altitude.
      \[Latitude \<Double?\>\]: The latitude of the location.
      \[Longitude \<Double?\>\]: The longitude of the location.
    \[DisplayName \<String\>\]: The name associated with the location.
    \[LocationEmailAddress \<String\>\]: Optional email address of the location.
    \[LocationType \<String\>\]: locationType
    \[LocationUri \<String\>\]: Optional URI representing the location.
    \[UniqueId \<String\>\]: For internal use only.
    \[UniqueIdType \<String\>\]: locationUniqueIdType
  \[DefaultPrice \<Double?\>\]: The default monetary price for the service.
  \[DefaultPriceType \<BookingPriceType?\>\]: Represents the type of pricing of a booking service.
  \[DefaultReminders \<IMicrosoftGraphBookingReminder\[\]\>\]: The default set of reminders for an appointment of this service.
The value of this property is available only when reading this bookingService by its ID.
    \[Message \<String\>\]: The message in the reminder.
    \[Offset \<TimeSpan?\>\]: The amount of time before the start of an appointment that the reminder should be sent.
It's denoted in ISO 8601 format.
    \[Recipients \<String\>\]: bookingReminderRecipients
  \[Description \<String\>\]: A text description for the service.
  \[IsAnonymousJoinEnabled \<Boolean?\>\]: True if an anonymousJoinWebUrl(webrtcUrl) will be generated for the appointment booked for this service.
  \[IsHiddenFromCustomers \<Boolean?\>\]: True means this service isn't available to customers for booking.
  \[IsLocationOnline \<Boolean?\>\]: True indicates that the appointments for the service will be held online.
Default value is false.
  \[LanguageTag \<String\>\]: The language of the self service booking page.
  \[MaximumAttendeesCount \<Int32?\>\]: The maximum number of customers allowed in a service.
If maximumAttendeesCount of the service is greater than 1, pass valid customer IDs while creating or updating an appointment. 
To create a customer, use the Create bookingCustomer operation.
  \[Notes \<String\>\]: Additional information about this service.
  \[PostBuffer \<TimeSpan?\>\]: The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.
  \[PreBuffer \<TimeSpan?\>\]: The time to buffer before an appointment for this service can start.
  \[SchedulingPolicy \<IMicrosoftGraphBookingSchedulingPolicy\>\]: This type represents the set of policies that dictate how bookings can be created in a Booking Calendar.
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[AllowStaffSelection \<Boolean?\>\]: True if to allow customers to choose a specific person for the booking.
    \[MaximumAdvance \<TimeSpan?\>\]: Maximum number of days in advance that a booking can be made.
It follows the ISO 8601 format.
    \[MinimumLeadTime \<TimeSpan?\>\]: The minimum amount of time before which bookings and cancellations must be made.
It follows the ISO 8601 format.
    \[SendConfirmationsToOwner \<Boolean?\>\]: True to notify the business via email when a booking is created or changed.
Use the email address specified in the email property of the bookingBusiness entity for the business.
    \[TimeSlotInterval \<TimeSpan?\>\]: Duration of each time slot, denoted in ISO 8601 format.
  \[SmsNotificationsEnabled \<Boolean?\>\]: True indicates SMS notifications can be sent to the customers for the appointment of the service.
Default value is false.
  \[StaffMemberIds \<String\[\]\>\]: Represents those staff members who provide this service.

CUSTOMQUESTIONS \<IMicrosoftGraphBookingQuestionAssignment\[\]\>: Contains the set of custom questions associated with a particular service.
  \[IsRequired \<Boolean?\>\]: Indicates whether it's mandatory to answer the custom question.
  \[QuestionId \<String\>\]: If it's mandatory to answer the custom question.

DEFAULTLOCATION \<IMicrosoftGraphLocation\>: location
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Address \<IMicrosoftGraphPhysicalAddress\>\]: physicalAddress
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[City \<String\>\]: The city.
    \[CountryOrRegion \<String\>\]: The country or region.
It's a free-format string value, for example, 'United States'.
    \[PostOfficeBox \<String\>\]: The post office box number.
    \[PostalCode \<String\>\]: The postal code.
    \[State \<String\>\]: The state.
    \[Street \<String\>\]: The street.
    \[Type \<String\>\]: physicalAddressType
  \[Coordinates \<IMicrosoftGraphOutlookGeoCoordinates\>\]: outlookGeoCoordinates
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Accuracy \<Double?\>\]: The accuracy of the latitude and longitude.
As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.
    \[Altitude \<Double?\>\]: The altitude of the location.
    \[AltitudeAccuracy \<Double?\>\]: The accuracy of the altitude.
    \[Latitude \<Double?\>\]: The latitude of the location.
    \[Longitude \<Double?\>\]: The longitude of the location.
  \[DisplayName \<String\>\]: The name associated with the location.
  \[LocationEmailAddress \<String\>\]: Optional email address of the location.
  \[LocationType \<String\>\]: locationType
  \[LocationUri \<String\>\]: Optional URI representing the location.
  \[UniqueId \<String\>\]: For internal use only.
  \[UniqueIdType \<String\>\]: locationUniqueIdType

DEFAULTREMINDERS \<IMicrosoftGraphBookingReminder\[\]\>: The default set of reminders for an appointment of this service.
The value of this property is available only when reading this bookingService by its ID.
  \[Message \<String\>\]: The message in the reminder.
  \[Offset \<TimeSpan?\>\]: The amount of time before the start of an appointment that the reminder should be sent.
It's denoted in ISO 8601 format.
  \[Recipients \<String\>\]: bookingReminderRecipients

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

SCHEDULINGPOLICY \<IMicrosoftGraphBookingSchedulingPolicy\>: This type represents the set of policies that dictate how bookings can be created in a Booking Calendar.
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[AllowStaffSelection \<Boolean?\>\]: True if to allow customers to choose a specific person for the booking.
  \[MaximumAdvance \<TimeSpan?\>\]: Maximum number of days in advance that a booking can be made.
It follows the ISO 8601 format.
  \[MinimumLeadTime \<TimeSpan?\>\]: The minimum amount of time before which bookings and cancellations must be made.
It follows the ISO 8601 format.
  \[SendConfirmationsToOwner \<Boolean?\>\]: True to notify the business via email when a booking is created or changed.
Use the email address specified in the email property of the bookingBusiness entity for the business.
  \[TimeSlotInterval \<TimeSpan?\>\]: Duration of each time slot, denoted in ISO 8601 format.

## RELATED LINKS
[New-MgBookingBusinessService](/powershell/module/Microsoft.Graph.Bookings/New-MgBookingBusinessService?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.bookings/new-mgbetabookingbusinessservice](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.bookings/new-mgbetabookingbusinessservice)

