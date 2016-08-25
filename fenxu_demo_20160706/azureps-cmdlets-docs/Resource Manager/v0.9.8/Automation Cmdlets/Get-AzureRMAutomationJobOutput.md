---
external help file: RMAzure_Automation.xml
online version: e41c8823-9e6a-4535-b90c-0e2de7634c47
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Get-AzureRMAutomationJobOutput
## XXXXXXXX
Xxxx xxx xxxxxx xx xx Xxxxxxxxxx xxx.

## XXXXXX

```
Get-AzureRMAutomationJobOutput [-ResourceGroupName] <String> [-AutomationAccountName] <String> [-Id] <Guid>
 [-StartTime <DateTimeOffset]>] [-Stream]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxXxxxxxxxxxXxxXxxxxx$$ xxxxxx xxxx xxx xxxxxx xx xx xxxxx$0 Xxxxxxxxxx xxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx xxx xxxxxx xx xx Xxxxxxxxxx xxx
```
PS C:\>Get-AzureRmAutomationJobOutput -AutomationAccountName "Contoso17" -Id 2989b069-24fe-40b9-b3bd-cb7e5eac4b64 -ResourceGroupName "ResourceGroup01" -Stream "Any"
```

Xxxx xxxxxxx xxxx xxx xx xxx xxxxxx xx xxx xxx xxxx xxx xxx xxxxxxxxx XX.

## XXXXXXXXXX

### -AutomationAccountName
Xxxxxxxxx xxx xxxx xx xx Xxxxxxxxxx xxxxxxx xxx xxxxx xxxx xxxxxx xxxx xxx xxxxxx.

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

### -Id
Xxxxxxxxx xxx XX xx x xxx xxx xxxxx xxxx xxxxxx xxxx xxxxxx.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: JobId

Required: True
Position: 3
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Xxxxxxxxx xxx xxxx xx x xxxxxxxx xxxxx xxx xxxxx xxxx xxxxxx xxxx xxx xxxxxx.

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
Xxxxxxxxx x xxxxx xxxx xx x $$XxxxXxxxXxxxxx$$ xxxxxx.
Xxx xxx xxxxxxx x xxxxxx xxxx xxx xx xxxxxxxxx xx x xxxxx $$XxxxXxxxXxxxxx$$.
Xxx xxxxxx xxxxxxxxx xxxxxx xxxxxxx xxxxx xxxx xxxx.

```yaml
Type: DateTimeOffset]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Stream
Xxxxxxxxx xxx xxxx xx xxxxxx.
Xxxxx xxxxxx xxx$ 

$$ Xxx $$ Xxxxx $$ Xxxxx $$ Xxxxxx $$ Xxxxxxxx $$ Xxxxxxx $$ Xxxxxxx

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Accepted values: Any, Progress, Output, Warning, Error, Debug, Verbose

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Get-AzureRmAutomationJob](e41c8823-9e6a-4535-b90c-0e2de7634c47)

[Resume-AzureRmAutomationJob](4b289017-5b98-45bc-87c4-86b08e1ac322)

[Stop-AzureRmAutomationJob](1b580598-1087-4a10-9bc3-747ec5d7604a)

[Suspend-AzureRmAutomationJob](cf05770c-fc18-4a31-beb9-4f8c1c39c285)


