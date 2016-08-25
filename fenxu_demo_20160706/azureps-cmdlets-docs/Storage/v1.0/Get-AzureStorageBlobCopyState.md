---
external help file: RMAzure_Storage.xml
online version: 606cb5d3-e7fd-4647-b980-329334abc795
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Get-AzureStorageBlobCopyState
## XXXXXXXX
Xxxx xxx xxxx xxxxxx xx xx Xxxxx Xxxxxxx xxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Get-AzureStorageBlobCopyState [-Blob] <String> [-Container] <String> [-ClientTimeoutPerRequest <Int32]>]
 [-ConcurrentTaskCount <Int32]>] [-Context <AzureStorageContext>] [-ServerTimeoutPerRequest <Int32]>]
 [-WaitForComplete]
```

### UNNAMED_PARAMETER_SET_2
```
Get-AzureStorageBlobCopyState [-Blob] <String> [-ClientTimeoutPerRequest <Int32]>]
 [-ConcurrentTaskCount <Int32]>] [-Context <AzureStorageContext>] [-ServerTimeoutPerRequest <Int32]>]
 [-WaitForComplete] -CloudBlobContainer <CloudBlobContainer>
```

### UNNAMED_PARAMETER_SET_3
```
Get-AzureStorageBlobCopyState [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-Context <AzureStorageContext>] [-ServerTimeoutPerRequest <Int32]>] [-WaitForComplete] -CloudBlob <CloudBlob>
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxxXxxxXxxxx$$ xxxxxx xxxx xxx xxxx xxxxxx xx xx xxxxx$0 Xxxxxxx xxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx xxx xxxx xxxxxx xx x xxxx
```
C:\PS>Get-AzureStorageBlobCopyState -Blob "ContosoPlanning2015" -Container "ContosoUploads"
```

Xxxx xxxxxxx xxxx xxx xxxx xxxxxx xx xxx xxxx xxxxx XxxxxxxXxxxxxxx0000 xx xxx xxxxxxxxx XxxxxxxXxxxxxx.

### Xxxxxxx 0$ Xxx xxx xxxx xxxxxx xxx xx x xxxx xx xxxxx xxx xxxxxxxx
```
C:\PS>Get-AzureStorageBlob -Blob "ContosoPlanning2015" -Container "ContosoUploads" | Get-AzureStorageBlobCopyState
```

Xxxx xxxxxxx xxxx xxx xxxx xxxxx XxxxxxxXxxxxxxx0000 xx xxx xxxxxxxxx xxxxx XxxxxxxXxxxxxx xx xxxxx xxx $$Xxx$XxxxxXxxxxxxXxxx$$ xxxxxx$ xxx xxxx xxxxxx xxx xxxxxx xx xxx xxxxxxx xxxxxx xx xxxxx xxx xxxxxxxx xxxxxxxx.
Xxx $$Xxx$XxxxxXxxxxxxXxxxXxxxXxxxx$$ xxxxxx xxxx xxx xxxx xxxxxx xxx xxxx xxxx.

### Xxxxxxx 0$ Xxx xxx xxxx xxxxxx xxx x xxxx xx x xxxxxxxxx xx xxxxx xxx xxxxxxxx
```
C:\PS>Get-AzureStorageContainer -Name "ContosoUploads" | Get-AzureStorageBlobCopyState -Blob "ContosoPlanning2015"
```

Xxxx xxxxxxx xxxx xxx xxxxxxxxx xxxxx xx xxxxx xxx $$Xxx$XxxxxXxxxxxxXxxx$$ xxxxxx$ xxx xxxx xxxxxx xxx xxxxxx xx xxx xxxxxxx xxxxxx.
Xxx $$Xxx$XxxxxXxxxxxxXxxxxxxxx$$ xxxxxx xxxx xxx xxxx xxxxxx xxx xxx xxxx xxxxx XxxxxxxXxxxxxxx0000 xx xxxx xxxxxxxxx.

## XXXXXXXXXX

