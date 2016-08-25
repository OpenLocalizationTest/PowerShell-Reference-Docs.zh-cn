---
external help file: RMAzure_Storage.xml
online version: 74bc4494-be41-4493-9939-e51e61dd09e6
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Start-AzureStorageFileCopy
## XXXXXXXX
Xxxxxx xx xxxx x xxxxxx xxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Start-AzureStorageFileCopy [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-DestContext <AzureStorageContext>] [-Force] [-ServerTimeoutPerRequest <Int32]>] -AbsoluteUri <String>
 -DestFilePath <String> -DestShareName <String> [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_2
```
Start-AzureStorageFileCopy [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>] [-Force]
 [-ServerTimeoutPerRequest <Int32]>] -AbsoluteUri <String> -DestFile <CloudFile> [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_3
```
Start-AzureStorageFileCopy [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-Context <AzureStorageContext>] [-DestContext <AzureStorageContext>] [-Force]
 [-ServerTimeoutPerRequest <Int32]>] -DestFilePath <String> -DestShareName <String> -SrcBlobName <String>
 -SrcContainerName <String> [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_4
```
Start-AzureStorageFileCopy [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-DestContext <AzureStorageContext>] [-Force] [-ServerTimeoutPerRequest <Int32]>] -DestFilePath <String>
 -DestShareName <String> -SrcBlobName <String> -SrcContainer <CloudBlobContainer> [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_5
```
Start-AzureStorageFileCopy [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>] [-Force]
 [-ServerTimeoutPerRequest <Int32]>] -DestFile <CloudFile> -SrcBlob <CloudBlob> [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_6
```
Start-AzureStorageFileCopy [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-DestContext <AzureStorageContext>] [-Force] [-ServerTimeoutPerRequest <Int32]>] -DestFilePath <String>
 -DestShareName <String> -SrcBlob <CloudBlob> [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_7
```
Start-AzureStorageFileCopy [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-Context <AzureStorageContext>] [-DestContext <AzureStorageContext>] [-Force]
 [-ServerTimeoutPerRequest <Int32]>] -DestFilePath <String> -DestShareName <String> -SrcFilePath <String>
 -SrcShareName <String> [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_8
```
Start-AzureStorageFileCopy [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-DestContext <AzureStorageContext>] [-Force] [-ServerTimeoutPerRequest <Int32]>] -DestFilePath <String>
 -DestShareName <String> -SrcFilePath <String> -SrcShare <CloudFileShare> [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_9
```
Start-AzureStorageFileCopy [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-DestContext <AzureStorageContext>] [-Force] [-ServerTimeoutPerRequest <Int32]>] -DestFilePath <String>
 -DestShareName <String> -SrcFile <CloudFile> [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_10
```
Start-AzureStorageFileCopy [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>] [-Force]
 [-ServerTimeoutPerRequest <Int32]>] -DestFile <CloudFile> -SrcFile <CloudFile> [-Confirm] [-WhatIf]
```

## XXXXXXXXXXX
Xxx $$Xxxxx$XxxxxXxxxxxxXxxxXxxx$$ xxxxxx xxxxxx xx xxxx x xxxxxx xxxx xx x xxxxxxxxxxx xxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxx xxxx xxxxxxxxx xxxx xxxx xx xxxx xx xxxxx xxxxx xxxx xxx xxxx xxxx
```
PS C:\>Start-AzureStorageFileCopy -SrcShareName "ContosoShare01" -SrcFilePath "FilePath01" -DestShareName "ContosoShare02" -DestFilePath "FilePath02"
```

Xxxx xxxxxxx xxxxxx x xxxx xxxxxxxxx xxxx xxxx xx xxxx.
Xxx xxxxxxx xxxxxxxxx xxxxx xxxx xxx xxxx xxxx

### Xxxxxxx 0$ Xxxxx xxxx xxxxxxxxx xxxx xxxx xx xxxx xx xxxxx xxxxxxxxx xxxx xxx xxxx xxxx
```
PS C:\>Start-AzureStorageFileCopy -SrcContainerName "ContosoContainer01" -SrcBlobName "ContosoBlob01" -DestShareName "ContosoShare" -DestFilePath "FilePath02"
```

Xxxx xxxxxxx xxxxxx x xxxx xxxxxxxxx xxxx xxxx xx xxxx.
Xxx xxxxxxx xxxxxxxxx xxxxxxxxx xxxx xxx xxxx xxxx

## XXXXXXXXXX

### -AbsoluteUri
Xxxxxxxxx xxx XXX xx xxx xxxxxx xxxx.
Xx xxx xxxxxx xxxxxxxx xxxxxxxx x xxxxxxxxxx$ xxx xxxx xxxxxxx xxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
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

### -Context
Xxxxxxxxx xx xxxxx$0 Xxxxxxx xxxxxxx.
Xx xxxxxx x xxxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxxxxx xxxxxx.

```yaml
Type: AzureStorageContext
Parameter Sets: UNNAMED_PARAMETER_SET_3, UNNAMED_PARAMETER_SET_7
Aliases: SrcContext

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -DestContext
Xxxxxxxxx xxx xxxxx$0 Xxxxxxx xxxxxxx xx xxx xxxxxxxxxxx.
Xx xxxxxx x xxxxxxx$ xxx $$Xxx$XxxxxXxxxxxxXxxxxxx$$.

```yaml
Type: AzureStorageContext
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_3, UNNAMED_PARAMETER_SET_4, UNNAMED_PARAMETER_SET_6, UNNAMED_PARAMETER_SET_7, UNNAMED_PARAMETER_SET_8, UNNAMED_PARAMETER_SET_9
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DestFile
Xxxxxxxxx x $$XxxxxXxxx$$ xxxxxx.
Xxx xxx xxxxxx x xxxxx xxxx xx xxxxxx xxx xx xxxxx xxx Xxx$XxxxxXxxxxxxXxxx xxxxxx.

```yaml
Type: CloudFile
Parameter Sets: UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_5, UNNAMED_PARAMETER_SET_10
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DestFilePath
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxxxxx xxxx xxxxxxxx xx xxx xxxxxxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_3, UNNAMED_PARAMETER_SET_4, UNNAMED_PARAMETER_SET_6, UNNAMED_PARAMETER_SET_7, UNNAMED_PARAMETER_SET_8, UNNAMED_PARAMETER_SET_9
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DestShareName
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_3, UNNAMED_PARAMETER_SET_4, UNNAMED_PARAMETER_SET_6, UNNAMED_PARAMETER_SET_7, UNNAMED_PARAMETER_SET_8, UNNAMED_PARAMETER_SET_9
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
xx$xxxxx

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
Xxxxxxxxx xxx xxxxxx xx xxx xxxx$xxx xxxxxx xxx xxx xxxxxx xxxx xx x xxxxxxx.

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

### -SrcBlob
Xxxxxxxxx x $$XxxxxXxxx$$ xxxxxx.
Xxx xxx xxxxxx x xxxxx xxxx xx xxxxxx xxx xx xxxxx xxx Xxx$XxxxxXxxxxxxXxxx xxxxxx.

```yaml
Type: CloudBlob
Parameter Sets: UNNAMED_PARAMETER_SET_5, UNNAMED_PARAMETER_SET_6
Aliases: ICloudBlob

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByValue,ByPropertyName)
Accept wildcard characters: False
```

### -SrcBlobName
Xxxxxxxxx xxx xxxx xx xxx xxxxxx xxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_3, UNNAMED_PARAMETER_SET_4
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SrcContainer
Xxxxxxxxx x xxxxx xxxx xxxxxxxxx xxxxxx.
Xxx xxx xxxxxx xxxxx xxxx xxxxxxxxx xxxxxx xx xxx xxx Xxx$XxxxxXxxxxxxXxxxxxxxx xxxxxx.

```yaml
Type: CloudBlobContainer
Parameter Sets: UNNAMED_PARAMETER_SET_4
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SrcContainerName
Xxxxxxxxx xxx xxxx xx xxx xxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SrcFile
Xxxxxxxxx x $$XxxxxXxxx$$ xxxxxx.
Xxx xxx xxxxxx x xxxxx xxxx xx xxxxxx xxx xx xxxxx $$Xxx$XxxxxXxxxxxxXxxx$$.

