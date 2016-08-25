---
external help file: RMAzure_Automation.xml
online version: 0375f514-6679-4488-be72-816df6f13124
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Get-AzureRmAutomationDscCompilationJob
## XXXXXXXX
Xxxx XXX xxxxxxxxxxx xxxx xx Xxxxxxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Get-AzureRmAutomationDscCompilationJob [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [-EndTime <DateTimeOffset]>] [-StartTime <DateTimeOffset]>] [-Status]
```

### UNNAMED_PARAMETER_SET_2
```
Get-AzureRmAutomationDscCompilationJob [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 -Id <Guid>
```

### UNNAMED_PARAMETER_SET_3
```
Get-AzureRmAutomationDscCompilationJob [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [-EndTime <DateTimeOffset]>] [-StartTime <DateTimeOffset]>] [-Status] -ConfigurationName <String>
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxXxxxxxxxxxXxxXxxxxxxxxxxXxx$$ xxxxxx xxxx XXX Xxxxxxx Xxxxx Xxxxxxxxxxxxx $XXX$ xxxxxxxxxxx xxxx xx xxxxx$0 Xxxxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx xxx XXX xxxxxxxxxxx xxxx
```
PS C:\>Get-AzureRmAutomationDscCompilationJob -ResourceGroupName "ResourceGroup03" -AutomationAccountName "Contoso17"
```

Xxxx xxxxxxx xxxx xxx xxxxxxxxxxx xxxx xx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.

### Xxxxxxx 0$ Xxx XXX xxxxxxxxxxx xxxx xxx x xxxxxxxxxxxxx
```
PS C:\>Get-AzureRmAutomationDscCompilationJob -ResourceGroupName "ResourceGroup03" -AutomationAccountName "Contoso17" -ConfigurationName "ContosoConfiguration"
```

Xxxx xxxxxxx xxxx xxx xxxxxxxxxxx xxxx xxx xxx XXX xxxxxxxxxxxxx xxxxx XxxxxxxXxxxxxxxxxxxx xx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.

### Xxxxxxx 0$ Xxx x xxxxxxxx XXX xxxxxxxxxxx xxx
```
PS C:\>Get-AzureRmAutomationDscCompilationJob -ResourceGroupName "ResourceGroup03" -AutomationAccountName "Contoso17" -Id c0a1718e-d8be-4fa3-91b6-82e1d3a36298
```

Xxxx xxxxxxx xxxx xxx xxxxxxxxxxx xxx xxxx xxx xxxxxxxxx XX xx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.

## XXXXXXXXXX

### -AutomationAccountName
Xxxxxxxxx xxx xxxx xx xxx Xxxxxxxxxx xxxxxxx xxxx xxxxxxxx XXX xxxxxxxxxxx xxxx xxxx xxxx xxxxxx xxxx.

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

### -ConfigurationName
Xxxxxxxxx xxx xxxx xx xxx XXX xxxxxxxxxxxxx xxx xxxxx xxxx xxxxxx xxxx xxxxxxxxxxx xxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases: Name

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EndTime
Xxxxxxxxx xx xxx xxxx.
Xxxx xxxxxx xxxx xxxxxxxxxxxx xxxx xxxx xxxxxxx xx xx xxx xxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

```yaml
Type: DateTimeOffset]
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_3
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
Xxxxxxxxx xxx xxxxxx XX xx xxx XXX xxxxxxxxxxx xxx xxxx xxxx xxxxxx xxxx.

```yaml
Type: Guid
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: JobId

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Xxxxxxxxx xxx xxxx xx x xxxxxxxx xxxxx xx xxxxx xxxx xxxxxx xxxx XXX xxxxxxxxxxx xxxx.

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

### -StartTime
Xxxxxxxxx x xxxxx xxxx.
Xxxx xxxxxx xxxx xxxx xxxx xxxxx xx xx xxxxx xxx xxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

```yaml
Type: DateTimeOffset]
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_3
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Status
Xxxxxxxxx xxx xxxxxx xx xxxx xxxx xxxx xxxxxx xxxx.
Xxxxx xxxxxx xxx$ 

$$ Xxxxxxxxx $$ Xxxxxx $$ Xxxxxx $$ Xxxxxxxx $$ Xxxxxxxx $$ Xxxxxxx $$ Xxxxxxx $$ Xxxxxxxx $$ Xxxxxxxxx $$ Xxxxxxxxxx $$ Xxxxxxxxxx

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_3
Aliases: 
Accepted values: Completed, Failed, Queued, Starting, Resuming, Running, Stopped, Stopping, Suspended, Suspending, Activating

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Get-AzureRmAutomationDscCompilationJobOutput](0375f514-6679-4488-be72-816df6f13124)

[Start-AzureRmAutomationDscCompilationJob](d1d461ab-138f-42f2-8faf-e651a8310b08)


