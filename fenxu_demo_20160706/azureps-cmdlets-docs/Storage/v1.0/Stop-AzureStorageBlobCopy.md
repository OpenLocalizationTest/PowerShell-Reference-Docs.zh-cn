---
external help file: RMAzure_Storage.xml
online version: 74bc4494-be41-4493-9939-e51e61dd09e6
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Stop-AzureStorageBlobCopy
## XXXXXXXX
Xxxxx x xxxx xxxxxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Stop-AzureStorageBlobCopy [-Blob] <String> [-Container] <String> [-ClientTimeoutPerRequest <Int32]>]
 [-ConcurrentTaskCount <Int32]>] [-Context <AzureStorageContext>] [-CopyId <String>] [-Force]
 [-ServerTimeoutPerRequest <Int32]>] [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_2
```
Stop-AzureStorageBlobCopy [-Blob] <String> [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-Context <AzureStorageContext>] [-CopyId <String>] [-Force] [-ServerTimeoutPerRequest <Int32]>]
 -CloudBlobContainer <CloudBlobContainer> [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_3
```
Stop-AzureStorageBlobCopy [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-Context <AzureStorageContext>] [-CopyId <String>] [-Force] [-ServerTimeoutPerRequest <Int32]>]
 -CloudBlob <CloudBlob> [-Confirm] [-WhatIf]
```

## XXXXXXXXXXX
Xxx $$Xxxx$XxxxxXxxxxxxXxxxXxxx$$ xxxxxx xxxxx x xxxx xxxxxxxxx xx xxx xxxxxxxxx xxxxxxxxxxx xxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxx xxxx xxxxxxxxx xx xxxx
```
PS C:\>Stop-AzureStorageBlobCopy -Container "ContainerName" -Blob "BlobName" -CopyId "CopyID"
```

Xxxx xxxxxxx xxxxx xxx xxxx xxxxxxxxx xx xxxx.

### Xxxxxxx 0$ Xxxx xxxx xxxxxxxxx xx xxxxx xxx xxxxxxxx
```
PS C:\>Get-AzureStorageContainer container* | Stop-AzureStorageBlobCopy -Blob "BlobName"
```

Xxxx xxxxxxx xxxxx xxx xxxx xxxxxxxxx xx xxxxxxx xxx xxxxxxxxx xx xxx xxxxxxxx xxxx $$Xxx$XxxxxXxxxxxxXxxxxxxxx$$.

### Xxxxxxx 0$ Xxxx xxxx xxxxxxxxx xx xxxxx xxx xxxxxxxx xxx Xxx$XxxxxXxxxxxxXxxx
```
PS C:\>Get-AzureStorageBlob -Container "ContainerName" | Stop-AzureStorageBlobCopy -Force
```

Xxxx xxxxxxx xxxxx xxx xxxx xxxxxxxxx xx xxxxxxx xxx xxxxxxxxx xx xxx xxxxxxxx xxxx xxx Xxx$XxxxxXxxxxxxXxxx xxxxxx.

## XXXXXXXXXX

### -Blob
Xxxxxxxxx xxx xxxx xx xxx xxxx.

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
Xxx xxx xxxxxx xxx xxxxxx xx xxx xxx Xxx$XxxxxXxxxxxxXxxxxxxxx xxxxxx.

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
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxxx.

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
Xxxxxxxxx xxx xxxxx$0 xxxxxxx xxxxxxx.
Xxx xxx xxxxxx xxx xxxxxxx xx xxxxx xxx Xxx$XxxxxXxxxxxxXxxxxxx xxxxxx.

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

### -CopyId
Xxxxxxxxx xxx xxxx XX.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Xxxxx xxx xxxxxxx xxxx xxxx xx xxx xxxxxxxxx xxxx xxxxxxx xxxxxxxxx xxx xxxxxxxxxxxx.

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

[Get-AzureStorageBlob](74bc4494-be41-4493-9939-e51e61dd09e6)

[Get-AzureStorageContainer](4880a1a4-c947-4310-8317-0a837b8acb7f)

[Start-AzureStorageBlobCopy](606cb5d3-e7fd-4647-b980-329334abc795)

[Get-AzureStorageBlobCopyState](5ead5288-78e9-4ebb-904e-5e86ea88da93)


