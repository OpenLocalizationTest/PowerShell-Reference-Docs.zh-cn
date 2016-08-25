---
external help file: RMAzure_Storage.xml
online version: 7e23b9f6-5f66-49a3-beb8-e2639c5234d7
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Set-AzureStorageShareQuota
## XXXXXXXX
Xxxx xxx xxxxxxx xxxxxxxx xxx x xxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Set-AzureStorageShareQuota [-ShareName] <String> [-Quota] <Int32>
 [-ClientTimeoutPerRequest <Nullable [System.Int32]>] [-ConcurrentTaskCount <Nullable [System.Int32]>]
 [-Context <AzureStorageContext>] [-ServerTimeoutPerRequest <Nullable [System.Int32]>]
```

### UNNAMED_PARAMETER_SET_2
```
Set-AzureStorageShareQuota [-Share] <CloudFileShare> [-Quota] <Int32>
 [-ClientTimeoutPerRequest <Nullable [System.Int32]>] [-ConcurrentTaskCount <Nullable [System.Int32]>]
 [-ServerTimeoutPerRequest <Nullable [System.Int32]>]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxxxXxxxx$$ xxxxxx xxxx xxx xxxxxxx xxxxxxxx xxx x xxxxxxxxx xxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx xxx xxxxxxx xxxxxxxx xx x xxxxx
```
PS C:\>Set-AzureStorageShareQuota -ShareName "ContosoShare01" -Quota 1024
```

Xxxx xxxxxxx xxxx xxx xxxxxxx xxxxxxxx xxx x xxxxx xxxxx XxxxxxxXxxxx00 xx 0000 XX.

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

### -Quota
$$Xxxx$$

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: True
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
Xxxxxxxxx x $$XxxxxXxxxXxxxx$$ xxxxxx xx xxxxxxxxx xxx xxxxx xxx xxxxx xxxx xxxxxxx xxxx x xxxxx.
Xx xxxxxx x $$XxxxxXxxxXxxxx$$ xxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxxx xxxxxx.

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
Xxxxxxxxx xxx xxxx xx xxx xxxx xxxxx xxx xxxxx xx xxx x xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: N,Name

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue, ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Get-AzureStorageFileContent](7e23b9f6-5f66-49a3-beb8-e2639c5234d7)

[Get-AzureStorageShare](10a13c83-d545-4729-99f9-048c774f32d7)

[New-AzureStorageContext](671aeec8-b7f9-49c5-866f-da84f189ab5b)


