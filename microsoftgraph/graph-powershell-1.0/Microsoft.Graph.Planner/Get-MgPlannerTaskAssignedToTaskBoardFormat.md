---
external help file: Microsoft.Graph.Planner-help.xml
Module Name: Microsoft.Graph.Planner
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.planner/get-mgplannertaskassignedtotaskboardformat
schema: 2.0.0
ms.prod: planner
---

# Get-MgPlannerTaskAssignedToTaskBoardFormat

## SYNOPSIS
Retrieve the properties and relationships of a plannerAssignedToTaskBoardTaskFormat object.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the beta release of this cmdlet, view [Get-MgBetaPlannerTaskAssignedToTaskBoardFormat](/powershell/module/Microsoft.Graph.Beta.Planner/Get-MgBetaPlannerTaskAssignedToTaskBoardFormat?view=graph-powershell-beta)

## SYNTAX

### Get (Default)
```
Get-MgPlannerTaskAssignedToTaskBoardFormat -PlannerTaskId <String> [-ExpandProperty <String[]>]
 [-Property <String[]>] [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgPlannerTaskAssignedToTaskBoardFormat -InputObject <IPlannerIdentity> [-ExpandProperty <String[]>]
 [-Property <String[]>] [<CommonParameters>]
```

## DESCRIPTION
Retrieve the properties and relationships of a plannerAssignedToTaskBoardTaskFormat object.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Planner

Get-MgPlannerTaskAssignedToTaskBoardFormat -PlannerTaskId $plannerTaskId

```
This example shows how to use the Get-MgPlannerTaskAssignedToTaskBoardFormat Cmdlet.


## PARAMETERS

### -ExpandProperty
Expand related entities

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Expand

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
Type: IPlannerIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PlannerTaskId
The unique identifier of plannerTask

```yaml
Type: String
Parameter Sets: Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Property
Select properties to be returned

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Select

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IPlannerIdentity
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphPlannerAssignedToTaskBoardTaskFormat
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT \<IPlannerIdentity\>: Identity Parameter
  \[GroupId \<String\>\]: The unique identifier of group
  \[PlannerBucketId \<String\>\]: The unique identifier of plannerBucket
  \[PlannerPlanId \<String\>\]: The unique identifier of plannerPlan
  \[PlannerTaskId \<String\>\]: The unique identifier of plannerTask
  \[UserId \<String\>\]: The unique identifier of user

## RELATED LINKS
[Get-MgBetaPlannerTaskAssignedToTaskBoardFormat](/powershell/module/Microsoft.Graph.Beta.Planner/Get-MgBetaPlannerTaskAssignedToTaskBoardFormat?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.planner/get-mgplannertaskassignedtotaskboardformat](https://learn.microsoft.com/powershell/module/microsoft.graph.planner/get-mgplannertaskassignedtotaskboardformat)


