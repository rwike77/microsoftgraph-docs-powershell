---
external help file: Microsoft.Graph.Beta.Planner-help.xml
Module Name: Microsoft.Graph.Beta.Planner
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.planner/new-mgbetaplannerroster
schema: 2.0.0
ms.prod: planner
---

# New-MgBetaPlannerRoster

## SYNOPSIS
Create a new plannerRoster object.
This API is available in the following national cloud deployments.

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaPlannerRoster [-AdditionalProperties <Hashtable>] [-Id <String>]
 [-Members <IMicrosoftGraphPlannerRosterMember[]>] [-Plans <IMicrosoftGraphPlannerPlan[]>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Create
```
New-MgBetaPlannerRoster -BodyParameter <IMicrosoftGraphPlannerRoster> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new plannerRoster object.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Using the New-MgBetaPlannerRoster Cmdlet
```powershell
Import-Module Microsoft.Graph.Beta.Planner
$params = @{
	"@odata.type" = "#microsoft.graph.plannerRoster"
}
New-MgBetaPlannerRoster -BodyParameter $params
```
This example shows how to use the New-MgBetaPlannerRoster Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
plannerRoster
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphPlannerRoster
Parameter Sets: Create
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
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Members
Retrieves the members of the plannerRoster.
To construct, see NOTES section for MEMBERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphPlannerRosterMember[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Plans
Retrieves the plans contained by the plannerRoster.
To construct, see NOTES section for PLANS properties and create a hash table.

```yaml
Type: IMicrosoftGraphPlannerPlan[]
Parameter Sets: CreateExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphPlannerRoster
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphPlannerRoster
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphPlannerRoster\>: plannerRoster
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[Members \<IMicrosoftGraphPlannerRosterMember\[\]\>\]: Retrieves the members of the plannerRoster.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[Roles \<String\[\]\>\]: Additional roles associated with the PlannerRosterMember, which determines permissions of the member in the plannerRoster.
Currently there are no available roles to assign, and every member has full control over the contents of the plannerRoster.
    \[TenantId \<String\>\]: Identifier of the tenant the user belongs to.
Currently only the users from the same tenant can be added to a plannerRoster.
    \[UserId \<String\>\]: Identifier of the user.
  \[Plans \<IMicrosoftGraphPlannerPlan\[\]\>\]: Retrieves the plans contained by the plannerRoster.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[Buckets \<IMicrosoftGraphPlannerBucket\[\]\>\]: Collection of buckets in the plan.
Read-only.
Nullable.
      \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
      \[CreationSource \<IMicrosoftGraphPlannerBucketCreation\>\]: plannerBucketCreation
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[CreationSourceKind \<String\>\]: plannerCreationSourceKind
      \[Name \<String\>\]: Name of the bucket.
      \[OrderHint \<String\>\]: Hint used to order items of this type in a list view.
For details about the supported format, see Using order hints in Planner.
      \[PlanId \<String\>\]: Plan ID to which the bucket belongs.
      \[Tasks \<IMicrosoftGraphPlannerTask\[\]\>\]: Read-only.
Nullable.
The collection of tasks in the bucket.
        \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
        \[ActiveChecklistItemCount \<Int32?\>\]: Number of checklist items with value set to false, representing incomplete items.
        \[AppliedCategories \<IMicrosoftGraphPlannerAppliedCategories\>\]: plannerAppliedCategories
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[AssignedToTaskBoardFormat \<IMicrosoftGraphPlannerAssignedToTaskBoardTaskFormat\>\]: plannerAssignedToTaskBoardTaskFormat
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
          \[OrderHintsByAssignee \<IMicrosoftGraphPlannerOrderHintsByAssignee\>\]: plannerOrderHintsByAssignee
            \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[UnassignedOrderHint \<String\>\]: Hint value used to order the task on the AssignedTo view of the Task Board when the task isn't assigned to anyone, or if the orderHintsByAssignee dictionary doesn't provide an order hint for the user the task is assigned to.
The format is defined as outlined here.
        \[AssigneePriority \<String\>\]: Hint used to order items of this type in a list view.
The format is defined as outlined here.
        \[Assignments \<IMicrosoftGraphPlannerAssignments\>\]: plannerAssignments
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[BucketId \<String\>\]: Bucket ID to which the task belongs.
The bucket needs to be in the plan that the task is in.
It is 28 characters long and case-sensitive.
Format validation is done on the service.
        \[BucketTaskBoardFormat \<IMicrosoftGraphPlannerBucketTaskBoardTaskFormat\>\]: plannerBucketTaskBoardTaskFormat
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
          \[OrderHint \<String\>\]: Hint used to order tasks in the bucket view of the task board.
For details about the supported format, see Using order hints in Planner.
        \[ChecklistItemCount \<Int32?\>\]: Number of checklist items that are present on the task.
        \[CompletedBy \<IMicrosoftGraphIdentitySet\>\]: identitySet
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[Application \<IMicrosoftGraphIdentity\>\]: identity
            \[(Any) \<Object\>\]: This indicates any property can be added to this object.
            \[DisplayName \<String\>\]: The display name of the identity.
This might not always be available or up to date.
For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
            \[Id \<String\>\]: Unique identifier for the identity.
          \[Device \<IMicrosoftGraphIdentity\>\]: identity
          \[User \<IMicrosoftGraphIdentity\>\]: identity
        \[CompletedDateTime \<DateTime?\>\]: Read-only.
Date and time at which the 'percentComplete' of the task is set to '100'.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
        \[ConversationThreadId \<String\>\]: Thread ID of the conversation on the task.
This is the ID of the conversation thread object created in the group.
        \[CreatedBy \<IMicrosoftGraphIdentitySet\>\]: identitySet
        \[CreatedDateTime \<DateTime?\>\]: Read-only.
Date and time at which the task is created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
        \[CreationSource \<IMicrosoftGraphPlannerTaskCreation\>\]: plannerTaskCreation
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[CreationSourceKind \<String\>\]: plannerCreationSourceKind
          \[TeamsPublicationInfo \<IMicrosoftGraphPlannerTeamsPublicationInfo\>\]: plannerTeamsPublicationInfo
            \[(Any) \<Object\>\]: This indicates any property can be added to this object.
            \[CreationSourceKind \<String\>\]: plannerCreationSourceKind
            \[TeamsPublicationInfo \<IMicrosoftGraphPlannerTeamsPublicationInfo\>\]: plannerTeamsPublicationInfo
            \[LastModifiedDateTime \<DateTime?\>\]: The date and time when this task was last modified by the publication process.
Read-only.
            \[PublicationId \<String\>\]: The identifier of the publication.
Read-only.
            \[PublishedToPlanId \<String\>\]: The identifier of the plannerPlan this task was originally placed in.
Read-only.
            \[PublishingTeamId \<String\>\]: The identifier of the team that initiated the publication process.
Read-only.
            \[PublishingTeamName \<String\>\]: The display name of the team that initiated the publication process.
This display name is for reference only, and might not represent the most up-to-date name of the team.
Read-only.
        \[Details \<IMicrosoftGraphPlannerTaskDetails\>\]: plannerTaskDetails
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
          \[Checklist \<IMicrosoftGraphPlannerChecklistItems\>\]: plannerChecklistItems
            \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[CompletionRequirements \<IMicrosoftGraphPlannerTaskCompletionRequirementDetails\>\]: plannerTaskCompletionRequirementDetails
            \[(Any) \<Object\>\]: This indicates any property can be added to this object.
            \[ChecklistRequirement \<IMicrosoftGraphPlannerChecklistRequirement\>\]: plannerChecklistRequirement
              \[(Any) \<Object\>\]: This indicates any property can be added to this object.
              \[RequiredChecklistItemIds \<String\[\]\>\]: A collection of required plannerChecklistItems identifiers to complete the plannerTask.
          \[Description \<String\>\]: Description of the task.
          \[Notes \<IMicrosoftGraphItemBody\>\]: itemBody
            \[(Any) \<Object\>\]: This indicates any property can be added to this object.
            \[Content \<String\>\]: The content of the item.
            \[ContentType \<String\>\]: bodyType
          \[PreviewType \<String\>\]: plannerPreviewType
          \[References \<IMicrosoftGraphPlannerExternalReferences\>\]: plannerExternalReferences
            \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[DueDateTime \<DateTime?\>\]: Date and time at which the task is due.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
        \[HasDescription \<Boolean?\>\]: Read-only.
Value is true if the details object of the task has a nonempty description and false otherwise.
        \[OrderHint \<String\>\]: Hint used to order items of this type in a list view.
The format is defined as outlined here.
        \[PercentComplete \<Int32?\>\]: Percentage of task completion.
When set to 100, the task is considered completed.
        \[PlanId \<String\>\]: Plan ID to which the task belongs.
        \[PreviewType \<String\>\]: plannerPreviewType
        \[Priority \<Int32?\>\]: Priority of the task.
Valid range of values is between 0 and 10 (inclusive), with increasing value being lower priority (0 has the highest priority and 10 has the lowest priority). 
Currently, Planner interprets values 0 and 1 as 'urgent', 2 and 3 and 4 as 'important', 5, 6, and 7 as 'medium', and 8, 9, and 10 as 'low'. 
Currently, Planner sets the value 1 for 'urgent', 3 for 'important', 5 for 'medium', and 9 for 'low'.
        \[ProgressTaskBoardFormat \<IMicrosoftGraphPlannerProgressTaskBoardTaskFormat\>\]: plannerProgressTaskBoardTaskFormat
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
          \[OrderHint \<String\>\]: Hint value used to order the task on the progress view of the task board.
For details about the supported format, see Using order hints in Planner.
        \[Recurrence \<IMicrosoftGraphPlannerTaskRecurrence\>\]: plannerTaskRecurrence
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[NextInSeriesTaskId \<String\>\]: The taskId of the next task in this series.
This value is assigned at the time the next task in the series is created, and is null prior to that time.
          \[OccurrenceId \<Int32?\>\]: The 1-based index of this task within the recurrence series.
The first task in a series has the value 1, the next task in the series has the value 2, and so on.
          \[PreviousInSeriesTaskId \<String\>\]: The taskId of the previous task in this series.
null for the first task in a series since it has no predecessor.
All subsequent tasks in the series have a value that corresponds to their predecessors.
          \[RecurrenceStartDateTime \<DateTime?\>\]: The date and time when this recurrence series begin.
For the first task in a series (occurrenceId = 1) this value is copied from schedule.patternStartDateTime.
For subsequent tasks in the series (occurrenceId \>= 2) this value is copied from the previous task and never changes; it preserves the start date of the recurring series.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
          \[Schedule \<IMicrosoftGraphPlannerRecurrenceSchedule\>\]: plannerRecurrenceSchedule
            \[(Any) \<Object\>\]: This indicates any property can be added to this object.
            \[NextOccurrenceDateTime \<DateTime?\>\]: The next date for this schedule.
When a new task is instantiated to continue the recurrence series, this date is used for the dueDateTime of the new plannerTask.
Auto-generated by the service.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
            \[Pattern \<IMicrosoftGraphRecurrencePattern\>\]: recurrencePattern
              \[(Any) \<Object\>\]: This indicates any property can be added to this object.
              \[DayOfMonth \<Int32?\>\]: The day of the month on which the event occurs.
Required if type is absoluteMonthly or absoluteYearly.
              \[DaysOfWeek \<String\[\]\>\]: A collection of the days of the week on which the event occurs.
The possible values are: sunday, monday, tuesday, wednesday, thursday, friday, saturday.
If type is relativeMonthly or relativeYearly, and daysOfWeek specifies more than one day, the event falls on the first day that satisfies the pattern. 
Required if type is weekly, relativeMonthly, or relativeYearly.
              \[FirstDayOfWeek \<String\>\]: dayOfWeek
              \[Index \<String\>\]: weekIndex
              \[Interval \<Int32?\>\]: The number of units between occurrences, where units can be in days, weeks, months, or years, depending on the type.
Required.
              \[Month \<Int32?\>\]: The month in which the event occurs. 
This is a number from 1 to 12.
              \[Type \<String\>\]: recurrencePatternType
            \[PatternStartDateTime \<DateTime?\>\]: The start date for the recurrence pattern.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Required.
          \[SeriesId \<String\>\]: The recurrence series this task belongs to.
A GUID-based value that serves as the unique identifier for a series.
        \[ReferenceCount \<Int32?\>\]: Number of external references that exist on the task.
        \[SpecifiedCompletionRequirements \<String\>\]: plannerTaskCompletionRequirements
        \[StartDateTime \<DateTime?\>\]: Date and time at which the task starts.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
        \[Title \<String\>\]: Title of the task.
    \[Container \<IMicrosoftGraphPlannerPlanContainer\>\]: plannerPlanContainer
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[ContainerId \<String\>\]: The identifier of the resource that contains the plan.
Optional.
      \[Type \<String\>\]: plannerContainerType
      \[Url \<String\>\]: The full canonical URL of the container.
Optional.
    \[Contexts \<IMicrosoftGraphPlannerPlanContextCollection\>\]: plannerPlanContextCollection
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[CreatedBy \<IMicrosoftGraphIdentitySet\>\]: identitySet
    \[CreatedDateTime \<DateTime?\>\]: Read-only.
Date and time at which the plan is created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    \[CreationSource \<IMicrosoftGraphPlannerPlanCreation\>\]: plannerPlanCreation
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[CreationSourceKind \<String\>\]: plannerCreationSourceKind
    \[Details \<IMicrosoftGraphPlannerPlanDetails\>\]: plannerPlanDetails
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
      \[CategoryDescriptions \<IMicrosoftGraphPlannerCategoryDescriptions\>\]: plannerCategoryDescriptions
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[Category1 \<String\>\]: The label associated with Category 1
        \[Category10 \<String\>\]: The label associated with Category 10
        \[Category11 \<String\>\]: The label associated with Category 11
        \[Category12 \<String\>\]: The label associated with Category 12
        \[Category13 \<String\>\]: The label associated with Category 13
        \[Category14 \<String\>\]: The label associated with Category 14
        \[Category15 \<String\>\]: The label associated with Category 15
        \[Category16 \<String\>\]: The label associated with Category 16
        \[Category17 \<String\>\]: The label associated with Category 17
        \[Category18 \<String\>\]: The label associated with Category 18
        \[Category19 \<String\>\]: The label associated with Category 19
        \[Category2 \<String\>\]: The label associated with Category 2
        \[Category20 \<String\>\]: The label associated with Category 20
        \[Category21 \<String\>\]: The label associated with Category 21
        \[Category22 \<String\>\]: The label associated with Category 22
        \[Category23 \<String\>\]: The label associated with Category 23
        \[Category24 \<String\>\]: The label associated with Category 24
        \[Category25 \<String\>\]: The label associated with Category 25
        \[Category3 \<String\>\]: The label associated with Category 3
        \[Category4 \<String\>\]: The label associated with Category 4
        \[Category5 \<String\>\]: The label associated with Category 5
        \[Category6 \<String\>\]: The label associated with Category 6
        \[Category7 \<String\>\]: The label associated with Category 7
        \[Category8 \<String\>\]: The label associated with Category 8
        \[Category9 \<String\>\]: The label associated with Category 9
      \[ContextDetails \<IMicrosoftGraphPlannerPlanContextDetailsCollection\>\]: plannerPlanContextDetailsCollection
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[SharedWith \<IMicrosoftGraphPlannerUserIds\>\]: plannerUserIds
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Owner \<String\>\]: 
    \[SharedWithContainers \<IMicrosoftGraphPlannerSharedWithContainer\[\]\>\]: List of containers the plan is shared with.
      \[ContainerId \<String\>\]: The identifier of the resource that contains the plan.
