---
external help file: RMAzure_Automation.xml
online version: 73a4a9ba-477c-41e6-9193-2be97182e07d
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXXXxxxxxxxxxXxxxxxxx
## XXXXXXXX
Xxxxxxx xx Xxxxxxxxxx xxxxxxxx.

## XXXXXX

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureRMAutomationSchedule [-ResourceGroupName] <String> [-AutomationAccountName] <String> [-Name] <String>
 [-StartTime] <DateTimeOffset> [-Description <String>] [-ExpiryTime <DateTimeOffset>] [-TimeZone <String>]
 -DayInterval <Byte>
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureRMAutomationSchedule [-ResourceGroupName] <String> [-AutomationAccountName] <String> [-Name] <String>
 [-StartTime] <DateTimeOffset> [-Description <String>] [-TimeZone <String>] [-OneTime]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureRMAutomationSchedule [-ResourceGroupName] <String> [-AutomationAccountName] <String> [-Name] <String>
 [-StartTime] <DateTimeOffset> [-Description <String>] [-ExpiryTime <DateTimeOffset>] [-TimeZone <String>]
 -HourInterval <Byte>
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureRMAutomationSchedule [-DayOfWeek <Nullable [System.DayOfWeek]>] [-DayOfWeekOccurrence]
 [-TimeZone <String>] -MonthInterval <Byte>
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureRMAutomationSchedule [-DaysOfMonth <DaysOfMonth[]>] [-TimeZone <String>] -MonthInterval <Byte>
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureRMAutomationSchedule [-DaysOfWeek <DayOfWeek[]>] [-TimeZone <String>] -WeekInterval <Byte>
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxXxxxxxxxxxXxxxxxxx$$ xxxxxx xxxxxxx x xxxxxxxx xx xxxxx$0 Xxxxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxx$xxxx xxxxxxxx xx xxxxx xxxx
```
PS C:\>$TimeZone = ([System.TimeZoneInfo]::Local)Id
PS C:\> New-AzureRmAutomationSchedule -AutomationAccountName "Contoso17" -Name "Schedule01" -StartTime "23:00" -OneTime -ResourceGroupName "ResourceGroup01" -TimeZone $TimeZone
```

Xxx xxxxx xxxxxxx xxxx xxx xxxx xxxx XX xxxx xxx xxxxxx xxx xxxxxx xx xx xxx $XxxxXxxx xxxxxxxx.
Xxx xxxxxx xxxxxxx xxxxxxx x xxxxxxxx xxxx xxxx xxx xxxx xx xxx xxxxxxx xxxx xx 00$00 XX xx xxx xxxxxxxxx xxxx xxxx..

### Xxxxxxx 0$ Xxxxxx x xxxxxxxxx xxxxxxxx
```
PS C:\>$StartTime = Get-Date "13:00:00"
PS C:\> $EndTime = $StartTime.AddYears(1)
PS C:\> New-AzureRmAutomationSchedule -AutomationAccountName "Contoso17" -Name "Schedule02" -StartTime $StartTime -ExpiryTime $EndTime -DailyInterval 1 -ResourceGroupName "ResourceGroup01"
```

Xxx xxxxx xxxxxxx xxxxxxx x xxxx xxxxxx xx xxxxx xxx $$Xxx$Xxxx$$ xxxxxx$ xxx xxxx xxxxxx xxx xxxxxx xx xxx $XxxxxXxxx xxxxxxxx.
Xxxxxxx x xxxx xxxx xx xx xxxxx xxxx xxxxxxx xx xxx xxxxxx.

Xxx xxxxxx xxxxxxx xxxxxxx x xxxx xxxxxx xx xxxxx xxx $$Xxx$Xxxx$$ xxxxxx$ xxx xxxx xxxxxx xxx xxxxxx xx xxx $XxxXxxx xxxxxxxx.
Xxx xxxxxxx xxxxxxxxx x xxxxxx xxxx.

Xxx xxxxx xxxxxxx xxxxxxx x xxxxx xxxxxxxx xxxxx Xxxxxxxx00 xx xxxxx xx xxx xxxx xxxxxx xx $XxxxxXxxx xxx xxxxxx xx xxx xxxx xxxxxx xx $XxxXxxx.

## XXXXXXXXXX

### $XxxxxxxxxxXxxxxxxXxxx
Xxxxxxxxx xxx xxxx xx xx Xxxxxxxxxx xxxxxxx xxx xxxxx xxxx xxxxxx xxxxxxx x xxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_3
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $XxxXxxxxxxx
Xxxxxxxxx xx xxxxxxxx$ xx xxxx$ xxx xxx xxxxxxxx.
Xx xxx xx xxx xxxxxxx xxxx xxxxxxxxx$ xxx xxx xx xxx xxxxxxx xxx $XxxXxxx$ xxxxxxxxx$ xxx xxxxxxx xxxxx xx xxx $0$.

