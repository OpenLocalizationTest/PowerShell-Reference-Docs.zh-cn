---
external help file: RMAzure_Storage.xml
online version: 17c0253c-c7b6-4c78-92ce-77277e156396
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Get-AzureStorageShare
## XXXXXXXX
Xxxx x xxxx xx xxxx xxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Get-AzureStorageShare [[-Prefix] <String>] [-ClientTimeoutPerRequest <Nullable [System.Int32]>]
 [-ConcurrentTaskCount <Nullable [System.Int32]>] [-Context <AzureStorageContext>]
 [-ServerTimeoutPerRequest <Nullable [System.Int32]>]
```

### UNNAMED_PARAMETER_SET_2
```
Get-AzureStorageShare [-Name] <String> [-ClientTimeoutPerRequest <Nullable [System.Int32]>]
 [-ConcurrentTaskCount <Nullable [System.Int32]>] [-Context <AzureStorageContext>]
 [-ServerTimeoutPerRequest <Nullable [System.Int32]>]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxxx$$ xxxxxx xxxx x xxxx xx xxxx xxxxxx xxx x xxxxxxx xxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx x xxxx xxxxx
```
PS C:\>Get-AzureStorageShare -Name "ContosoShare06"
```

Xxxx xxxxxxx xxxx xxx xxxx xxxxx xxxxx XxxxxxxXxxxx00.

### Xxxxxxx 0$ Xxx xxx xxxx xxxxxx xxxx xxxxx xxxx x xxxxxx
```
PS C:\>Get-AzureStorageShare -Prefix "Contoso"
```

Xxxx xxxxxxx xxxx xxx xxxx xxxxxx xxxx xxxx xxxxx xxxx xxxxx xxxx Xxxxxxx.

### Xxxxxxx 0$ Xxx xxx xxxx xxxxxx xx x xxxxxxxxx xxxxxxx
```
PS C:\>$Context = New-AzureStorageContext -Local
PS C:\> Get-AzureStorageShare -Context $Context
```

Xxx xxxxx xxxxxxx xxxx xxx $$Xxx$XxxxxXxxxxxxXxxxxxx$$ xxxxxx xx xxxxxx x xxxxxxx xx xxxxx xxx $Xxxxx$ xxxxxxxxx$ xxx xxxx xxxxxx xxxx xxxxxxx xxxxxx xx xxx $Xxxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx xxxx xxxxxx xxx xxx xxxxxxx xxxxxx xxxxxx xx $Xxxxxxx.

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
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByValue,ByPropertyName)
Accept wildcard characters: False
```

### -Name
Xxxxxxxxx xxx xxxx xx xxx xxxx xxxxx.
Xxxx xxxxxx xxxx xxx xxxx xxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx$ xx xxxxxxx xx xxx xxxxxxx xxx xxxx xx x xxxx xxxxx xxxx xxxx xxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Prefix
Xxxxxxxxx xxx xxxxxx xxx xxxx xxxxxx.
Xxxx xxxxxx xxxx xxxx xxxxxx xxxx xxxxx xxx xxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx$ xx xx xxxx xxxxxx xx xx xxxx xxxxxx xxxxx xxx xxxxxxxxx xxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: 1
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

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[New-AzureStorageShare](17c0253c-c7b6-4c78-92ce-77277e156396)

[Remove-AzureStorageShare](f9a0f4e1-3677-4786-bd84-d3645c61baca)


