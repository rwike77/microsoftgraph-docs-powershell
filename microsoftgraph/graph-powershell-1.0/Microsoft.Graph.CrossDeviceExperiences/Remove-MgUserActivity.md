---
external help file: Microsoft.Graph.CrossDeviceExperiences-help.xml
Module Name: Microsoft.Graph.CrossDeviceExperiences
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.crossdeviceexperiences/remove-mguseractivity
schema: 2.0.0
ms.prod: project-rome
---

# Remove-MgUserActivity

## SYNOPSIS
Delete an existing user activity for your app.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the beta release of this cmdlet, view [Remove-MgBetaUserActivity](/powershell/module/Microsoft.Graph.Beta.CrossDeviceExperiences/Remove-MgBetaUserActivity?view=graph-powershell-beta)

## SYNTAX

### Delete (Default)
```
Remove-MgUserActivity -UserActivityId <String> -UserId <String> [-IfMatch <String>] [-PassThru] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### DeleteViaIdentity
```
Remove-MgUserActivity -InputObject <ICrossDeviceExperiencesIdentity> [-IfMatch <String>] [-PassThru] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Delete an existing user activity for your app.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Code snippet

```powershell
Import-Module Microsoft.Graph.CrossDeviceExperiences

# A UPN can also be used as -UserId.
Remove-MgUserActivity -UserId $userId -UserActivityId $userActivityId
```
This example shows how to use the Remove-MgUserActivity Cmdlet.

To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).


## PARAMETERS

### -IfMatch
ETag

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
Type: ICrossDeviceExperiencesIdentity
Parameter Sets: DeleteViaIdentity
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

### -UserActivityId
The unique identifier of userActivity

```yaml
Type: String
Parameter Sets: Delete
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserId
The unique identifier of user

```yaml
Type: String
Parameter Sets: Delete
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

### Microsoft.Graph.PowerShell.Models.ICrossDeviceExperiencesIdentity
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT \<ICrossDeviceExperiencesIdentity\>: Identity Parameter
  \[ActivityHistoryItemId \<String\>\]: The unique identifier of activityHistoryItem
  \[UserActivityId \<String\>\]: The unique identifier of userActivity
  \[UserId \<String\>\]: The unique identifier of user

## RELATED LINKS
[Remove-MgBetaUserActivity](/powershell/module/Microsoft.Graph.Beta.CrossDeviceExperiences/Remove-MgBetaUserActivity?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.crossdeviceexperiences/remove-mguseractivity](https://learn.microsoft.com/powershell/module/microsoft.graph.crossdeviceexperiences/remove-mguseractivity)