```yaml
Type: Byte
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxXxXxxx
Xxxxxxxxx x xxxx xx xxxx xx xxx xxxx xxx xxx xxxxxx xxxxxxxx.

```yaml
Type: Nullable [System.DayOfWeek]
Parameter Sets: UNNAMED_PARAMETER_SET_4
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxXxXxxxXxxxxxxxxx
Xxxxxxxxx xxx xxxxxxxxxx xx xxx xxxx xxxxxx xxx xxxxx xxxx xxx xxxxxxxx xxxx.
xxxx$xxxxxxxxxxx

$$ 0 $$ 0 $$ 0 $$ 0 $$ $0 $$ Xxxxx $$ Xxxxxx $$ Xxxxx $$ Xxxxxx $$ XxxxXxx

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_4
Aliases: 
Accepted values: First, Second, Third, Fourth, Last

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxXxxxx
Xxxxxxxxx x xxxx xx xxxx xx xxx xxxxx xxx xxx xxxxxxx xxxxxxxx.

```yaml
Type: DaysOfMonth[]
Parameter Sets: UNNAMED_PARAMETER_SET_5
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxXxxx
Xxxxxxxxx x xxxx xx xxxx xx xxx xxxx xxx xxx xxxxxx xxxxxxxx.

```yaml
Type: DayOfWeek[]
Parameter Sets: UNNAMED_PARAMETER_SET_6
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxxxxxx
Xxxxxxxxx x xxxxxxxxxxx xxx xxx xxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_3
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxxXxxx
Xxxxxxxxx xxx xxxxxx xxxx xx x xxxxxxxx xx x $$XxxxXxxxXxxxxx$$ xxxxxx.
Xxx xxx xxxxxxx x xxxxxx xxxx xxx xx xxxxxxxxx xx x xxxxx $$XxxxXxxxXxxxxx$$.

```yaml
Type: DateTimeOffset
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_3
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxxxxxx
Xxxxxxxxx xx xxxxxxxx$ xx xxxxx$ xxx xxx xxxxxxxx.

```yaml
Type: Byte
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxXxxxxxxx
Xxxxxxxxx xx xxxxxxxx$ xx Xxxxxx$ xxx xxx xxxxxxxx.

```yaml
Type: Byte
Parameter Sets: UNNAMED_PARAMETER_SET_4, UNNAMED_PARAMETER_SET_5
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxx
Xxxxxxxxx x xxxx xxx xxx xxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_3
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $XxxXxxx
Xxxxxxxxx xxxx xxx xxxxxx xxxxxxx x xxx$xxxx xxxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxXxxxxXxxx
Xxxxxxxxx xxx xxxx xx x xxxxxxxx xxxxx xxx xxxxx xxxx xxxxxx xxxxxxx x xxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_3
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxXxxx
Xxxxxxxxx xxx xxxxx xxxx xx x xxxxxxxx xx x $$XxxxXxxxXxxxxx$$ xxxxxx.
Xxx xxx xxxxxxx x xxxxxx xxxx xxx xx xxxxxxxxx xx x xxxxx $$XxxxXxxxXxxxxx$$.
. Xx xxx $XxxxXxxx$ xxxxxxxxx xx xxxxxxxxx$ xxx xxxxxx xxxx xx xxxxxxx xxx xxx xxxx xxxx xxxxxxxxx xx xxxx.

```yaml
Type: DateTimeOffset
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_3
Aliases: 

Required: True
Position: 4
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $XxxxXxxx
Xxxxxxxxx xxx xxxx xxxx xxx xxx xxxxxxxx.
Xxxx xxxxxx xxx xx xxx XXXX XX xx xxx Xxxxxxx Xxxx Xxxx XX.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $XxxxXxxxxxxx
Xxxxxxxxx xx xxxxxxxx$ xx xxxxx$ xxx xxx xxxxxxxx.

```yaml
Type: Byte
Parameter Sets: UNNAMED_PARAMETER_SET_6
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

### Xxxxxxxxx.Xxxxx.Xxxxxxxx.Xxxxxxxxxx.Xxxxx.Xxxxxxxx

## XXXXX

## XXXXXXX XXXXX

[Xxx$XxxxxXxXxxxxxxxxxXxxxxxxx](73a4a9ba-477c-41e6-9193-2be97182e07d)

[Xxxxxx$XxxxxXxXxxxxxxxxxXxxxxxxx](633c3e61-0da0-4a01-897b-e81c6e571196)

[Xxx$XxxxxXxXxxxxxxxxxXxxxxxxx](2d34dc26-ead0-49f0-9e1a-9d4a81712616)