Optional.
      \[Type \<String\>\]: plannerContainerType
      \[Url \<String\>\]: The full canonical URL of the container.
Optional.
      \[AccessLevel \<String\>\]: plannerPlanAccessLevel
    \[Tasks \<IMicrosoftGraphPlannerTask\[\]\>\]: Collection of tasks in the plan.
Read-only.
Nullable.
    \[Title \<String\>\]: Required.
Title of the plan.

MEMBERS \<IMicrosoftGraphPlannerRosterMember\[\]\>: Retrieves the members of the plannerRoster.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[Roles \<String\[\]\>\]: Additional roles associated with the PlannerRosterMember, which determines permissions of the member in the plannerRoster.
Currently there are no available roles to assign, and every member has full control over the contents of the plannerRoster.
  \[TenantId \<String\>\]: Identifier of the tenant the user belongs to.
Currently only the users from the same tenant can be added to a plannerRoster.
  \[UserId \<String\>\]: Identifier of the user.

PLANS \<IMicrosoftGraphPlannerPlan\[\]\>: Retrieves the plans contained by the plannerRoster.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[Buckets \<IMicrosoftGraphPlannerBucket\[\]\>\]: Collection of buckets in the plan.
Read-only.
Nullable.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[CreationSource \<IMicrosoftGraphPlannerBucketCreation\>\]: plannerBucketCreation
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[CreationSourceKind \<String\>\]: plannerCreationSourceKind
    \[Name \<String\>\]: Name of the bucket.
    \[OrderHint \<String\>\]: Hint used to order items of this type in a list view.
