---
external help file: RMAzure_Storage.xml
online version: d9ec4b6f-fb17-4f29-b209-a3d5f212a6f1
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Get-AzureStorageFileCopyState
## XXXXXXXX
Xxxx xxx xxxxx xx x xxxx xxxxxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Get-AzureStorageFileCopyState [-ShareName] <String> [-FilePath] <String>
 [-ClientTimeoutPerRequest <Nullable [System.Int32]>] [-ConcurrentTaskCount <Nullable [System.Int32]>]
 [-Context <AzureStorageContext>] [-ServerTimeoutPerRequest <Nullable [System.Int32]>] [-WaitForComplete]
```

### UNNAMED_PARAMETER_SET_2
```
Get-AzureStorageFileCopyState [-File] <CloudFile> [-ClientTimeoutPerRequest <Nullable [System.Int32]>]
 [-ConcurrentTaskCount <Nullable [System.Int32]>] [-ServerTimeoutPerRequest <Nullable [System.Int32]>]
 [-WaitForComplete]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxxXxxxXxxxx$$ xxxxxx xxxx xxx xxxxx xx xx xxxxx$0 Xxxxxxx xxxx xxxx xxxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx xxx xxxx xxxxx xx xxxx xxxx
```
PS C:\>Get-AzureStorageFileCopyState -ShareName "ContosoShare" -FilePath "ContosoFile"
```

Xxxx xxxxxxx xxxx xxx xxxxx xx xxx xxxx xxxxxxxxx xxx x xxxx xxxx xxx xxx xxxxxxxxx xxxx.

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

### -File
Xxxxxxxxx x $$XxxxxXxxx$$ xxxxxx.
Xxx xxx xxxxxx x xxxxx xxxx xx xxxxxx xxx xx xxxxx xxx Xxx$XxxxxXxxxxxxXxxx xxxxxx.

```yaml
Type: CloudFile
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByValue)
Accept wildcard characters: False
```

### -FilePath
Xxxxxxxxx xxx xxxx xx xxx xxxx xxxxxxxx xx xx xxxxx$0 Xxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
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

### -ShareName
Xxxxxxxxx xxx xxxx xx x xxxxx.

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

### -WaitForComplete
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

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Get-AzureStorageFile](d9ec4b6f-fb17-4f29-b209-a3d5f212a6f1)

[New-AzureStorageContext](671aeec8-b7f9-49c5-866f-da84f189ab5b)

[Start-AzureStorageFileCopy](66445d9f-72a9-44e3-9f1b-72ec0888357a)

[Stop-AzureStorageFileCopy](abc5a8cb-1151-4d5c-9230-d5c3a44f5a4c)


