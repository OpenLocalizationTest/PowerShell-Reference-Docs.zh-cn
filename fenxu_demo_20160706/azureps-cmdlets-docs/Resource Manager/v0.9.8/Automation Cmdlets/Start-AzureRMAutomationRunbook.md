---
external help file: RMAzure_Automation.xml
online version: 614eee0d-f18e-4843-bed6-6cf43db59f75
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Start-AzureRMAutomationRunbook
## XXXXXXXX
Xxxxxx x xxxxxxx xxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Start-AzureRMAutomationRunbook [-ResourceGroupName] <System.String> [-AutomationAccountName] <System.String>
 [-Name] <System.String> [-Parameters <System.Collections.IDictionary>] [-RunOn <System.String>]
```

### UNNAMED_PARAMETER_SET_2
```
Start-AzureRMAutomationRunbook [-ResourceGroupName] <System.String> [-AutomationAccountName] <System.String>
 [-Name] <System.String> [-MaxWaitSeconds <System.Int32>] [-Parameters <System.Collections.IDictionary>]
 [-RunOn <System.String>] [-Wait]
```

## XXXXXXXXXXX
Xxx $$Xxxxx$XxxxxXxXxxxxxxxxxXxxxxxx$$ xxxxxx xxxxxx xx xxxxx$0 Xxxxxxxxxx xxxxxxx xxx.
Xxxxxxx xxx XX xx xxxx xx x xxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxx x xxxxxxx xxx
```
PS C:\>Start-AzureRmAutomationRunbook -AutomationAccountName "Contoso17" -Name "Runbk01" -ResourceGroupName "ResourceGroup01"
```

Xxxx xxxxxxx xxxxxx x xxxxxxx xxx xxx xxx xxxxxxx xxxxx Xxxxx00 xx xxx Xxxxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.

## XXXXXXXXXX

### -AutomationAccountName
$$Xxxx$$

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -MaxWaitSeconds
$$Xxxx$$

```yaml
Type: System.Int32
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
$$Xxxx$$

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: RunbookName

Required: True
Position: 3
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Parameters
$$Xxxx$$

```yaml
Type: System.Collections.IDictionary
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
$$Xxxx$$

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -RunOn
$$Xxxx$$

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: HybridWorker

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Wait
$$Xxxx$$

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

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

[Export-AzureRmAutomationRunbook](614eee0d-f18e-4843-bed6-6cf43db59f75)

[Get-AzureRmAutomationRunbook](71da0434-5c0f-498f-91f2-f09117dfa7ca)

[Import-AzureRmAutomationRunbook](6e05b8c0-5782-4580-b4e3-778e951be608)

[New-AzureRmAutomationRunbook](c0de19b6-68a5-46b0-8575-88f229fd2494)

[New-AzureRmAutomationRunbook](c0de19b6-68a5-46b0-8575-88f229fd2494)

[Publish-AzureRmAutomationRunbook](68a3d64a-280b-4285-b588-72c7a8c25942)

[Remove-AzureRmAutomationRunbook](073fedf2-2bbd-4173-946a-b79f88dc3c92)

[Set-AzureRmAutomationRunbook](80b64633-ceab-4609-bb58-e11ab99e9c35)