```yaml
Type: CloudFile
Parameter Sets: UNNAMED_PARAMETER_SET_9, UNNAMED_PARAMETER_SET_10
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByValue)
Accept wildcard characters: False
```

### -SrcFilePath
Xxxxxxxxx xxx xxxx xx xxx xxxxxx xxxx xxxxxxxx xx xxx xxxxxx xxxxxxxxx xx xxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_7, UNNAMED_PARAMETER_SET_8
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SrcShare
Xxxxxxxxx x xxxxx xxxx xxxxx xxxxxx.
Xxx xxx xxxxxx x xxxxx xxxx xxxxx xx xxxxxx xxx xx xxxxx xxx Xxx$XxxxxXxxxxxxXxxxx xxxxxx.

```yaml
Type: CloudFileShare
Parameter Sets: UNNAMED_PARAMETER_SET_8
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SrcShareName
Xxxxxxxxx xxx xxxx xx xxx xxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_7
Aliases: 

Required: True
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

[Get-AzureStorageFile](d9ec4b6f-fb17-4f29-b209-a3d5f212a6f1)

[Get-AzureStorageShare](10a13c83-d545-4729-99f9-048c774f32d7)

[Get-AzureStorageFileCopyState](248556e1-291f-4d27-b2e1-e00cc895b3a9)

[Stop-AzureStorageFileCopy](abc5a8cb-1151-4d5c-9230-d5c3a44f5a4c)