For details about the supported format, see Using order hints in Planner.
    \[PlanId \<String\>\]: Plan ID to which the bucket belongs.
    \[Tasks \<IMicrosoftGraphPlannerTask\[\]\>\]: Read-only.
Nullable.
The collection of tasks in the bucket.
      \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
      \[ActiveChecklistItemCount \<Int32?\>\]: Number of checklist items with value set to false, representing incomplete items.
      \[AppliedCategories \<IMicrosoftGraphPlannerAppliedCategories\>\]: plannerAppliedCategories
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[AssignedToTaskBoardFormat \<IMicrosoftGraphPlannerAssignedToTaskBoardTaskFormat\>\]: plannerAssignedToTaskBoardTaskFormat
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
        \[OrderHintsByAssignee \<IMicrosoftGraphPlannerOrderHintsByAssignee\>\]: plannerOrderHintsByAssignee
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[UnassignedOrderHint \<String\>\]: Hint value used to order the task on the AssignedTo view of the Task Board when the task isn't assigned to anyone, or if the orderHintsByAssignee dictionary doesn't provide an order hint for the user the task is assigned to.
The format is defined as outlined here.
      \[AssigneePriority \<String\>\]: Hint used to order items of this type in a list view.
The format is defined as outlined here.
      \[Assignments \<IMicrosoftGraphPlannerAssignments\>\]: plannerAssignments
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[BucketId \<String\>\]: Bucket ID to which the task belongs.
The bucket needs to be in the plan that the task is in.
It is 28 characters long and case-sensitive.
Format validation is done on the service.
      \[BucketTaskBoardFormat \<IMicrosoftGraphPlannerBucketTaskBoardTaskFormat\>\]: plannerBucketTaskBoardTaskFormat
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
        \[OrderHint \<String\>\]: Hint used to order tasks in the bucket view of the task board.
