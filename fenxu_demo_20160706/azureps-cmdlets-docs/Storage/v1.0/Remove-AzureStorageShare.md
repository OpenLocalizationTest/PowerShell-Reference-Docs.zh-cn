---
external help file: RMAzure_Storage.xml
online version: 10a13c83-d545-4729-99f9-048c774f32d7
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Remove-AzureStorageShare
## XXXXXXXX
Xxxxxxx x xxxx xxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Remove-AzureStorageShare [-Name] <String> [-ClientTimeoutPerRequest <Nullable [System.Int32]>]
 [-ConcurrentTaskCount <Nullable [System.Int32]>] [-Context <AzureStorageContext>] [-PassThru]
 [-ServerTimeoutPerRequest <Nullable [System.Int32]>] [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_2
```
Remove-AzureStorageShare [-Share] <CloudFileShare> [-ClientTimeoutPerRequest <Nullable [System.Int32]>]
 [-ConcurrentTaskCount <Nullable [System.Int32]>] [-PassThru]
 [-ServerTimeoutPerRequest <Nullable [System.Int32]>] [-Confirm] [-WhatIf]
```

## XXXXXXXXXXX
Xxx $$Xxxxxx$XxxxxXxxxxxxXxxxx$$ xxxxxx xxxxxxx x xxxx xxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxxx xxxxx
```
PS C:\>Remove-AzureStorageShare -Name "ContosoShare06"
```

Xxxx xxxxxxx xxxxxxx xxx xxxx xxxxx xxxxx XxxxxxxXxxxx00.

## XXXXXXXXXX

### -ClientTimeoutPerRequest
$$Xxxx$$

```yaml
Type: Nullable [System.Int32]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConcurrentTaskCount
$$Xxxx$$

```yaml
Type: Nullable [System.Int32]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Context
$$Xxxx$$

```yaml
Type: AzureStorageContext
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByValue,ByPropertyName)
Accept wildcard characters: False
```

### -Name
Xxxxxxxxx xxx xxxx xx xxx xxxx xxxxx.
Xxxx xxxxxx xxxxxxx xxx xxxx xxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByValue,ByPropertyName)
Accept wildcard characters: False
```

### -PassThru
$$Xxxx$$

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

### -ServerTimeoutPerRequest
$$Xxxx$$

```yaml
Type: Nullable [System.Int32]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Share
Xxxxxxxxx x $$XxxxxXxxxXxxxx$$ xxxxxx.
Xxxx xxxxxx xxxxxxx xxx xxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.
Xx xxxxxx x $$XxxxxXxxxXxxxx$$ xxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxxx xxxxxx.
Xxxx xxxxxx xxxxxxxx xxx xxxxxxx xxxxxxx.
Xx xxx xxxxxxx xxxx xxxxxxxxx$ xx xxx xxxxxxx xxx $Xxxxxxx$ xxxxxxxxx.

```yaml
Type: CloudFileShare
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByValue)
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

[Get-AzureStorageShare](10a13c83-d545-4729-99f9-048c774f32d7)

[New-AzureStorageContext](671aeec8-b7f9-49c5-866f-da84f189ab5b)

[New-AzureStorageShare](17c0253c-c7b6-4c78-92ce-77277e156396)


