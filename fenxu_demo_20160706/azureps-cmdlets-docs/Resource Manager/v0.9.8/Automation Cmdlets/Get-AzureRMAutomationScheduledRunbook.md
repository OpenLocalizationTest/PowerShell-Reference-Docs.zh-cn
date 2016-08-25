---
external help file: RMAzure_Automation.xml
online version: 34edfa3b-7ef9-4aab-bb17-5ea725a22ed4
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Get-AzureRMAutomationScheduledRunbook
## XXXXXXXX
Xxxx Xxxxxxxxxx xxxxxxxx xxx xxxxxxxxxx xxxxxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Get-AzureRMAutomationScheduledRunbook [-ResourceGroupName] <String> [-AutomationAccountName] <String>
```

### UNNAMED_PARAMETER_SET_2
```
Get-AzureRMAutomationScheduledRunbook [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 -JobScheduleId <Guid]>
```

### UNNAMED_PARAMETER_SET_3
```
Get-AzureRMAutomationScheduledRunbook [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 -RunbookName <String> -ScheduleName <String>
```

### UNNAMED_PARAMETER_SET_4
```
Get-AzureRMAutomationScheduledRunbook [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 -RunbookName <String>
```

### UNNAMED_PARAMETER_SET_5
```
Get-AzureRMAutomationScheduledRunbook [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 -ScheduleName <String>
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxXxxxxxxxxxXxxxxxxxxXxxxxxx$$ xxxxxx xxxx xxx xx xxxx xxxxx$0 Xxxxxxxxxx xxxxxxxx xxx xxxxxxxxxx xxxxxxxxx.
Xx xxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxxx xxxxxxxx.
Xxxxxxx xxx xxxx xx x xxxxxxx xx x xxxxxxxx xx xxxx xx xxx xxxxxxxx xxxxxxx xxxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx xxx xxxxxxxxx xxxxxxxx
```
PS C:\>Get-AzureRmAutomationScheduledRunbook -AutomationAccountName "Contoso17" -ResourceGroupName "ResourceGroup01"
```

Xxxx xxxxxxx xxxx xxx xxxxxxxxx xxxxxxxx xx xxx xxxxx$0 Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.

### Xxxxxxx 0$ Xxx xxx xxxxxxxxx xxxxxxxxxx xxxx x xxxxxxx
```
PS C:\>Get-AzureRmAutomationScheduledRunbook -AutomationAccountName "Contoso17" -ResourceGroupName "ResourceGroup01" -RunbookName "Runbk01"
```

Xxxx xxxxxxx xxxx xxx xxxxxxxxx xxxxxxxx xxx xxx xxxxxxx Xxxxx00 xx xxx xxxxx$0 Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.

### Xxxxxxx 0$ Xxx xxx xxxxxxxx xxxxxxxxxx xxxx x xxxxxxxx
```
PS C:\>Get-AzureRmAutomationScheduledRunbook -AutomationAccountName "Contoso17" -ResourceGroupName "ResourceGroup01" -ScheduleName "Schedule01"
```

Xxxx xxxxxxx xxxx xxx xxxxxxxxx xxxxxxxx xxx xxx xxxxxxxx Xxxxxxxx00 xx xxx xxxxx$0 Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.

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

### -JobScheduleId
Xxxxxxxxx xxx XX xx x xxxxxxxxx xxx xxxx xxxx xxxxxx xxxx.

```yaml
Type: Guid]
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Xxxxxxxxx xxx xxxx xx x xxxxxxxx xxxxx xxx xxxxxxxxx xxxxxxxx xxxx xxxx xxxxxx xxxx.

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
Xxxxxxxxx xxx xxxx xx x xxxxxxx xxx xxxxx xxxx xxxxxx xxxx xxxxxxxxx xxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_3, UNNAMED_PARAMETER_SET_4
Aliases: Name

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ScheduleName
Xxxxxxxxx xxx xxxx xx x xxxxxxxx xxx xxxxx xxxx xxxxxx xxxx xxxxxxxxx xxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_3, UNNAMED_PARAMETER_SET_5
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

### Microsoft.Azure.Commands.Automation.Model.JobSchedule

## XXXXX

## XXXXXXX XXXXX

[Register-AzureRmAutomationScheduledRunbook](34edfa3b-7ef9-4aab-bb17-5ea725a22ed4)

[Unregister-AzureRmAutomationScheduledRunbook](a56fc467-f64d-4453-9b55-cdd5cad1aa98)