For details about the supported format, see Using order hints in Planner.
      \[ChecklistItemCount \<Int32?\>\]: Number of checklist items that are present on the task.
      \[CompletedBy \<IMicrosoftGraphIdentitySet\>\]: identitySet
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[Application \<IMicrosoftGraphIdentity\>\]: identity
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[DisplayName \<String\>\]: The display name of the identity.
This might not always be available or up to date.
For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
          \[Id \<String\>\]: Unique identifier for the identity.
        \[Device \<IMicrosoftGraphIdentity\>\]: identity
        \[User \<IMicrosoftGraphIdentity\>\]: identity
      \[CompletedDateTime \<DateTime?\>\]: Read-only.
Date and time at which the 'percentComplete' of the task is set to '100'.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      \[ConversationThreadId \<String\>\]: Thread ID of the conversation on the task.
This is the ID of the conversation thread object created in the group.
      \[CreatedBy \<IMicrosoftGraphIdentitySet\>\]: identitySet
      \[CreatedDateTime \<DateTime?\>\]: Read-only.
Date and time at which the task is created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      \[CreationSource \<IMicrosoftGraphPlannerTaskCreation\>\]: plannerTaskCreation
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[CreationSourceKind \<String\>\]: plannerCreationSourceKind
        \[TeamsPublicationInfo \<IMicrosoftGraphPlannerTeamsPublicationInfo\>\]: plannerTeamsPublicationInfo
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[CreationSourceKind \<String\>\]: plannerCreationSourceKind
          \[TeamsPublicationInfo \<IMicrosoftGraphPlannerTeamsPublicationInfo\>\]: plannerTeamsPublicationInfo
          \[LastModifiedDateTime \<DateTime?\>\]: The date and time when this task was last modified by the publication process.
