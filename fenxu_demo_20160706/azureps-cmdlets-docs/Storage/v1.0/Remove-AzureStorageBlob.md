---
external help file: RMAzure_Storage.xml
online version: 74bc4494-be41-4493-9939-e51e61dd09e6
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxxxxx$XxxxxXxxxxxxXxxx
## XXXXXXXX
Xxxxxxx xxx xxxxxxxxx xxxxxxx xxxx.

## XXXXXX

### XXXXXXX$XXXXXXXXX$XXX$0
```
Remove-AzureStorageBlob [-Blob] <String> [-Container] <String> [-ClientTimeoutPerRequest <Int32]>]
 [-ConcurrentTaskCount <Int32]>] [-Context <AzureStorageContext>] [-DeleteSnapshot] [-Force] [-PassThru]
 [-ServerTimeoutPerRequest <Int32]>] [-Confirm] [-WhatIf]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Remove-AzureStorageBlob [-Blob] <String> [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-Context <AzureStorageContext>] [-DeleteSnapshot] [-Force] [-PassThru] [-ServerTimeoutPerRequest <Int32]>]
 -CloudBlobContainer <CloudBlobContainer> [-Confirm] [-WhatIf]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Remove-AzureStorageBlob [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-Context <AzureStorageContext>] [-DeleteSnapshot] [-Force] [-PassThru] [-ServerTimeoutPerRequest <Int32]>]
 -CloudBlob <CloudBlob> [-Confirm] [-WhatIf]
```

## XXXXXXXXXXX
Xxx $$Xxxxxx$XxxxxXxxxxxxXxxx$$ xxxxxx xxxxxxx xxx xxxxxxxxx xxxx xxxx x xxxxxxx xxxxxxx xx xxxxx$0.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxxxxxx xxxx xx xxxx
```
PS C:\>Remove-AzureStorageBlob -Container "ContainerName" -Blob "BlobName"
```

Xxxx xxxxxxx xxxxxxx x xxxx xxxxxxxxxx xx xxx xxxx.

### Xxxxxxx 0$ Xxxxxx x xxxxxxx xxxx xxxxx xxx xxxxxxxx
```
PS C:\>Get-AzureStorageBlob -Container "ContainerName" -Blob "BlobName" | Remove-AzureStorageBlob
```

Xxxx xxxxxxx xxxx xxx xxxxxxxx.

### Xxxxxxx 0$ Xxxxxx xxxxxxx xxxxx xxxxx xxx xxxxxxxx
```
PS C:\>Get-AzureStorageContainer -Container container* | Remove-AzureStorageBlob -Blob "BlobName"
```

Xxxx xxxxxxx xxxx xxx xxxxxxxx $$$ xxxxxxxx xxxxxxxxx xxx xxx xxxxxxxx xx xxxxxxxx xxx xxxx xx xxxxx xxx xxxx xxxxxxx xxxx.

## XXXXXXXXXX

### $Xxxx
Xxxxxxxxx xxx xxxx xx xxx xxxx xxx xxxx xx xxxxxx.

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

### $XxxxxxXxxxxxxXxxXxxxxxx
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

### $XxxxxXxxx
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

### $XxxxxXxxxXxxxxxxxx
Xxxxxxxxx x $$XxxxxXxxxXxxxxxxxx$$ xxxxxx xxxx xxx xxxxx$0 Xxxxxxx Xxxxxx xxxxxxx.
Xxx xxx xxx xxx Xxx$XxxxxXxxxxxxXxxxxxxxx xxxxxx xx xxx xx.

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

### $XxxxxxxxxxXxxxXxxxx
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

### $Xxxxxxxxx
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

### $Xxxxxxx
Xxxxxxxxx xxx xxxxx$0 xxxxxxx xxxxxxx.
Xxx xxx xxx xxx Xxx$XxxxxXxxxxxxXxxxxxx xxxxxx xx xxxxxx xx.

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

### $XxxxxxXxxxxxxx
Xxxxxxxxx xxxx xxx xxxxxxxxx xx xxxxxxx$ xxx xxx xxx xxxx xxxx.
Xx xxxx xxxxxxxxx xx xxx xxxxxxxxx$ xxx xxxx xxxx xxx xxx xxxxxxxxx xxx xxxxxxx xxxxxxxx.
Xxx xxxx xx xxxxxxxx xx xxxxxxx xxx xxxxxx xxxxxxxxx.

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

### $Xxxxx
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxxx xxx xxxx xxx xxx xxxxxxxx xxxxxxx xxxxxxxxxxxx.

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

### $XxxxXxxx
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxxx x $$Xxxxxxx$$ xxxx xxxxxxxx xxx xxxxxxx xx xxx xxxxxxxxx.
Xx xxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxx x xxxxx.

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

### $XxxxxxXxxxxxxXxxXxxxxxx
Xxxxxxxxx xxx xxxxx$0 xxxxxxx xxx xxx xxxxxx xx xxxx.
Xx xxx xxxxxxxxx$ xxx xxxxxx xxxxx xxxx xxx xxxxxxx xxxxxxx.

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

### $Xxxxxxx
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

### $XxxxXx
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

[Xxx$XxxxxXxxxxxxXxxx](74bc4494-be41-4493-9939-e51e61dd09e6)

[Xxx$XxxxxXxxxxxxXxxxXxxxxxx](15371eb7-da6a-4b26-bbda-b59a2eeedb1d)

[Xxx$XxxxxXxxxxxxXxxxXxxxxxx](c3d50900-70d6-44af-b939-abe86fcf89e6)


