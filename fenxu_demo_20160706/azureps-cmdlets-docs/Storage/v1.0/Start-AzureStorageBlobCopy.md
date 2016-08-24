---
external help file: RMAzure_Storage.xml
online version: 5ead5288-78e9-4ebb-904e-5e86ea88da93
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxxxx$XxxxxXxxxxxxXxxxXxxx
## XXXXXXXX
Xxxxxx xx xxxx x xxxx.

## XXXXXX

### XXXXXXX$XXXXXXXXX$XXX$0
```
Start-AzureStorageBlobCopy [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-Context <AzureStorageContext>] [-DestContext <AzureStorageContext>] [-Force]
 [-ServerTimeoutPerRequest <Int32]>] -AbsoluteUri <String> -DestBlob <String> -DestContainer <String>
 [-Confirm] [-WhatIf]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Start-AzureStorageBlobCopy [-SrcBlob] <String> [-ClientTimeoutPerRequest <Int32]>]
 [-ConcurrentTaskCount <Int32]>] [-Context <AzureStorageContext>] [-DestBlob <String>]
 [-DestContext <AzureStorageContext>] [-Force] [-ServerTimeoutPerRequest <Int32]>] -DestContainer <String>
 -SrcContainer <String> [-Confirm] [-WhatIf]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Start-AzureStorageBlobCopy [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-Context <AzureStorageContext>] [-DestContext <AzureStorageContext>] [-Force]
 [-ServerTimeoutPerRequest <Int32]>] -CloudBlob <CloudBlob> -DestCloudBlob <CloudBlob> [-Confirm] [-WhatIf]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Start-AzureStorageBlobCopy [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-Context <AzureStorageContext>] [-DestBlob <String>] [-DestContext <AzureStorageContext>] [-Force]
 [-ServerTimeoutPerRequest <Int32]>] -CloudBlob <CloudBlob> -DestContainer <String> [-Confirm] [-WhatIf]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Start-AzureStorageBlobCopy [-SrcBlob] <String> [-ClientTimeoutPerRequest <Int32]>]
 [-ConcurrentTaskCount <Int32]>] [-Context <AzureStorageContext>] [-DestBlob <String>]
 [-DestContext <AzureStorageContext>] [-Force] [-ServerTimeoutPerRequest <Int32]>]
 -CloudBlobContainer <CloudBlobContainer> -DestContainer <String> [-Confirm] [-WhatIf]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Start-AzureStorageBlobCopy [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-Context <AzureStorageContext>] [-DestBlob <String>] [-DestContext <AzureStorageContext>] [-Force]
 [-ServerTimeoutPerRequest <Int32]>] -DestContainer <String> -SrcFilePath <String> -SrcShareName <String>
 [-Confirm] [-WhatIf]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Start-AzureStorageBlobCopy [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-Context <AzureStorageContext>] [-DestBlob <String>] [-DestContext <AzureStorageContext>] [-Force]
 [-ServerTimeoutPerRequest <Int32]>] -DestContainer <String> -SrcFilePath <String> -SrcShare <CloudFileShare>
 [-Confirm] [-WhatIf]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Start-AzureStorageBlobCopy [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-Context <AzureStorageContext>] [-DestBlob <String>] [-DestContext <AzureStorageContext>] [-Force]
 [-ServerTimeoutPerRequest <Int32]>] -DestContainer <String> -SrcDir <CloudFileDirectory> -SrcFilePath <String>
 [-Confirm] [-WhatIf]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Start-AzureStorageBlobCopy [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-Context <AzureStorageContext>] [-DestContext <AzureStorageContext>] [-Force]
 [-ServerTimeoutPerRequest <Int32]>] -DestCloudBlob <CloudBlob> -SrcFile <CloudFile> [-Confirm] [-WhatIf]
```

### XXXXXXX$XXXXXXXXX$XXX$00
```
Start-AzureStorageBlobCopy [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-Context <AzureStorageContext>] [-DestBlob <String>] [-DestContext <AzureStorageContext>] [-Force]
 [-ServerTimeoutPerRequest <Int32]>] -DestContainer <String> -SrcFile <CloudFile> [-Confirm] [-WhatIf]
```

## XXXXXXXXXXX
Xxx $$Xxxxx$XxxxxXxxxxxxXxxxXxxx$$ xxxxxx xxxxxx xx xxxx x xxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxx x xxxxx xxxx
```
C:\PS>Start-AzureStorageBlobCopy -SrcBlob "ContosoPlanning2015" -DestContainer "ContosoArchives" -SrcContainer "ContosoUploads"
```

Xxxx xxxxxxx xxxxxx xxx xxxx xxxxxxxxx xx xxx xxxx xxxxx XxxxxxxXxxxxxxx0000 xxxx xxx xxxxxxxxx xxxxx XxxxxxxXxxxxxx xx xxx xxxxxxxxx xxxxx XxxxxxxXxxxxxxx.

