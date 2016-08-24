---
external help file: RMAzure_Storage.xml
online version: d9ec4b6f-fb17-4f29-b209-a3d5f212a6f1
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXxxxxxxXxxxXxxxxxx
## XXXXXXXX
Xxxxxxxxx xxx xxxxxxxx xx x xxxx.

## XXXXXX

### XXXXXXX$XXXXXXXXX$XXX$0
```
Get-AzureStorageFileContent [-ShareName] <String> [-Path] <String> [[-Destination] <String>] [-CheckMd5]
 [-ClientTimeoutPerRequest <Nullable [System.Int32]>] [-ConcurrentTaskCount <Nullable [System.Int32]>]
 [-Context <AzureStorageContext>] [-Force] [-PassThru] [-ServerTimeoutPerRequest <Nullable [System.Int32]>]
 [-Confirm] [-WhatIf]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Get-AzureStorageFileContent [-Share] <CloudFileShare> [-Path] <String> [[-Destination] <String>] [-CheckMd5]
 [-ClientTimeoutPerRequest <Nullable [System.Int32]>] [-ConcurrentTaskCount <Nullable [System.Int32]>] [-Force]
 [-PassThru] [-ServerTimeoutPerRequest <Nullable [System.Int32]>] [-Confirm] [-WhatIf]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Get-AzureStorageFileContent [-Directory] <CloudFileDirectory> [-Path] <String> [[-Destination] <String>]
 [-CheckMd5] [-ClientTimeoutPerRequest <Nullable [System.Int32]>]
 [-ConcurrentTaskCount <Nullable [System.Int32]>] [-Force] [-PassThru]
 [-ServerTimeoutPerRequest <Nullable [System.Int32]>] [-Confirm] [-WhatIf]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Get-AzureStorageFileContent [-File] <CloudFile> [[-Destination] <String>] [-CheckMd5]
 [-ClientTimeoutPerRequest <Nullable [System.Int32]>] [-ConcurrentTaskCount <Nullable [System.Int32]>] [-Force]
 [-PassThru] [-ServerTimeoutPerRequest <Nullable [System.Int32]>] [-Confirm] [-WhatIf]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxxXxxxxxx$$ xxxxxx xxxxxxxxx xxx xxxxxxxx xx x xxxx$ xxx xxxx xxxxx xx xx x xxxxxxxxxxx xxxx xxx xxxxxxx.
Xxxx xxxxxx xxxx xxx xxxxxx xxx xxxxxxxx xx xxx xxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxxxx x xxxx xxxx x xxxxxx
```
PS C:\>Get-AzureStorageFileContent -ShareName "ContosoShare06" -Path "ContosoWorkingFolder/CurrentDataFile"
```

Xxxx xxxxxxx xxxxxxxxx x xxxx xxxx xx xxxxx XxxxxxxXxxxXxxx xx xxx xxxxxx XxxxxxxXxxxxxxXxxxxx xxxx xxx xxxx xxxxx XxxxxxxXxxxx00 xx xxxxxxx xxxxxx.

## XXXXXXXXXX

### $XxxxxXx0
Xx xxx xxxxxxx xxx xxxx xx x xxxx xxxx xxxx xxx xxxxx$ xxxx xxxxxx xxxxxxx xxxx xxxx$ xxx xxxxx xxx xxxxxxxx xx xxx xxx xxxx.
Xx xxx xxxxxxx x xxxx xx x xxxx xxxx xxxxxxx xxxxxx xxx xxx xxxxxxx xxx $Xxxxx$ xxxxxxxxx$ xxx xxxxxx xxxxxxxxxx xxx xxxx.
Xx xxx xxxxxxx x xxxx xx xx xxxxxxxx xxxx xxx xxx xx xxx xxxxxxx $Xxxxx$$ xxx xxxxxx xxxxxxx xxx xxxxxx xx xxxxxxxxx.

Xx xxx xxxxxxx xxx xxxx xx x xxxxxx$ xxxx xxxxxx xxxxxxxx xx xxxxxx x xxxx xxxx xxx xxx xxxx xx xxx Xxxxx xxxxxxx xxxx.

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
Xx xxx xxxxxxx xxx xxxx xx x xxxx xxxx xxxx xxx xxxxx$ xxxx xxxxxx xxxxxxx xxxx xxxx$ xxx xxxxx xxx xxxxxxxx xx xxx xxx xxxx.
Xx xxx xxxxxxx x xxxx xx x xxxx xxxx xxxxxxx xxxxxx xxx xxx xxxxxxx xxx $Xxxxx$ xxxxxxxxx$ xxx xxxxxx xxxxxxxxxx xxx xxxx.
Xx xxx xxxxxxx x xxxx xx xx xxxxxxxx xxxx xxx xxx xx xxx xxxxxxx $Xxxxx$$ xxx xxxxxx xxxxxxx xxx xxxxxx xx xxxxxxxxx.

Xx xxx xxxxxxx xxx xxxx xx x xxxxxx$ xxxx xxxxxx xxxxxxxx xx xxxxxx x xxxx xxxx xxx xxx xxxx xx xxx Xxxxx xxxxxxx xxxx.

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

### $XxxxxxxxxxXxxxXxxxx
Xx xxx xxxxxxx xxx xxxx xx x xxxx xxxx xxxx xxx xxxxx$ xxxx xxxxxx xxxxxxx xxxx xxxx$ xxx xxxxx xxx xxxxxxxx xx xxx xxx xxxx.
Xx xxx xxxxxxx x xxxx xx x xxxx xxxx xxxxxxx xxxxxx xxx xxx xxxxxxx xxx $Xxxxx$ xxxxxxxxx$ xxx xxxxxx xxxxxxxxxx xxx xxxx.
Xx xxx xxxxxxx x xxxx xx xx xxxxxxxx xxxx xxx xxx xx xxx xxxxxxx $Xxxxx$$ xxx xxxxxx xxxxxxx xxx xxxxxx xx xxxxxxxxx.

Xx xxx xxxxxxx xxx xxxx xx x xxxxxx$ xxxx xxxxxx xxxxxxxx xx xxxxxx x xxxx xxxx xxx xxx xxxx xx xxx Xxxxx xxxxxxx xxxx.

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

### $Xxxxxxx
Xx xxx xxxxxxx xxx xxxx xx x xxxx xxxx xxxx xxx xxxxx$ xxxx xxxxxx xxxxxxx xxxx xxxx$ xxx xxxxx xxx xxxxxxxx xx xxx xxx xxxx.
Xx xxx xxxxxxx x xxxx xx x xxxx xxxx xxxxxxx xxxxxx xxx xxx xxxxxxx xxx $Xxxxx$ xxxxxxxxx$ xxx xxxxxx xxxxxxxxxx xxx xxxx.
Xx xxx xxxxxxx x xxxx xx xx xxxxxxxx xxxx xxx xxx xx xxx xxxxxxx $Xxxxx$$ xxx xxxxxx xxxxxxx xxx xxxxxx xx xxxxxxxxx.

Xx xxx xxxxxxx xxx xxxx xx x xxxxxx$ xxxx xxxxxx xxxxxxxx xx xxxxxx x xxxx xxxx xxx xxx xxxx xx xxx Xxxxx xxxxxxx xxxx.

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

### $Xxxxxxxxxxx
Xxxxxxxxx xxx xxxxxxxxxxx xxxx.
Xxxx xxxxxx xxxxxxxxx xxx xxxx xxxxxxxx xx xxx xxxxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

Xx xxx xxxxxxx xxx xxxx xx x xxxx xxxx xxxx xxx xxxxx$ xxxx xxxxxx xxxxxxx xxxx xxxx$ xxx xxxxx xxx xxxxxxxx xx xxx xxx xxxx.
Xx xxx xxxxxxx x xxxx xx x xxxx xxxx xxxxxxx xxxxxx xxx xxx xxxxxxx xxx $Xxxxx$ xxxxxxxxx$ xxx xxxxxx xxxxxxxxxx xxx xxxx.
Xx xxx xxxxxxx x xxxx xx xx xxxxxxxx xxxx xxx xxx xx xxx xxxxxxx $Xxxxx$$ xxx xxxxxx xxxxxxx xxx xxxxxx xx xxxxxxxxx.

Xx xxx xxxxxxx xxx xxxx xx x xxxxxx$ xxxx xxxxxx xxxxxxxx xx xxxxxx x xxxx xxxx xxx xxx xxxx xx xxx Xxxxx xxxxxxx xxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxxxx
Xxxxxxxxx x xxxxxx xx x $$XxxxxXxxxXxxxxxxxx$$ xxxxxx.
Xxxx xxxxxx xxxx xxxxxxx xxx x xxxx xx xxx xxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.
Xx xxxxxx x xxxxxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxxxxxxx xxxxxx.
Xxx xxx xxxx xxx xxx Xxx$XxxxxXxxxxxxXxxx xxxxxx xx xxxxxx x xxxxxxxxx.

```yaml
Type: CloudFileDirectory
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByValue)
Accept wildcard characters: False
```

### $Xxxx
Xxxxxxxxx x xxxx xx x $$XxxxxXxxx$$ xxxxxx.
Xxxx xxxxxx xxxx xxx xxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.
Xx xxxxxx x $$XxxxxXxxx$$ xxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxx xxxxxx.

```yaml
Type: CloudFile
Parameter Sets: UNNAMED_PARAMETER_SET_4
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByValue)
Accept wildcard characters: False
```

### $Xxxxx
Xx xxx xxxxxxx xxx xxxx xx x xxxx xxxx xxxx xxx xxxxx$ xxxx xxxxxx xxxxxxx xxxx xxxx$ xxx xxxxx xxx xxxxxxxx xx xxx xxx xxxx.
Xx xxx xxxxxxx x xxxx xx x xxxx xxxx xxxxxxx xxxxxx xxx xxx xxxxxxx xxx $Xxxxx$ xxxxxxxxx$ xxx xxxxxx xxxxxxxxxx xxx xxxx.
Xx xxx xxxxxxx x xxxx xx xx xxxxxxxx xxxx xxx xxx xx xxx xxxxxxx $Xxxxx$$ xxx xxxxxx xxxxxxx xxx xxxxxx xx xxxxxxxxx.

Xx xxx xxxxxxx xxx xxxx xx x xxxxxx$ xxxx xxxxxx xxxxxxxx xx xxxxxx x xxxx xxxx xxx xxx xxxx xx xxx Xxxxx xxxxxxx xxxx.

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
Xx xxx xxxxxxx xxx xxxx xx x xxxx xxxx xxxx xxx xxxxx$ xxxx xxxxxx xxxxxxx xxxx xxxx$ xxx xxxxx xxx xxxxxxxx xx xxx xxx xxxx.
Xx xxx xxxxxxx x xxxx xx x xxxx xxxx xxxxxxx xxxxxx xxx xxx xxxxxxx xxx $Xxxxx$ xxxxxxxxx$ xxx xxxxxx xxxxxxxxxx xxx xxxx.
Xx xxx xxxxxxx x xxxx xx xx xxxxxxxx xxxx xxx xxx xx xxx xxxxxxx $Xxxxx$$ xxx xxxxxx xxxxxxx xxx xxxxxx xx xxxxxxxxx.

Xx xxx xxxxxxx xxx xxxx xx x xxxxxx$ xxxx xxxxxx xxxxxxxx xx xxxxxx x xxxx xxxx xxx xxx xxxx xx xxx Xxxxx xxxxxxx xxxx.

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

### $Xxxx
Xxxxxxxxx xxx xxxx xx x xxxx.
Xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.
Xx xxx xxxx xxxx xxx xxxxx$ xxxx xxxxxx xxxxxxx xx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_3
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxXxxxxxxXxxXxxxxxx
Xx xxx xxxxxxx xxx xxxx xx x xxxx xxxx xxxx xxx xxxxx$ xxxx xxxxxx xxxxxxx xxxx xxxx$ xxx xxxxx xxx xxxxxxxx xx xxx xxx xxxx.
Xx xxx xxxxxxx x xxxx xx x xxxx xxxx xxxxxxx xxxxxx xxx xxx xxxxxxx xxx $Xxxxx$ xxxxxxxxx$ xxx xxxxxx xxxxxxxxxx xxx xxxx.
Xx xxx xxxxxxx x xxxx xx xx xxxxxxxx xxxx xxx xxx xx xxx xxxxxxx $Xxxxx$$ xxx xxxxxx xxxxxxx xxx xxxxxx xx xxxxxxxxx.

Xx xxx xxxxxxx xxx xxxx xx x xxxxxx$ xxxx xxxxxx xxxxxxxx xx xxxxxx x xxxx xxxx xxx xxx xxxx xx xxx Xxxxx xxxxxxx xxxx.

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

### $Xxxxx
Xxxxxxxxx x $$XxxxxXxxxXxxxx$$ xxxxxx.
Xxxx xxxxxx xxxxxxxxx xxx xxxxxxxx xx xxx xxxx xx xxx xxxxx xxxx xxxxxxxxx xxxxxxxxx.
Xx xxxxxx x $$XxxxxXxxxXxxxx$$ xxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxxx xxxxxx.
Xxxx xxxxxx xxxxxxxx xxx xxxxxxx xxxxxxx.
Xx xxx xxxxxxx xxxx xxxxxxxxx$ xx xxx xxxxxxx xxx $Xxxxxxx$ xxxxxxxxx.

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

### $XxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxx xxxx xxxxx.
Xxxx xxxxxx xxxxxxxxx xxx xxxxxxxx xx xxx xxxx xx xxx xxxxx xxxx xxxxxxxxx xxxxxxxxx.

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

[Xxx$XxxxxXxxxxxxXxxx](d9ec4b6f-fb17-4f29-b209-a3d5f212a6f1)

[Xxx$XxxxxXxxxxxxXxxxXxxxxxx](cd2e0aa7-3259-4aa5-8494-c432063d34e7)


