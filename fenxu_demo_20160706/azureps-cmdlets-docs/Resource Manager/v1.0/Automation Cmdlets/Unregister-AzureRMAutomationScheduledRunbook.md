---
external help file: RMAzure_Automation.xml
online version: cfac4e12-2a1f-4b2c-873b-f5a3f9c4a2ce
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Unregister-AzureRMAutomationScheduledRunbook
## XXXXXXXX
Xxxxxxx xx xxxxxxxxxxx xxxxxxx x xxxxxxx xxx x xxxxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Unregister-AzureRMAutomationScheduledRunbook [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [-Force] -JobScheduleId <Guid]> [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_2
```
Unregister-AzureRMAutomationScheduledRunbook [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [-Force] -RunbookName <String> -ScheduleName <String> [-Confirm] [-WhatIf]
```

## XXXXXXXXXXX
Xxx $$Xxxxxxxxxx$XxxxxXxXxxxxxxxxxXxxxxxxxxXxxxxxx$$ xxxxxx xxxxxxx xxx xxxxxxxxxxx xxxxxxx xx xxxxx$0 Xxxxxxxxxx xxxxxxx xxx x xxxxxxxx.
Xxx xxxxxxxx xx xxxxxx xxxxxx xxx xxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx xxx xxxxxxxxxxx xxxxxxx x xxxxxxx xxx x xxxxxxxx
```
PS C:\>Unregister-AzureRmAutomationScheduledRunbook -AutomationAccountName "Contoso17" -Name "Runbk01" -ResourceGroupName "ResourceGroup01" -ScheduleName "Runbk01Sched"
```

Xxxx xxxxxxx xxxxxxx xxx xxxxxxxxxxx xxxxxxx xxx xxxxxxx xxxxx Xxxxx00 xxx xxx xxxxxxxx xxxxx Xxxxx00Xxxxx.

## XXXXXXXXXX

### -AutomationAccountName
Xxxxxxxxx xx Xxxxxxxxxx xxxxxxx xxx xxx xxxxxxx xx xxxxx xxxx xxxxxx xxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Force
xx$xxxxx

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -JobScheduleId
Xxxxxxxxx xxx XX xx x xxxxxxxxx xxxxxxx.

```yaml
Type: Guid]
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Xxxxxxxxx xxx xxxx xx x xxxxxxxx xxxxx xxx xxx xxxxxxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -RunbookName
Xxxxxxxxx xxx xxxx xx xxx xxxxxxx xxxx xxxx xxxxxx xxxxxxxxxxx xxxx x xxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: Name

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ScheduleName
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxx xxxx xxxxx xxxx xxxxxx xxxxxxxxxxx x xxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Confirm
xxxx$xxxxxxxxxxx

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

### -WhatIf
xxxx$xxxxxxxxxx

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

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Get-AzureRmAutomationScheduledRunbook](cfac4e12-2a1f-4b2c-873b-f5a3f9c4a2ce)

[Register-AzureRmAutomationScheduledRunbook](34edfa3b-7ef9-4aab-bb17-5ea725a22ed4)