Read-only.
          \[PublicationId \<String\>\]: The identifier of the publication.
Read-only.
          \[PublishedToPlanId \<String\>\]: The identifier of the plannerPlan this task was originally placed in.
Read-only.
          \[PublishingTeamId \<String\>\]: The identifier of the team that initiated the publication process.
Read-only.
          \[PublishingTeamName \<String\>\]: The display name of the team that initiated the publication process.
This display name is for reference only, and might not represent the most up-to-date name of the team.
Read-only.
      \[Details \<IMicrosoftGraphPlannerTaskDetails\>\]: plannerTaskDetails
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
        \[Checklist \<IMicrosoftGraphPlannerChecklistItems\>\]: plannerChecklistItems
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[CompletionRequirements \<IMicrosoftGraphPlannerTaskCompletionRequirementDetails\>\]: plannerTaskCompletionRequirementDetails
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[ChecklistRequirement \<IMicrosoftGraphPlannerChecklistRequirement\>\]: plannerChecklistRequirement
            \[(Any) \<Object\>\]: This indicates any property can be added to this object.
            \[RequiredChecklistItemIds \<String\[\]\>\]: A collection of required plannerChecklistItems identifiers to complete the plannerTask.
        \[Description \<String\>\]: Description of the task.
        \[Notes \<IMicrosoftGraphItemBody\>\]: itemBody
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[Content \<String\>\]: The content of the item.
          \[ContentType \<String\>\]: bodyType
        \[PreviewType \<String\>\]: plannerPreviewType
        \[References \<IMicrosoftGraphPlannerExternalReferences\>\]: plannerExternalReferences
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[DueDateTime \<DateTime?\>\]: Date and time at which the task is due.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      \[HasDescription \<Boolean?\>\]: Read-only.
Value is true if the details object of the task has a nonempty description and false otherwise.
      \[OrderHint \<String\>\]: Hint used to order items of this type in a list view.
