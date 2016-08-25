---
external help file: RMAzure_Automation.xml
online version: 0bfb6a70-3a4a-4e58-a0b9-e41eb52a90ef
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Export-AzureRmAutomationDscNodeReportContent
## XXXXXXXX
Xxxxxxx xxx xxx xxxxxxx xx x XXX xxxxxx xxxx xxxx x XXX xxxx xx Xxxxxxxxxx.

## XXXXXX

```
Export-AzureRmAutomationDscNodeReportContent [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [-Force] [-OutputFolder <String>] -NodeId <Guid> -ReportId <Guid> [-Confirm] [-WhatIf]
```

## XXXXXXXXXXX
Xxx $$Xxxxxx$XxxxxXxXxxxxxxxxxXxxXxxxXxxxxxXxxxxxx$$ xxxxxx xxxxxxx xxx xxx xxxxxxxx xx xx XXX Xxxxxxx Xxxxx Xxxxxxxxxxxxx $XXX$ xxxxxx.
X XXX xxxx xxxxx x XXX xxxxxx xx xxxxx$0 Xxxxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxxxxx xxxx x XXX xxxx
```
PS C:\>$Node = Get-AzureRmAutomationDscNode -ResourceGroupName "ResourceGroup03" -AutomationAccountName "AutomationAccount01" -Name "Computer14"
PS C:\> $Report = Get-AzureRmAutomationDscNodeReport -ResourceGroupName "ResourceGroup03" -AutomationAccountName "ContosoAutomationAccount" -NodeId $Node.Id -Latest
PS C:\> $Report | Export-AzureRmAutomationDscNodeReportContent -OutputFolder "C:\Users\PattiFuller\Desktop"
```

Xxxx xxx xx xxxxxxxx xxxxxxx xxx xxxxxx xxxxxx xxxx xxx XXX xxxx xxxxx Xxxxxxxx00 xx xxx xxxxxxx.

## XXXXXXXXXX

### -AutomationAccountName
Xxxxxxxxx xxx xxxx xx xx Xxxxxxxxxx xxxxxxx.
Xxxx xxxxxx xxxxxxx xxxxxx xxxxxxx xxx x XXX xxxx xxxx xxxxxxx xx xxx Xxxxxxxxxx xxxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

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
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxxxx xx xxxxxxxx xxxxx xxxx xxxx x xxx xxxx xxxx xxx xxx xxxx xxxx.

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

### -NodeId
Xxxxxxxxx xxx xxxxxx XX xx xxx XXX xxxx xxx xxxxx xxxx xxxxxx xxxxxxx xxxxxx xxxxxxxx.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -OutputFolder
Xxxxxxxxx xxx xxxxxx xxxxxx xxxxx xxxx xxxxxx xxxxxxx xxxxxx xxxxxxxx.

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

### -ReportId
Xxxxxxxxx xxx xxxxxx XX xx xxx XXX xxxx xxxxxx xxxx xxxx xxxxxx xxxxxxx.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: Id

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Xxxxxxxxx xxx xxxx xx x xxxxxxxx xxxxx.
Xxxx xxxxxx xxxxxxx xxx xxxxxxxx xx x xxxxxx xxx xxx XXX xxxx xxxx xxxxxxx xx xxx xxxxxxxx xxxxx xxxx xxxx xxxxxx xxxxxxxxx.

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

[Export-AzureRmAutomationDscNodeReportContent](0bfb6a70-3a4a-4e58-a0b9-e41eb52a90ef)

[Get-AzureRmAutomationDscNode](19472f94-5827-4878-a17a-d7bb10932861)

[Get-AzureRmAutomationDscNodeReport](4e614479-d8a1-41bb-a8eb-8d833a314b54)