### Xxxxxxx 0$ Xxx x xxxxxxxxx xx xxxxxxx xxxxx xx xxxx
```
C:\PS>Get-AzureStorageContainer -Name "ContosoUploads" | Start-AzureStorageBlobCopy -SrcBlob "ContosoPlanning2015" -DestContainer "ContosoArchives"
```

Xxxx xxxxxxx xxxx xxx xxxxxxxxx xxxxx XxxxxxxXxxxxxx$ xx xxxxx xxx $$Xxx$XxxxxXxxxxxxXxxxxxxxx$$ xxxxxx$ xxx xxxx xxxxxx xxx xxxxxxxxx xx xxx xxxxxxx xxxxxx xx xxxxx xxx xxxxxxxx xxxxxxxx.
Xxxx xxxxxx xxxxxx xxx xxxx xxxxxxxxx xx xxx xxxx xxxxx XxxxxxxXxxxxxxx0000.
Xxx xxxxxxxx xxxxxx xxxxxxxx xxx xxxxxx xxxxxxxxx.
Xxx $XxxxXxxxxxxxx$ xxxxxxxxx xxxxxxxxx XxxxxxxXxxxxxxx xx xxx xxxxxxxxxxx xxxxxxxxx.

### Xxxxxxx 0$ Xxx x xxxx xx xxxx
```
C:\PS>Get-AzureStorageBlob -Container "ContosoUploads" | Start-AzureStorageBlobCopy -DestContainer "ContosoArchives"
```

Xxxx xxxxxxx xxxx xxx xxxxx xx xxx xxxxxxxxx xxxxx XxxxxxxXxxxxxx$ xx xxxxx xxx $$Xxx$XxxxxXxxxxxxXxxx$$ xxxxxx$ xxx xxxx xxxxxx xxx xxxxxxx xx xxx xxxxxxx xxxxxx xx xxxxx xxx xxxxxxxx xxxxxxxx.
Xxxx xxxxxx xxxxxx xxx xxxx xxxxxxxxx xx xxx xxxxx xx xxx xxxxxxxxx xxxxx XxxxxxxXxxxxxxx.

### Xxxxxxx 0$ Xxxx x xxxx xxxxxxxxx xx xx xxxxxx
```
C:\PS>$SrcBlob = Get-AzureStorageBlob -Container "ContosoUploads" -Blob "ContosoPlanning2015"
C:\PS> $DestBlob = Get-AzureStorageBlob -Container "ContosoArchives" -Blob "ContosoPlanning2015Archived"
C:\PS> Start-AzureStorageBlobCopy -ICloudBlob $SrcBlob.ICloudBlob -DestICloudBlob $DestBlob.ICloudBlob
```

Xxx xxxxx xxxxxxx xxxx xxx xxxx xxxxx XxxxxxxXxxxxxxx0000 xx xxx xxxxxxxxx xxxxx XxxxxxxXxxxxxx.
Xxx xxxxxxx xxxxxx xxxx xxxxxx xx xxx $XxxXxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx xxxx xxxxx XxxxxxxXxxxxxxx0000Xxxxxxxx xx xxx xxxxxxxxx xxxxx XxxxxxxXxxxxxxx.
Xxx xxxxxxx xxxxxx xxxx xxxxxx xx xxx $XxxxXxxx xxxxxxxx.

Xxx xxxx xxxxxxx xxxxxx xxx xxxx xxxxxxxxx xxxx xxx xxxxxx xxxxxxxxx xx xxx xxxxxxxxxxx xxxxxxxxx.
Xxx xxxxxxx xxxx xxxxxxxx xxx xxxxxxxx xx xxxxxxx xxx $$XXxxxxXxxx$$ xxxxxxx xxx xxx $XxxXxxx xxx $XxxxXxxx xxxxx.

### Xxxxxxx 0$ Xxxx x xxxx xxxx x XXX
```
C:\PS>$Context = New-AzureStorageContext -StorageAccountName "ContosoGeneral" -StorageAccountKey "< Storage Key for ContosoGeneral ends with == >"
C:\PS> Start-AzureStorageBlobCopy -AbsoluteUri "http://www.contosointernal.com/planning" -DestContainer "ContosoArchive" -DestBlob "ContosoPlanning2015" -DestContext $Context
```

Xxxx xxxxxxx xxxxxxx x xxxxxxx xxx xxx xxxxxxx xxxxx XxxxxxxXxxxxxx xxxx xxxx xxx xxxxxxxxx xxx$ xxx xxxx xxxxxx xxxx xxx xx xxx $Xxxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxx xxx xxxx xxxx xxx xxxxxxxxx XXX xx xxx xxxx xxxxx XxxxxxxXxxxxxxx xx xxx xxxxxxxxx xxxxx XxxxxxxXxxxxxx.
Xxx xxxxxxx xxxxxx xxx xxxx xxxxxxxxx xx xxx xxxxxxx xxxxxx xx $Xxxxxxx.

## XXXXXXXXXX