The format is defined as outlined here.
      \[PercentComplete \<Int32?\>\]: Percentage of task completion.
When set to 100, the task is considered completed.
      \[PlanId \<String\>\]: Plan ID to which the task belongs.
      \[PreviewType \<String\>\]: plannerPreviewType
      \[Priority \<Int32?\>\]: Priority of the task.
Valid range of values is between 0 and 10 (inclusive), with increasing value being lower priority (0 has the highest priority and 10 has the lowest priority). 
Currently, Planner interprets values 0 and 1 as 'urgent', 2 and 3 and 4 as 'important', 5, 6, and 7 as 'medium', and 8, 9, and 10 as 'low'. 
Currently, Planner sets the value 1 for 'urgent', 3 for 'important', 5 for 'medium', and 9 for 'low'.
      \[ProgressTaskBoardFormat \<IMicrosoftGraphPlannerProgressTaskBoardTaskFormat\>\]: plannerProgressTaskBoardTaskFormat
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
        \[OrderHint \<String\>\]: Hint value used to order the task on the progress view of the task board.
For details about the supported format, see Using order hints in Planner.
      \[Recurrence \<IMicrosoftGraphPlannerTaskRecurrence\>\]: plannerTaskRecurrence
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[NextInSeriesTaskId \<String\>\]: The taskId of the next task in this series.
This value is assigned at the time the next task in the series is created, and is null prior to that time.
        \[OccurrenceId \<Int32?\>\]: The 1-based index of this task within the recurrence series.
