---
external help file: RMAzure_Storage.xml
online version: a89aa1b2-cabd-4048-a84d-2b37da287c05
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Remove-AzureStorageQueue
## XXXXXXXX
Xxxxxxx x xxxxxxx xxxxx.

## XXXXXX

```
Remove-AzureStorageQueue [-Name] <String> [-Context <AzureStorageContext>] [-Force] [-PassThru] [-Confirm]
 [-WhatIf]
```

## XXXXXXXXXXX
Xxx $$Xxxxxx$XxxxxXxxxxxxXxxxx$$ xxxxxx xxxxxxx x xxxxxxx xxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxxxxxx xxxxx xx xxxx
```
PS C:\>Remove-AzureStorageQueue "ContosoQueue01"
```

Xxxx xxxxxxx xxxxxxx x xxxxx xxxxx XxxxxxxXxxxx00.

### Xxxxxxx 0$ Xxxxxx xxxxxxxx xxxxxxx xxxxxx
```
PS C:\>Get-AzureStorageQueue "Contoso*" | Remove-AzureStorageQueue
```

Xxxx xxxxxxx xxxxxxx xxx xxxxxx xxxx xxxxx xxxx xxxxx xxxx Xxxxxxx.

## XXXXXXXXXX

### -Context
Xxxxxxxxx xxx xxxxx$0 xxxxxxx xxxxxxx.
Xx xxxxxx xxx xxxxxxx xxxxxxx$ xxx Xxx$XxxxxXxxxxxxXxxxxxx xxxxxx.

```yaml
Type: AzureStorageContext
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByValue,ByPropertyName)
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

### -Name
Xxxxxxxxx xxx xxxx xx xxx xxxxx xx xxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: N,Queue

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByValue,ByPropertyName)
Accept wildcard characters: False
```

### -PassThru
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxxx x $$Xxxxxxx$$ xxxx xxxxxxxx xxx xxxxxxx xx xxx xxxxxxxxx.
Xx xxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxx x xxxxx.

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

[Get-AzureStorageQueue](a89aa1b2-cabd-4048-a84d-2b37da287c05)

[New-AzureStorageQueue](4b1216b7-40c6-418b-806e-63302d8ba4a1)


