---
external help file: RMAzure_Storage.xml
online version: d9ec4b6f-fb17-4f29-b209-a3d5f212a6f1
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# New-AzureStorageDirectory
## XXXXXXXX
Xxxxxxx x xxxxxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
New-AzureStorageDirectory [-ShareName] <String> [-Path] <String>
 [-ClientTimeoutPerRequest <Nullable [System.Int32]>] [-ConcurrentTaskCount <Nullable [System.Int32]>]
 [-Context <AzureStorageContext>] [-ServerTimeoutPerRequest <Nullable [System.Int32]>]
```

### UNNAMED_PARAMETER_SET_2
```
New-AzureStorageDirectory [-Share] <CloudFileShare> [-Path] <String>
 [-ClientTimeoutPerRequest <Nullable [System.Int32]>] [-ConcurrentTaskCount <Nullable [System.Int32]>]
 [-ServerTimeoutPerRequest <Nullable [System.Int32]>]
```

### UNNAMED_PARAMETER_SET_3
```
New-AzureStorageDirectory [-Directory] <CloudFileDirectory> [-Path] <String>
 [-ClientTimeoutPerRequest <Nullable [System.Int32]>] [-ConcurrentTaskCount <Nullable [System.Int32]>]
 [-ServerTimeoutPerRequest <Nullable [System.Int32]>]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxxxxxxx$$ xxxxxx xxxxxxx x xxxxxxxxx.
Xxxx xxxxxx xxxxxxx x $$XxxxxXxxxXxxxxxxxx$$ xxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxxxxx xx x xxxx xxxxx
```
PS C:\>New-AzureStorageDirectory -ShareName "ContosoShare06" -Path "ContosoWorkingFolder"
```

Xxxx xxxxxxx xxxxxxx x xxxxxx xxxxx XxxxxxxXxxxxxxXxxxxx xx xxx xxxx xxxxx xxxxx XxxxxxxXxxxx00.

### Xxxxxxx 0$ Xxxxxx x xxxxxx xx x xxxx xxxxx xxxxxxxxx xx x xxxx xxxxx xxxxxx
```
PS C:\>Get-AzureStorageShare -Name "ContosoShare06" | New-AzureStorageDirectory -Path "ContosoWorkingFolder"
```

Xxxx xxxxxxx xxxx xxx $$Xxx$XxxxxXxxxxxxXxxxx$$ xxxxxx xx xxx xxx xxxx xxxxx xxxxx XxxxxxxXxxxx00$ xxx xxxx xxxxxx xx xx xxx xxxxxxx xxxxxx xx xxxxx xxx xxxxxxxx xxxxxxxx.
Xxx xxxxxxx xxxxxx xxxxxxx xxx xxxxxx xxxxx XxxxxxxXxxxxxxXxxxxx xx XxxxxxxXxxxx00.

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
Xxxx xxxxxx xxxxxxx xxx xxxxxx xx xxx xxxxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.
Xx xxxxxx x xxxxxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxxxxxxx xxxxxx.
Xxx xxx xxxx xxx xxx Xxx$XxxxxXxxxxxxXxxx xxxxxx xx xxxxxx x xxxxxxxxx.

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

### -Path
$$Xxxx$$

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True(ByValue,ByPropertyName)
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
Xxxx xxxxxx xxxxxxx x xxxxxx xx xxx xxxx xxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.
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
Xxxx xxxxxx xxxxxxx x xxxxxx xx xxx xxxx xxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

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

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Get-AzureStorageFile](d9ec4b6f-fb17-4f29-b209-a3d5f212a6f1)

[Get-AzureStorageShare](10a13c83-d545-4729-99f9-048c774f32d7)

[New-AzureStorageContext](671aeec8-b7f9-49c5-866f-da84f189ab5b)

[New-AzureStorageDirectory](2eea330c-759d-4dee-81e9-2e72de9f707e)

[Remove-AzureStorageDirectory](2cbd0756-0224-43b0-8e22-a7316b7e24c2)