The first task in a series has the value 1, the next task in the series has the value 2, and so on.
        \[PreviousInSeriesTaskId \<String\>\]: The taskId of the previous task in this series.
null for the first task in a series since it has no predecessor.
All subsequent tasks in the series have a value that corresponds to their predecessors.
        \[RecurrenceStartDateTime \<DateTime?\>\]: The date and time when this recurrence series begin.
For the first task in a series (occurrenceId = 1) this value is copied from schedule.patternStartDateTime.
For subsequent tasks in the series (occurrenceId \>= 2) this value is copied from the previous task and never changes; it preserves the start date of the recurring series.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
        \[Schedule \<IMicrosoftGraphPlannerRecurrenceSchedule\>\]: plannerRecurrenceSchedule
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[NextOccurrenceDateTime \<DateTime?\>\]: The next date for this schedule.
When a new task is instantiated to continue the recurrence series, this date is used for the dueDateTime of the new plannerTask.
Auto-generated by the service.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
          \[Pattern \<IMicrosoftGraphRecurrencePattern\>\]: recurrencePattern
            \[(Any) \<Object\>\]: This indicates any property can be added to this object.
            \[DayOfMonth \<Int32?\>\]: The day of the month on which the event occurs.
Required if type is absoluteMonthly or absoluteYearly.
            \[DaysOfWeek \<String\[\]\>\]: A collection of the days of the week on which the event occurs.
The possible values are: sunday, monday, tuesday, wednesday, thursday, friday, saturday.
If type is relativeMonthly or relativeYearly, and daysOfWeek specifies more than one day, the event falls on the first day that satisfies the pattern. 
Required if type is weekly, relativeMonthly, or relativeYearly.
            \[FirstDayOfWeek \<String\>\]: dayOfWeek
            \[Index \<String\>\]: weekIndex
            \[Interval \<Int32?\>\]: The number of units between occurrences, where units can be in days, weeks, months, or years, depending on the type.
Required.
            \[Month \<Int32?\>\]: The month in which the event occurs. 
This is a number from 1 to 12.
            \[Type \<String\>\]: recurrencePatternType
          \[PatternStartDateTime \<DateTime?\>\]: The start date for the recurrence pattern.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Required.
        \[SeriesId \<String\>\]: The recurrence series this task belongs to.
