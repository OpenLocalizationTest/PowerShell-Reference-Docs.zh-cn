---
external help file: RMAzure_Storage.xml
online version: c3d50900-70d6-44af-b939-abe86fcf89e6
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Get-AzureStorageBlobContent
## XXXXXXXX
Xxxxxxxxx x xxxxxxx xxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Get-AzureStorageBlobContent [-Blob] <String> [-Container] <String> [-CheckMd5]
 [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>] [-Context <AzureStorageContext>]
 [-Destination <String>] [-Force] [-ServerTimeoutPerRequest <Int32]>] [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_2
```
Get-AzureStorageBlobContent [-Blob] <String> [-CheckMd5] [-ClientTimeoutPerRequest <Int32]>]
 [-ConcurrentTaskCount <Int32]>] [-Context <AzureStorageContext>] [-Destination <String>] [-Force]
 [-ServerTimeoutPerRequest <Int32]>] -CloudBlobContainer <CloudBlobContainer> [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_3
```
Get-AzureStorageBlobContent [-CheckMd5] [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-Context <AzureStorageContext>] [-Destination <String>] [-Force] [-ServerTimeoutPerRequest <Int32]>]
 -CloudBlob <CloudBlob> [-Confirm] [-WhatIf]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxxXxxxxxx$$ xxxxxx xxxxxxxxx xxx xxxxxxxxx xxxxxxx xxxx.
Xx xxx xxxx xxxx xx xxx xxxxx xxx xxx xxxxx xxxxxxxx$ xxxx xxxxxx xxxxxxxxxxxxx xxxxxxxx xx xx xx xx xxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxxxx xxxx xxxxxxx xx xxxx
```
PS C:\>Get-AzureStorageBlobContent -Container "ContainerName" -Blob "Blob" -Destination "C:\test\"
```

Xxxx xxxxxxx xxxxxxxxx x xxxx xx xxxx.

### Xxxxxxx 0$ Xxxxxxxx xxxx xxxxxxx xxxxx xxx xxxxxxxx
```
PS C:\>Get-AzureStorageBlob -Container containername -Blob blobname | Get-AzureStorageBlobContent
```

Xxxx xxxxxxx xxxx xxx xxxxxxxx xx xxxx xxx xxxxxxxx xxxx xxxxxxx.

### Xxxxxxx 0$ Xxxxxxxx xxxx xxxxxxx xxxxx xxx xxxxxxxx xxx x xxxxxxxx xxxxxxxxx
```
PS C:\>Get-AzureStorageContainer container* | Get-AzureStorageBlobContent -Blob "cbox.exe" -Destination "C:\test"
```

Xxxx xxxxxxx xxxx xxx xxxxxxxx xxxxxxxx xxxxxxxxx xxx xxx xxxxxxxx xx xxxx xxx xxxxxxxx xxxx xxxxxxx.

## XXXXXXXXXX

### -Blob
Xxxxxxxxx xxx xxxx xx xxx xxxx xx xx xxxxxxxxxx.

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

### -CheckMd5
Xxxxxxxxx xxxxxxx xx xxxxx xxx Xx0 xxx xxx xxx xxxxxxxxxx xxxx.

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
Xxxxxxxxx x xxxxx xxxx.
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
Xxxxxxxxx x $$XxxxxXxxxXxxxxxxxx$$ xxxxxx xxxx xxx xxxxx$0 xxxxxxx xxxxxx xxxxxxx.
Xxx xxx xxxxxx xx xx xxx xxx Xxx$XxxxxXxxxxxxXxxxxxxxx xxxxxx.

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
Xxxxxxxxx xxx xxxx xx xxxxxxxxx xxxx xxx xxx xxxx xxx xxxx xx xxxxxxxx.

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
Xxxxxxxxx xxx Xxxxx xxxxxxx xxxxxxx xxxx xxxxx xxx xxxx xx xxxxxxxx xxxx xxxxxxx.
Xxx xxx xxx xxx Xxx$XxxxxXxxxxxxXxxxxxx xxxxxx xx xxxxxx x xxxxxxx xxxxxxx.

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

### -Destination
Xxxxxxxxx xxx xxxxxxxx xx xxxxx xxx xxxxxxxxxx xxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Path

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Xxxxxxxxxx xx xxxxxxxx xxxx xxxxxxx xxxxxxxxxxxx.

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

### AzureStorageContainer

## XXXXX
Xx xxx xxxx xxxx xx xxxxxxx xxx xxxxx xxxxxxxx$ xxxx xxxxxx xxxxxxxxxxxx xx$ xx xx xx xxxxxxxx.

## XXXXXXX XXXXX

[Set-AzureStorageBlobContent](c3d50900-70d6-44af-b939-abe86fcf89e6)

[Get-AzureStorageBlob](74bc4494-be41-4493-9939-e51e61dd09e6)

[Remove-AzureStorageBlob](fddc1b9e-caf4-47d7-a6b2-a2b2bb50113a)