### -Blob
Xxxxxxxxx xxx xxxx xx x xxxx.
Xxxx xxxxxx xxxx xxx xxxxx xx xxx xxxx xxxx xxxxxxxxx xxx xxx xxxxx$0 Xxxxxxx xxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClientTimeoutPerRequest
Xxxxxxxxx xxx xxxxxx$xxxx xxxx$xxx xxxxxxxx$ xx xxxxxxx$ xxx xxx xxxxxxx xxxxxxx.
Xx xxx xxxxxxxx xxxx xxxxx xx xxx xxxxxxxxx xxxxxxxx$ xxxx xxxxxx xxxxxxx xxx xxxxxxx.
Xx xxxx xxxxxx xxxx xxx xxxxxxx x xxxxxxxxxx xxxxxxxx xxxxxx xxx xxxxxxxx xxxxxxx$ xxxx xxxxxx xxxxxxx xx xxxxx.

```yaml
Type: Int32]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CloudBlob
Xxxxxxxxx x $$XxxxxXxxx$$ xxxxxx xxxx xxxxx$0 Xxxxxxx Xxxxxx xxxxxxx.
Xx xxxxxx x $$XxxxxXxxx$$ xxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxx xxxxxx.

```yaml
Type: CloudBlob
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases: ICloudBlob

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -CloudBlobContainer
Xxxxxxxxx x $$XxxxxXxxxXxxxxxxxx$$ xxxxxx xxxx xxx xxxxx$0 Xxxxxxx Xxxxxx xxxxxxx.
Xxxx xxxxxx xxxx xxx xxxx xxxxxx xx x xxxx xx xxx xxxxxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.
Xx xxxxxx x $$XxxxxXxxxXxxxxxxxx$$ xxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxxxxxxx xxxxxx.

```yaml
Type: CloudBlobContainer
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ConcurrentTaskCount
Xxxxxxxxx xxx xxxxxxx xxxxxxxxxx xxxxxxx xxxxx.
Xxx xxx xxx xxxx xxxxxxxxx xx xxxxx xxx xxxxxxxxxxx xx xxxxxxxx xxxxx XXX xxx xxxxxxxxx xxxxx xx xxxxxxxxxx xxx xxxxxxx xxxxxx xx xxxxxxxxxx xxxxxxx xxxxx.
Xxx xxxxxxxxx xxxxx xx xx xxxxxxxx xxxxx xxx xx xxx xxxxxxxxxx xx xxx xxxx xxxxx.
Xxxx xxxxxxxxx xxx xxxx xxxxxx xxxxxxx xxxxxxxxxx xxxxxxxx xx xxx xxxxxxxxx xxxxxxxxxxxx$ xxxx xx 000 xxxxxxxx xxx xxxxxx.
Xxx xxxxxxx xxxxx xx 00.

```yaml
Type: Int32]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Container
Xxxxxxxxx xxx xxxx xx x xxxxxxxxx.
Xxxx xxxxxx xxxx xxx xxxx xxxxxx xxx x xxxx xx xxx xxxxxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

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

### -Context
Xxxxxxxxx xx xxxxx$0 xxxxxxx xxxxxxx.
Xx xxxxxx x xxxxxxx xxxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxxxxx xxxxxx.

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

### -ServerTimeoutPerRequest
Xxxxxxxxx xxx xxxxxxx xxxx xxxx$xxx xxxxxxxx$ xx xxxxxxx$ xxx x xxxxxxx.
Xx xxx xxxxxxxxx xxxxxxxx xxxxxxx xxxxxx xxx xxxxxxx xxxxxxxxx xxx xxxxxxx$ xxx xxxxxxx xxxxxxx xxxxxxx xx xxxxx.

```yaml
Type: Int32]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WaitForComplete
Xxxxxxxxx xxxx xxxx xxxxxx xxxxx xxx xxx xxxx xx xxxxxx.
Xx xxx xx xxx xxxxxxx xxxx xxxxxxxxx$ xxxx xxxxxx xxxxxxx x xxxxxx xxxxxxxxxxx.

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

### CopyState

## XXXXX

## XXXXXXX XXXXX

[Start-AzureStorageBlobCopy](606cb5d3-e7fd-4647-b980-329334abc795)

[Stop-AzureStorageBlobCopy](c75b9de9-597d-4986-980e-10e49eeef4a7)


