---
external help file: Microsoft.Graph.Bookings-help.xml
Module Name: Microsoft.Graph.Bookings
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.bookings/invoke-mgdeactivatesolutionbackuprestoreprotectionpolicy
schema: 2.0.0
ms.subservice: m365-backup-storage
---

# Invoke-MgDeactivateSolutionBackupRestoreProtectionPolicy

## SYNOPSIS
Deactivate a protectionPolicyBase.

> [!NOTE]
> To view the beta release of this cmdlet, view [Invoke-MgBetaDeactivateSolutionBackupRestoreProtectionPolicy](/powershell/module/Microsoft.Graph.Beta.Bookings/Invoke-MgBetaDeactivateSolutionBackupRestoreProtectionPolicy?view=graph-powershell-beta)

## SYNTAX

### Deactivate (Default)
```
Invoke-MgDeactivateSolutionBackupRestoreProtectionPolicy -ProtectionPolicyBaseId <String>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-ProgressAction <ActionPreference>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### DeactivateViaIdentity
```
Invoke-MgDeactivateSolutionBackupRestoreProtectionPolicy -InputObject <IBookingsIdentity>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-ProgressAction <ActionPreference>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Deactivate a protectionPolicyBase.

## EXAMPLES
### Example 1: Deactivate an active protection policy

```powershell

Import-Module Microsoft.Graph.Bookings

Invoke-MgDeactivateSolutionBackupRestoreProtectionPolicy -ProtectionPolicyBaseId $protectionPolicyBaseId

```
This example will deactivate an active protection policy

### Example 2 : Deactivate a protection policy in updating state

```powershell

Import-Module Microsoft.Graph.Bookings

Invoke-MgDeactivateSolutionBackupRestoreProtectionPolicy -ProtectionPolicyBaseId $protectionPolicyBaseId

```
This example will deactivate a protection policy in updating state


## PARAMETERS

### -Headers
Optional headers that will be added to the request.

```yaml
Type: IDictionary
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IBookingsIdentity
Parameter Sets: DeactivateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ProgressAction
{{ Fill ProgressAction Description }}

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: proga

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProtectionPolicyBaseId
The unique identifier of protectionPolicyBase

```yaml
Type: String
Parameter Sets: Deactivate
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResponseHeadersVariable
Optional Response Headers Variable.

```yaml
Type: String
Parameter Sets: (All)
Aliases: RHV

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
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphProtectionPolicyBase
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<IBookingsIdentity>`: Identity Parameter
  - `[AttendanceRecordId <String>]`: The unique identifier of attendanceRecord
  - `[BookingAppointmentId <String>]`: The unique identifier of bookingAppointment
  - `[BookingBusinessId <String>]`: The unique identifier of bookingBusiness
  - `[BookingCurrencyId <String>]`: The unique identifier of bookingCurrency
  - `[BookingCustomQuestionId <String>]`: The unique identifier of bookingCustomQuestion
  - `[BookingCustomerBaseId <String>]`: The unique identifier of bookingCustomerBase
  - `[BookingServiceId <String>]`: The unique identifier of bookingService
  - `[BookingStaffMemberBaseId <String>]`: The unique identifier of bookingStaffMemberBase
  - `[Email <String>]`: Alternate key of virtualEventRegistration
  - `[MeetingAttendanceReportId <String>]`: The unique identifier of meetingAttendanceReport
  - `[ProtectionPolicyBaseId <String>]`: The unique identifier of protectionPolicyBase
  - `[RestoreSessionBaseId <String>]`: The unique identifier of restoreSessionBase
  - `[Role <String>]`: Usage: role='{role}'
  - `[ServiceAppId <String>]`: The unique identifier of serviceApp
  - `[UserId <String>]`: Usage: userId='{userId}'
  - `[VirtualEventId <String>]`: The unique identifier of virtualEvent
  - `[VirtualEventPresenterId <String>]`: The unique identifier of virtualEventPresenter
  - `[VirtualEventRegistrationId <String>]`: The unique identifier of virtualEventRegistration
  - `[VirtualEventRegistrationQuestionBaseId <String>]`: The unique identifier of virtualEventRegistrationQuestionBase
  - `[VirtualEventSessionId <String>]`: The unique identifier of virtualEventSession
  - `[VirtualEventTownhallId <String>]`: The unique identifier of virtualEventTownhall
  - `[VirtualEventWebinarId <String>]`: The unique identifier of virtualEventWebinar

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.bookings/invoke-mgdeactivatesolutionbackuprestoreprotectionpolicy](https://learn.microsoft.com/powershell/module/microsoft.graph.bookings/invoke-mgdeactivatesolutionbackuprestoreprotectionpolicy)

[https://learn.microsoft.com/graph/api/protectionpolicybase-deactivate?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/protectionpolicybase-deactivate?view=graph-rest-1.0)























