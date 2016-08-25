---
external help file: RMAzure_Storage.xml
online version: 15371eb7-da6a-4b26-bbda-b59a2eeedb1d
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Set-AzureStorageBlobContent
## XXXXXXXX
Xxxxxxx x xxxxx xxxx xx xx xxxxx$0 Xxxxxxx xxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Set-AzureStorageBlobContent [-File] <String> [-Container] <String> [-Blob <String>] [-BlobType]
 [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>] [-Context <AzureStorageContext>] [-Force]
 [-Metadata <Hashtable>] [-Properties <Hashtable>] [-ServerTimeoutPerRequest <Int32]>] [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_2
```
Set-AzureStorageBlobContent [-File] <String> [-Blob <String>] [-BlobType] [-ClientTimeoutPerRequest <Int32]>]
 [-ConcurrentTaskCount <Int32]>] [-Context <AzureStorageContext>] [-Force] [-Metadata <Hashtable>]
 [-Properties <Hashtable>] [-ServerTimeoutPerRequest <Int32]>] -CloudBlobContainer <CloudBlobContainer>
 [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_3
```
Set-AzureStorageBlobContent [-File] <String> [-BlobType] [-ClientTimeoutPerRequest <Int32]>]
 [-ConcurrentTaskCount <Int32]>] [-Context <AzureStorageContext>] [-Force] [-Metadata <Hashtable>]
 [-Properties <Hashtable>] [-ServerTimeoutPerRequest <Int32]>] -CloudBlob <CloudBlob> [-Confirm] [-WhatIf]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxxXxxxxxx$$ xxxxxx xxxxxxx x xxxxx xxxx xx xx xxxxx$0 Xxxxxxx xxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxxxx xxxx
```
PS C:\>Set-AzureStorageBlobContent -Container "ContosoUpload" -File ".\PlanningData" -Blob "Planning2015"
```

Xxxx xxxxxxx xxxxxxx xxx xxxx xxxx xx xxxxx XxxxxxxxXxxx xx x xxxx xxxxx Xxxxxxxx0000.

### Xxxxxxx 0$ Xxxxxx xxx xxxxx xxxxx xxx xxxxxxx xxxxxx
```
PS C:\>Get-ChildItem -File -Recurse | Set-AzureStorageBlobContent -Container "ContosoUploads"
```

Xxxx xxxxxxx xxxx xxx xxxx xxxxxxxxxx xxxxxx Xxx$XxxxxXxxx xx xxx xxx xxx xxxxx xx xxx xxxxxxx xxxxxx xxx xx xxxxxxxxxx$ xxx xxxx xxxxxx xxxx xx xxx xxxxxxx xxxxxx xx xxxxx xxx xxxxxxxx xxxxxxxx.
Xxx $$Xxx$XxxxxXxxxxxxXxxxXxxxxxx$$ xxxxxx xxxxxxx xxx xxxxx xx xxx xxxxxxxxx xxxxx XxxxxxxXxxxxxx.

### Xxxxxxx 0$ Xxxxxxxxx xx xxxxxxxx xxxx
```
PS C:\>Get-AzureStorageBlob -Container "ContosoUploads" -Blob "Planning2015" | Set-AzureStorageBlobContent -File "ContosoPlanning"
```

Xxxx xxxxxxx xxxx xxx xxxx xxxxx Xxxxxxxx0000 xx xxx XxxxxxxXxxxxxx xxxxxxxxx xx xxxxx xxx Xxx$XxxxxXxxxxxxXxxx xxxxxx$ xxx xxxx xxxxxx xxxx xxxx xx xxx xxxxxxx xxxxxx.
Xxx xxxxxxx xxxxxxx xxx xxxx xxxx xx xxxxx XxxxxxxXxxxxxxx xx Xxxxxxxx0000.
Xxxx xxxxxxx xxxx xxx xxxxxxx xxx $Xxxxx$ xxxxxxxxx.
Xxx xxxxxxx xxxxxxx xxx xxx xxxxxxxxxxxx.
Xx xxx xxxxxxx xxx xxxxxxx$ xxx xxxxxx xxxxxxxxxx xxx xxxxxxxx xxxx.

### Xxxxxxx 0$ Xxxxxx x xxxx xx x xxxxxxxxx xx xxxxx xxx xxxxxxxx
```
PS C:\>Get-AzureStorageContainer -Container "ContosoUpload*" | Set-AzureStorageBlobContent -File "ContosoPlanning" -Blob "Planning2015"
```

Xxxx xxxxxxx xxxx xxx xxxxxxxxx xxxx xxxxxx xxxx xxx xxxxxx XxxxxxxXxxxxx xx xxxxx xxx $$Xxx$XxxxxXxxxxxxXxxxxxxxx$$ xxxxxx$ xxx xxxx xxxxxx xxxx xxxx xx xxx xxxxxxx xxxxxx.
Xxx xxxxxxx xxxxxxx xxx xxxx xxxx xx xxxxx XxxxxxxXxxxxxxx xx Xxxxxxxx0000.

### Xxxxxxx 0$ Xxxxxx x xxxx xxx xxxxxxxx
```
PS C:\>$Metadata = @{"key" = "value"; "name" = "test"}
PS C:\> Set-AzureStorageBlobContent -File "ContosoPlanning" -Container "ContosoUploads" -Metadata $Metadata
```

Xxx xxxxx xxxxxxx xxxxxxx x xxxx xxxxx xxxx xxxxxxxx xxxxxxxx xxx x xxxx$ xxx xxxxxx xxxx xxxx xxxxx xx xxx $Xxxxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxxx xxx xxxx xxxx xx xxxxx XxxxxxxXxxxxxxx xx xxx xxxxxxxxx xxxxx XxxxxxxXxxxxxx.
Xxx xxxx xxxxxxxx xxx xxxxxxxx xxxxxx xx $Xxxxxxxx.

## XXXXXXXXXX

### -Blob
Xxxxxxxxx xxx xxxx xx x xxxx.
Xxxx xxxxxx xxxxxxx x xxxx xx xxx xxxxx$0 Xxxxxxx xxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BlobType
Xxxxxxxxx xxx xxxx xxx xxx xxxx xxxx xxxx xxxxxx xxxxxxx.
xxxx$xxxxxxxxxxx

$$ Xxxxx $$ Xxxx

Xxx xxxxxxx xxxxx xx Xxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Accepted values: Block, Page, Append

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
Xxxxxxxxx x $$XxxxxXxxx$$ xxxxxx.
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
Xxxx xxxxxx xxxxxxx xxxxxxx xx x xxxx xx xxx xxxxxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.
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
Xxxx xxxxxx xxxxxxx x xxxx xx x xxxx xx xxx xxxxxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

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

### -File
Xxxxxxxxx x xxxxx xxxx xxxx xxx x xxxx xx xxxxxx xx xxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: FullName

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_3
Aliases: FullName

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Force
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxxxxxx xx xxxxxxxx xxxx xxxxxxx xxxxxxxxx xxx xxx xxxxxxxxxxxx.

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

### -Metadata
Xxxxxxxxx xxxxxxxx xxx xxx xxxxxxxx xxxx.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Properties
Xxxxxxxxx xxxxxxxxxx xxx xxx xxxxxxxx xxxx.

```yaml
Type: Hashtable
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

[Get-AzureStorageBlobContent](15371eb7-da6a-4b26-bbda-b59a2eeedb1d)

[Get-AzureStorageBlob](74bc4494-be41-4493-9939-e51e61dd09e6)

[Remove-AzureStorageBlob](fddc1b9e-caf4-47d7-a6b2-a2b2bb50113a)


