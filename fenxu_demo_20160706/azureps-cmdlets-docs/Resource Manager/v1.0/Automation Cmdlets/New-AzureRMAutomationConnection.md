---
external help file: RMAzure_Automation.xml
online version: 68f56d1c-23a9-4cb5-8fe8-c3a1e7c2ac1a
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# New-AzureRMAutomationConnection
## XXXXXXXX
Xxxxxxx xx Xxxxxxxxxx xxxxxxxxxx.

## XXXXXX

```
New-AzureRMAutomationConnection [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [-Name] <String> [-ConnectionTypeName] <String> [-ConnectionFieldValues] <IDictionary> [-Description <String>]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxXxxxxxxxxxXxxxxxxxxx$$ xxxxxx xxxxxxx x xxxxxxxxxx xx xxxxx$0 Xxxxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxxxxxxxxx
```
PS C:\>$FieldValues = @{"AutomationCertificateName"="ContosoCertificate";"SubscriptionID"="81b59010-dc55-45b7-89cd-5ca26db62472"}
PS C:\> New-AzureRmAutomationConnection -Name "Connection12" -ConnectionTypeName Azure -ConnectionFieldValues $FieldValues -ResourceGroupName "ResourceGroup01" -AutomationAccountName "AutomationAccount01"
```

Xxx xxxxx xxxxxxx xxxxxxx x xxxx xxxxx xx xxxxx xxxxxx xx xxx $XxxxxXxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxxx xx xxxxx$0 xxxxxxxxxx xxxxx Xxxxxxxxxx00 xx xxx Xxxxxxxxxx xxxxxxx xxxxx XxxxxxxxxxXxxxxxx00.
Xxx xxxxxxx xxxx xxx xxxxxxxxxx xxxxx xxxxxx xx $XxxxxXxxxxx.

## XXXXXXXXXX

### -AutomationAccountName
Xxxxxxxxx xxx xxxx xx xxx Xxxxxxxxxx xxxxxxx xxx xxxxx xxxx xxxxxx xxxxxxx x xxxxxxxxxx.

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

### -ConnectionFieldValues
Xxxxxxxxx x xxxx xxxxx xxxx xxxxxxxx xxx$xxxxx xxxxx.
Xxx xxxx xxxxxxxxx xxx xxxxxxxxxx xxxxxx xxx xxx xxxxxxxxx xxxxxxxxxx xxxx.
Xxx xxxxxx xxxxxxxxx xxx xxxxxxxx xxxxxx xx xxxx xxxxxxxxxx xxxxx xxx xxx xxxxxxxxxx xxxxxxxx.

```yaml
Type: IDictionary
Parameter Sets: (All)
Aliases: 

Required: True
Position: 5
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ConnectionTypeName
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxxxx xxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 4
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Description
Xxxxxxxxx x xxxxxxxxxxx xxx xxx xxxxxxxxxx.

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

### -Name
Xxxxxxxxx x xxxx xxx xxx xxxxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxx xxxxx xxx xxxxx xxxx xxxxxx xxxxxxx x xxxxxxxxxx.

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

## XXXXXX

## XXXXXXX

### Microsoft.Azure.Commands.Automation.Model.Connection

## XXXXX

## XXXXXXX XXXXX

[Get-AzureRmAutomationConnection](68f56d1c-23a9-4cb5-8fe8-c3a1e7c2ac1a)

[Remove-AzureRmAutomationConnection](76dc3b3d-2dd3-49ad-a28c-afbfc754e020)


