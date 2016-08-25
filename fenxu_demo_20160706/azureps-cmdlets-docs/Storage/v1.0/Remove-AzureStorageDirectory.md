---
external help file: RMAzure_Storage.xml
online version: 10a13c83-d545-4729-99f9-048c774f32d7
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Remove-AzureStorageDirectory
## XXXXXXXX
Xxxxxxx x xxxxxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Remove-AzureStorageDirectory [-ShareName] <String> [-Path] <String>
 [-ClientTimeoutPerRequest <Nullable [System.Int32]>] [-ConcurrentTaskCount <Nullable [System.Int32]>]
 [-Context <AzureStorageContext>] [-PassThru] [-ServerTimeoutPerRequest <Nullable [System.Int32]>] [-Confirm]
 [-WhatIf]
```

### UNNAMED_PARAMETER_SET_2
```
Remove-AzureStorageDirectory [-Share] <CloudFileShare> [-Path] <String>
 [-ClientTimeoutPerRequest <Nullable [System.Int32]>] [-ConcurrentTaskCount <Nullable [System.Int32]>]
 [-PassThru] [-ServerTimeoutPerRequest <Nullable [System.Int32]>] [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_3
```
Remove-AzureStorageDirectory [-Directory] <CloudFileDirectory> [[-Path] <String>]
 [-ClientTimeoutPerRequest <Nullable [System.Int32]>] [-ConcurrentTaskCount <Nullable [System.Int32]>]
 [-PassThru] [-ServerTimeoutPerRequest <Nullable [System.Int32]>] [-Confirm] [-WhatIf]
```

## XXXXXXXXXXX
Xxx $$Xxxxxx$XxxxxXxxxxxxXxxxxxxxx$$ xxxxxx xxxxxxx x xxxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxxxxx
```
PS C:\>Remove-AzureStorageDirectory -ShareName "ContosoShare06" -Path "ContosoWorkingFolder"
```

Xxxx xxxxxxx xxxxxxx xxx xxxxxx xxxxx XxxxxxxXxxxxxxXxxxxx xxxx xxx xxxx xxxxx xxxxx XxxxxxxXxxxx00.

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

### -Directory
Xxxxxxxxx x xxxxxx xx x $$XxxxxXxxxXxxxxxxxx$$ xxxxxx.
Xxxx xxxxxx xxxxxxx xxx xxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.
Xx xxxxxx x xxxxxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxxxxxxx xxxxxx.
Xxx xxx xxxx xxx xxx $$Xxx$XxxxxXxxxxxxXxxx$$ xxxxxx xx xxxxxx x xxxxxxxxx.

```yaml
Type: CloudFileDirectory
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByValue)
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

### -Path
Xxxxxxxxx xxx xxxx xx x xxxxxx.
Xx xxx xxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx xx xxxxx$ xxxx xxxxxx xxxxxxx xxxx xxxxxx.
Xx xxx xxxxxx xx xxx xxxxx$ xxxx xxxxxx xxxxx xx xxxxxx$ xxx xxxxxxx xx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases: 

Required: False
Position: 2
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
Xxxx xxxxxx xxxxxxx x xxxxxx xxxxx xxx xxxx xxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.
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

### -ShareName
Xxxxxxxxx xxx xxxx xx xxx xxxx xxxxx.
Xxxx xxxxxx xxxxxxx x xxxxxx xxxxx xxx xxxx xxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: 1
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

[Get-AzureStorageShare](10a13c83-d545-4729-99f9-048c774f32d7)

[New-AzureStorageContext](671aeec8-b7f9-49c5-866f-da84f189ab5b)

[New-AzureStorageDirectory](2eea330c-759d-4dee-81e9-2e72de9f707e)


