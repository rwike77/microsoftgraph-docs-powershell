---
external help file: Microsoft.Graph.Bookings-help.xml
Module Name: Microsoft.Graph.Bookings
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.bookings/get-mgbookingbusinessstaffavailability
schema: 2.0.0
ms.prod: bookings
---

# Get-MgBookingBusinessStaffAvailability

## SYNOPSIS
Get the availability information of staff members of a Microsoft Bookings calendar.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the beta release of this cmdlet, view [Get-MgBetaBookingBusinessStaffAvailability](/powershell/module/Microsoft.Graph.Beta.Bookings/Get-MgBetaBookingBusinessStaffAvailability?view=graph-powershell-beta)

## SYNTAX

### GetExpanded (Default)
```
Get-MgBookingBusinessStaffAvailability -BookingBusinessId <String> [-AdditionalProperties <Hashtable>]
 [-EndDateTime <IMicrosoftGraphDateTimeZone>] [-StaffIds <String[]>]
 [-StartDateTime <IMicrosoftGraphDateTimeZone>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Get
```
Get-MgBookingBusinessStaffAvailability -BookingBusinessId <String>
 -BodyParameter <IPaths1U5Iok1SolutionsBookingbusinessesBookingbusinessIdMicrosoftGraphGetstaffavailabilityPostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### GetViaIdentityExpanded
```
Get-MgBookingBusinessStaffAvailability -InputObject <IBookingsIdentity> [-AdditionalProperties <Hashtable>]
 [-EndDateTime <IMicrosoftGraphDateTimeZone>] [-StaffIds <String[]>]
 [-StartDateTime <IMicrosoftGraphDateTimeZone>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgBookingBusinessStaffAvailability -InputObject <IBookingsIdentity>
 -BodyParameter <IPaths1U5Iok1SolutionsBookingbusinessesBookingbusinessIdMicrosoftGraphGetstaffavailabilityPostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Get the availability information of staff members of a Microsoft Bookings calendar.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Bookings

$params = @{
	staffIds = @(
		"311a5454-08b2-4560-ba1c-f715e938cb79"
	)
	startDateTime = @{
		dateTime = "2022-01-25T00:00:00"
		timeZone = "India Standard Time"
	}
	endDateTime = @{
		dateTime = "2022-01-26T17:00:00"
		timeZone = "Pacific Standard Time"
	}
}

Get-MgBookingBusinessStaffAvailability -BookingBusinessId $bookingBusinessId -BodyParameter $params

```
This example shows how to use the Get-MgBookingBusinessStaffAvailability Cmdlet.


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: GetExpanded, GetViaIdentityExpanded
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
Type: IPaths1U5Iok1SolutionsBookingbusinessesBookingbusinessIdMicrosoftGraphGetstaffavailabilityPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Get, GetViaIdentity
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
Parameter Sets: GetExpanded, Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EndDateTime
dateTimeTimeZone
To construct, see NOTES section for ENDDATETIME properties and create a hash table.

```yaml
Type: IMicrosoftGraphDateTimeZone
Parameter Sets: GetExpanded, GetViaIdentityExpanded
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
Parameter Sets: GetViaIdentityExpanded, GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -StaffIds
.

```yaml
Type: String[]
Parameter Sets: GetExpanded, GetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StartDateTime
dateTimeTimeZone
To construct, see NOTES section for STARTDATETIME properties and create a hash table.

```yaml
Type: IMicrosoftGraphDateTimeZone
Parameter Sets: GetExpanded, GetViaIdentityExpanded
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

### Microsoft.Graph.PowerShell.Models.IBookingsIdentity
### Microsoft.Graph.PowerShell.Models.IPaths1U5Iok1SolutionsBookingbusinessesBookingbusinessIdMicrosoftGraphGetstaffavailabilityPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphStaffAvailabilityItem
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IPaths1U5Iok1SolutionsBookingbusinessesBookingbusinessIdMicrosoftGraphGetstaffavailabilityPostRequestbodyContentApplicationJsonSchema\>: .
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[EndDateTime \<IMicrosoftGraphDateTimeZone\>\]: dateTimeTimeZone
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[DateTime \<String\>\]: A single point of time in a combined date and time representation ({date}T{time}; for example, 2017-08-29T04:00:00.0000000).
    \[TimeZone \<String\>\]: Represents a time zone, for example, 'Pacific Standard Time'.
See below for more possible values.
  \[StaffIds \<String\[\]\>\]: 
  \[StartDateTime \<IMicrosoftGraphDateTimeZone\>\]: dateTimeTimeZone

ENDDATETIME \<IMicrosoftGraphDateTimeZone\>: dateTimeTimeZone
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[DateTime \<String\>\]: A single point of time in a combined date and time representation ({date}T{time}; for example, 2017-08-29T04:00:00.0000000).
  \[TimeZone \<String\>\]: Represents a time zone, for example, 'Pacific Standard Time'.
See below for more possible values.

INPUTOBJECT \<IBookingsIdentity\>: Identity Parameter
  \[BookingAppointmentId \<String\>\]: The unique identifier of bookingAppointment
  \[BookingBusinessId \<String\>\]: The unique identifier of bookingBusiness
  \[BookingCurrencyId \<String\>\]: The unique identifier of bookingCurrency
  \[BookingCustomQuestionId \<String\>\]: The unique identifier of bookingCustomQuestion
  \[BookingCustomerBaseId \<String\>\]: The unique identifier of bookingCustomerBase
  \[BookingServiceId \<String\>\]: The unique identifier of bookingService
  \[BookingStaffMemberBaseId \<String\>\]: The unique identifier of bookingStaffMemberBase

STARTDATETIME \<IMicrosoftGraphDateTimeZone\>: dateTimeTimeZone
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[DateTime \<String\>\]: A single point of time in a combined date and time representation ({date}T{time}; for example, 2017-08-29T04:00:00.0000000).
  \[TimeZone \<String\>\]: Represents a time zone, for example, 'Pacific Standard Time'.
See below for more possible values.

## RELATED LINKS
[Get-MgBetaBookingBusinessStaffAvailability](/powershell/module/Microsoft.Graph.Beta.Bookings/Get-MgBetaBookingBusinessStaffAvailability?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.bookings/get-mgbookingbusinessstaffavailability](https://learn.microsoft.com/powershell/module/microsoft.graph.bookings/get-mgbookingbusinessstaffavailability)