### $XxxxxxxxXxx
Xxxxxxxxx xxx xxxxxxxx XXX xx x xxxx xx xxxx xx xx xxxxx$0 Xxxxxxx xxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: SrcUri

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
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
Xxxxxxxxx x $$XxxxxXxxx$$ xxxxxx xxxx xxxxx$0 Xxxxxxx Xxxxxx xxxxxxx.
Xx xxxxxx x $$XxxxxXxxx$$ xxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxx xxxxxx.

```yaml
Type: CloudBlob
Parameter Sets: UNNAMED_PARAMETER_SET_3, UNNAMED_PARAMETER_SET_4
Aliases: SrcICloudBlob,SrcCloudBlob,ICloudBlob

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByValue,ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxXxxxXxxxxxxxx
Xxxxxxxxx x $$XxxxxXxxxXxxxxxxxx$$ xxxxxx xxxx xxx xxxxx$0 Xxxxxxx Xxxxxx xxxxxxx.
Xxxx xxxxxx xxxxxx x xxxx xxxx xxx xxxxxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.
Xx xxxxxx x $$XxxxxXxxxXxxxxxxxx$$ xxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxxxxxxx xxxxxx.

```yaml
Type: CloudBlobContainer
Parameter Sets: UNNAMED_PARAMETER_SET_5
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

### $Xxxxxxx
Xxxxxxxxx xx xxxxx$0 xxxxxxx xxxxxxx.
Xx xxxxxx x xxxxxxx xxxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxxxxx xxxxxx.

```yaml
Type: AzureStorageContext
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: SrcContext

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: AzureStorageContext
Parameter Sets: UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_3, UNNAMED_PARAMETER_SET_4, UNNAMED_PARAMETER_SET_5, UNNAMED_PARAMETER_SET_6, UNNAMED_PARAMETER_SET_7, UNNAMED_PARAMETER_SET_8, UNNAMED_PARAMETER_SET_9, UNNAMED_PARAMETER_SET_10
Aliases: SrcContext

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxxxxx xxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_4, UNNAMED_PARAMETER_SET_5, UNNAMED_PARAMETER_SET_6, UNNAMED_PARAMETER_SET_7, UNNAMED_PARAMETER_SET_8, UNNAMED_PARAMETER_SET_10
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxxxXxxx
Xxxxxxxxx x xxxxxxxxxxx $$XxxxxXxxx$$ xxxxxx

```yaml
Type: CloudBlob
Parameter Sets: UNNAMED_PARAMETER_SET_3, UNNAMED_PARAMETER_SET_9
Aliases: DestICloudBlob

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxxxxxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_4, UNNAMED_PARAMETER_SET_5, UNNAMED_PARAMETER_SET_6, UNNAMED_PARAMETER_SET_7, UNNAMED_PARAMETER_SET_8, UNNAMED_PARAMETER_SET_10
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxxxxx
Xxxxxxxxx xx xxxxx$0 xxxxxxx xxxxxxx.
Xx xxxxxx x xxxxxxx xxxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxxxxx xxxxxx.

```yaml
Type: AzureStorageContext
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxx
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxxxxxx xxx xxxxxxxxxxx xxxx xxxxxxx xxxxxxxxx xxx xxx xxxxxxxxxxxx.

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

### $XxxXxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxx xxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_5
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxXxxxxxxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxXxx
Xxxxxxxxx x $$XxxxxXxxxXxxxxxxxx$$ xxxxxx xxxx xxxxx$0 Xxxxxxx Xxxxxx xxxxxxx.

```yaml
Type: CloudFileDirectory
Parameter Sets: UNNAMED_PARAMETER_SET_8
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxXxxx
Xxxxxxxx x $$XxxxxXxxx$$ xxxxxx xxxx xxxxx$0 Xxxxxxx Xxxxxx xxxxxxx.
Xxx xxx xxxxxx xx xx xxx Xxx$XxxxxXxxxxxxXxxx xxxxxx.

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

### $XxxXxxxXxxx
Xxxxxxxxx xxx xxxxxx xxxx xxxxxxxx xxxx xx xxxxxx xxxxxxxxx xx xxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_6, UNNAMED_PARAMETER_SET_7, UNNAMED_PARAMETER_SET_8
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxXxxxx
Xxxxxxxxx x $$XxxxxXxxxXxxxx$$ xxxxxx xxxx xxxxx$0 Xxxxxxx Xxxxxx xxxxxxx.
Xxx xxx xxxxxx xx xx xxx Xxx$XxxxxXxxxxxxXxxxx xxxxxx.

```yaml
Type: CloudFileShare
Parameter Sets: UNNAMED_PARAMETER_SET_7
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxXxxxxXxxx
Xxxxxxxxx xxx xxxxxx xxxxx xxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_6
Aliases: 

Required: True
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

[Xxx$XxxxxXxxxxxxXxxxXxxxXxxxx](5ead5288-78e9-4ebb-904e-5e86ea88da93)

[Xxxx$XxxxxXxxxxxxXxxxXxxx](c75b9de9-597d-4986-980e-10e49eeef4a7)


