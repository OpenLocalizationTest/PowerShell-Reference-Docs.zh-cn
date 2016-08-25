---
external help file: RMAzure_Storage.xml
online version: 36ff9a70-74d8-4b37-9962-c01b531c9a01
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Get-AzureStorageTable
## XXXXXXXX
Xxxxx xxx xxxxxxx xxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Get-AzureStorageTable [[-Name] <String>] [-Context <AzureStorageContext>]
```

### UNNAMED_PARAMETER_SET_2
```
Get-AzureStorageTable [-Context <AzureStorageContext>] -Prefix <String>
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxxx$$ xxxxxx xxxxx xxx xxxxxxx xxxxxx xxxxxxxxxx xxxx xxx xxxxxxx xxxxxxx xx xxxxx$0.

## XXXXXXXX

### Xxxxxxx 0$ Xxxx xxx Xxxxx Xxxxxxx xxxxxx
```
PS C:\>Get-AzureStorageTable
```

Xxxx xxxxxxx xxxx xxx xxxxxxx xxxxxx xxx x Xxxxxxx xxxxxxx.

### Xxxxxxx 0$ Xxxx Xxxxx Xxxxxxx xxxxxx xxxxx x xxxxxxxx xxxxxxxxx
```
PS C:\>Get-AzureStorageTable -Name table*
```

Xxxx xxxxxxx xxxx x xxxxxxxx xxxxxxxxx xx xxx xxxxxxx xxxxxx xxxxx xxxx xxxxxx xxxx xxxxx.

### Xxxxxxx 0$ Xxxx Xxxxx Xxxxxxx xxxxxx xxxxx xxxxx xxxx xxxxxx
```
PS C:\>Get-AzureStorageTable -Prefix "table"
```

Xxxx xxxxxxx xxxx xxx $Xxxxxx$ xxxxxxxxx xx xxx xxxxxxx xxxxxx xxxxx xxxx xxxxxx xxxx xxxxx.

## XXXXXXXXXX

### -Context
Xxxxxxxxx xxx xxxxxxx xxxxxxx.
Xx xxxxxx xx$ xxx xxx xxx xxx Xxx$XxxxxXxxxxxxXxxxxxx xxxxxx.

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

### -Name
Xxxxxxxxx xxx xxxxx xxxx.
Xx xxx xxxxx xxxx xx xxxxx$ xxx xxxxxx xxxxx xxx xxx xxxxxx.
Xxxxxxxxx$ xx xxxxx xxx xxxxxx xxxx xxxxx xxx xxxxxxxxx xxxx xx xxx xxxxxxx xxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: N,Table

Required: False
Position: 1
Default value: None
Accept pipeline input: True(ByValue,ByPropertyName)
Accept wildcard characters: False
```

### -Prefix
Xxxxxxxxx x xxxxxx xxxx xx xxx xxxx xx xxx xxxxx xx xxxxxx xxx xxxx xx xxx.
Xxx xxx xxx xxxx xx xxxx xxx xxxxxx xxxx xxxxx xxxx xxx xxxx xxxxxx$ xxxx xx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[New-AzureStorageTable](36ff9a70-74d8-4b37-9962-c01b531c9a01)

[Remove-AzureStorageTable](f287198d-609e-4ac1-9221-9ce5453a732e)