A GUID-based value that serves as the unique identifier for a series.
      \[ReferenceCount \<Int32?\>\]: Number of external references that exist on the task.
      \[SpecifiedCompletionRequirements \<String\>\]: plannerTaskCompletionRequirements
      \[StartDateTime \<DateTime?\>\]: Date and time at which the task starts.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      \[Title \<String\>\]: Title of the task.
  \[Container \<IMicrosoftGraphPlannerPlanContainer\>\]: plannerPlanContainer
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[ContainerId \<String\>\]: The identifier of the resource that contains the plan.
Optional.
    \[Type \<String\>\]: plannerContainerType
    \[Url \<String\>\]: The full canonical URL of the container.
Optional.
  \[Contexts \<IMicrosoftGraphPlannerPlanContextCollection\>\]: plannerPlanContextCollection
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[CreatedBy \<IMicrosoftGraphIdentitySet\>\]: identitySet
  \[CreatedDateTime \<DateTime?\>\]: Read-only.
Date and time at which the plan is created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  \[CreationSource \<IMicrosoftGraphPlannerPlanCreation\>\]: plannerPlanCreation
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[CreationSourceKind \<String\>\]: plannerCreationSourceKind
  \[Details \<IMicrosoftGraphPlannerPlanDetails\>\]: plannerPlanDetails
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[CategoryDescriptions \<IMicrosoftGraphPlannerCategoryDescriptions\>\]: plannerCategoryDescriptions
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Category1 \<String\>\]: The label associated with Category 1
      \[Category10 \<String\>\]: The label associated with Category 10
      \[Category11 \<String\>\]: The label associated with Category 11
      \[Category12 \<String\>\]: The label associated with Category 12
      \[Category13 \<String\>\]: The label associated with Category 13
      \[Category14 \<String\>\]: The label associated with Category 14
      \[Category15 \<String\>\]: The label associated with Category 15
      \[Category16 \<String\>\]: The label associated with Category 16
      \[Category17 \<String\>\]: The label associated with Category 17
      \[Category18 \<String\>\]: The label associated with Category 18
      \[Category19 \<String\>\]: The label associated with Category 19
      \[Category2 \<String\>\]: The label associated with Category 2
      \[Category20 \<String\>\]: The label associated with Category 20
      \[Category21 \<String\>\]: The label associated with Category 21
      \[Category22 \<String\>\]: The label associated with Category 22
      \[Category23 \<String\>\]: The label associated with Category 23
      \[Category24 \<String\>\]: The label associated with Category 24
      \[Category25 \<String\>\]: The label associated with Category 25
      \[Category3 \<String\>\]: The label associated with Category 3
      \[Category4 \<String\>\]: The label associated with Category 4
      \[Category5 \<String\>\]: The label associated with Category 5
      \[Category6 \<String\>\]: The label associated with Category 6
      \[Category7 \<String\>\]: The label associated with Category 7
      \[Category8 \<String\>\]: The label associated with Category 8
      \[Category9 \<String\>\]: The label associated with Category 9
    \[ContextDetails \<IMicrosoftGraphPlannerPlanContextDetailsCollection\>\]: plannerPlanContextDetailsCollection
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[SharedWith \<IMicrosoftGraphPlannerUserIds\>\]: plannerUserIds
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Owner \<String\>\]: 
  \[SharedWithContainers \<IMicrosoftGraphPlannerSharedWithContainer\[\]\>\]: List of containers the plan is shared with.
    \[ContainerId \<String\>\]: The identifier of the resource that contains the plan.
Optional.
    \[Type \<String\>\]: plannerContainerType
    \[Url \<String\>\]: The full canonical URL of the container.
Optional.
    \[AccessLevel \<String\>\]: plannerPlanAccessLevel
  \[Tasks \<IMicrosoftGraphPlannerTask\[\]\>\]: Collection of tasks in the plan.
Read-only.
Nullable.
  \[Title \<String\>\]: Required.
Title of the plan.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.planner/new-mgbetaplannerroster](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.planner/new-mgbetaplannerroster)

