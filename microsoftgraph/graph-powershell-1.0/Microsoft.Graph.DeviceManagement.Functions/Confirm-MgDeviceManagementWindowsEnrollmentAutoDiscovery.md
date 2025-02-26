---
external help file: Microsoft.Graph.DeviceManagement.Functions-help.xml
Module Name: Microsoft.Graph.DeviceManagement.Functions
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement.functions/confirm-mgdevicemanagementwindowsenrollmentautodiscovery
schema: 2.0.0
---

# Confirm-MgDeviceManagementWindowsEnrollmentAutoDiscovery

## SYNOPSIS
Invoke function verifyWindowsEnrollmentAutoDiscovery

> [!NOTE]
> To view the beta release of this cmdlet, view [Confirm-MgBetaDeviceManagementWindowsEnrollmentAutoDiscovery](/powershell/module/Microsoft.Graph.Beta.DeviceManagement.Functions/Confirm-MgBetaDeviceManagementWindowsEnrollmentAutoDiscovery?view=graph-powershell-beta)

## SYNTAX

### Verify (Default)
```
Confirm-MgDeviceManagementWindowsEnrollmentAutoDiscovery -DomainName <String> [<CommonParameters>]
```

### VerifyViaIdentity
```
Confirm-MgDeviceManagementWindowsEnrollmentAutoDiscovery -InputObject <IDeviceManagementFunctionsIdentity>
 [<CommonParameters>]
```

## DESCRIPTION
Invoke function verifyWindowsEnrollmentAutoDiscovery

## PARAMETERS

### -DomainName
Usage: domainName='{domainName}'

```yaml
Type: String
Parameter Sets: Verify
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
Type: IDeviceManagementFunctionsIdentity
Parameter Sets: VerifyViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IDeviceManagementFunctionsIdentity
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT \<IDeviceManagementFunctionsIdentity\>: Identity Parameter
  \[Category \<String\>\]: Usage: category='{category}'
  \[DeviceConfigurationId \<String\>\]: The unique identifier of deviceConfiguration
  \[DomainName \<String\>\]: Usage: domainName='{domainName}'
  \[Scope \<String\>\]: Usage: scope='{scope}'
  \[SecretReferenceValueId \<String\>\]: Usage: secretReferenceValueId='{secretReferenceValueId}'
  \[SummarizeBy \<UserExperienceAnalyticsSummarizedBy?\>\]: Usage: summarizeBy='{summarizeBy}'

## RELATED LINKS
[Confirm-MgBetaDeviceManagementWindowsEnrollmentAutoDiscovery](/powershell/module/Microsoft.Graph.Beta.DeviceManagement.Functions/Confirm-MgBetaDeviceManagementWindowsEnrollmentAutoDiscovery?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement.functions/confirm-mgdevicemanagementwindowsenrollmentautodiscovery](https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement.functions/confirm-mgdevicemanagementwindowsenrollmentautodiscovery)



