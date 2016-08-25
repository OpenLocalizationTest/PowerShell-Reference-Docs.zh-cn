---
external help file: RMAzure_Automation.xml
online version: 03d80a68-8443-42e0-87bc-5d0e22ac3a57
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Get-AzureRMAutomationJob
## XXXXXXXX
Xxxx Xxxxxxxxxx xxxxxxx xxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Get-AzureRMAutomationJob [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [-EndTime <DateTimeOffset]>] [-StartTime <DateTimeOffset]>] [-Status]
```

### UNNAMED_PARAMETER_SET_2
```
Get-AzureRMAutomationJob [-ResourceGroupName] <String> [-AutomationAccountName] <String> -Id <Guid>
```

### UNNAMED_PARAMETER_SET_3
```
Get-AzureRMAutomationJob [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [-EndTime <DateTimeOffset]>] [-StartTime <DateTimeOffset]>] [-Status] -RunbookName <String>
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxXxxxxxxxxxXxx$$ xxxxxx xxxx xxxxxxx xxxx xx xxxxx$0 Xxxxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx x xxxxxxxx xxxxxxx xxx
```
PS C:\>Get-AzureRmAutomationJob -AutomationAccountName "Contoso17" -Id 2989b069-24fe-40b9-b3bd-cb7e5eac4b647
```

Xxxx xxxxxxx xxxx xxx xxx xxxx xxx xxx xxxxxxxxx XXXX.

### Xxxxxxx 0$ Xxx xxx xxxx xxx x xxxxxxx
```
PS C:\>Get-AzureRmAutomationJob -AutomationAccountName "Contoso17" -ResourceGroupName "ResourceGroup01" -RunbookName "Runbook02"
```

Xxxx xxxxxxx xxxx xxx xxxx xxxxxxxxxx xxxx x xxxxxxx xxxxx Xxxxxxx00.

### Xxxxxxx 0$ Xxx xxx xxxxxxx xxxx
```
PS C:\>Get-AzureRmAutomationJob -AutomationAccountName "Contoso17" -ResourceGroupName "ResourceGroup01" -Status "Running"
```

Xxxx xxxxxxx xxxx xxx xxxxxxx xxxx xx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.

## XXXXXXXXXX

### -AutomationAccountName
Xxxxxxxxx xxx xxxx xx xx Xxxxxxxxxx xxxxxxx xxx xxxxx xxxx xxxxxx xxxx xxxx.

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

### -EndTime
Xxxxxxxxx xxx xxx xxxx xxx x xxx xx x $$XxxxXxxxXxxxxx$$ xxxxxx.
Xxx xxx xxxxxxx x xxxxxx xxxx xxx xx xxxxxxxxx xx x xxxxx $$XxxxXxxxXxxxxx$$.
Xxxx xxxxxx xxxx xxxx xxxx xxxx xx xxx xxxx xx xx xxxxxx xxx xxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

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
Xxxxxxxxx xxx XX xx x xxx xxxx xxxx xxxxxx xxxx.

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
Xxxxxxxxx xxx xxxx xx x xxxxxxxx xxxxx xx xxxxx xxxx xxxxxx xxxx xxxx.

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
Xxxxxxxxx xxx xxxx xx x xxxxxxx xxx xxxxx xxxx xxxxxx xxxx xxxx.

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

### -StartTime
Xxxxxxxxx xxx xxxxx xxxx xx x xxx xx x $$XxxxXxxxXxxxxx$$ xxxxxx.
Xxxx xxxxxx xxxx xxxx xxxx xxxx x xxxxx xxxx xx xx xxxxx xxx xxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

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
Xxxxxxxxx xxx xxxxxx xx x xxx.
Xxxx xxxxxx xxxx xxxx xxxx xxxx x xxxxxx xxxxxxxx xxxx xxxxxxxxx.
Xxxxx xxxxxx xxx$ 

$$ Xxxxxxxxxx $$ Xxxxxxxxx $$ Xxxxxx $$ Xxxxxx $$ Xxxxxxxx $$ Xxxxxxx $$ Xxxxxxxx $$ Xxxxxxx $$ Xxxxxxxx $$ Xxxxxxxxx $$ Xxxxxxxxxx

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

### Microsoft.Azure.Commands.Automation.Model.Job

## XXXXX

## XXXXXXX XXXXX

[Get-AzureRmAutomationJobOutput](03d80a68-8443-42e0-87bc-5d0e22ac3a57)

[Resume-AzureRmAutomationJob](4b289017-5b98-45bc-87c4-86b08e1ac322)

[Stop-AzureRmAutomationJob](1b580598-1087-4a10-9bc3-747ec5d7604a)

[Suspend-AzureRmAutomationJob](cf05770c-fc18-4a31-beb9-4f8c1c39c285)


