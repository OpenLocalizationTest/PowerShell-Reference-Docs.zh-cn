---
external help file: RMAzure_Storage.xml
online version: 2cbd0756-0224-43b0-8e22-a7316b7e24c2
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Set-AzureStorageFileContent
## XXXXXXXX
Xxxxxxx xxx xxxxxxxx xx x xxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Set-AzureStorageFileContent [-ShareName] <String> [-Source] <String> [[-Path] <String>]
 [-ClientTimeoutPerRequest <Nullable [System.Int32]>] [-ConcurrentTaskCount <Nullable [System.Int32]>]
 [-Context <AzureStorageContext>] [-Force] [-PassThru] [-ServerTimeoutPerRequest <Nullable [System.Int32]>]
 [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_2
```
Set-AzureStorageFileContent [-Share] <CloudFileShare> [-Source] <String> [[-Path] <String>]
 [-ClientTimeoutPerRequest <Nullable [System.Int32]>] [-ConcurrentTaskCount <Nullable [System.Int32]>] [-Force]
 [-PassThru] [-ServerTimeoutPerRequest <Nullable [System.Int32]>] [-Confirm] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_3
```
Set-AzureStorageFileContent [-Directory] <CloudFileDirectory> [-Source] <String> [[-Path] <String>]
 [-ClientTimeoutPerRequest <Nullable [System.Int32]>] [-ConcurrentTaskCount <Nullable [System.Int32]>] [-Force]
 [-PassThru] [-ServerTimeoutPerRequest <Nullable [System.Int32]>] [-Confirm] [-WhatIf]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxxXxxxxxx$$ xxxxxx xxxxxxx xxx xxxxxxxx xx x xxxx xx x xxxx xx x xxxxxxxxx xxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxxx xx xxx xxxxxxx xxxxxx
```
PS C:\>Set-AzureStorageFileContent â€"ShareName "ContosoShare06" â€"Source "DataFile37" â€"Path "ContosoWorkingFolder/CurrentDataFile"
```

Xxxx xxxxxxx xxxxxxx x xxxx xxxx xx xxxxx XxxxXxxx00 xx xxx xxxxxxx xxxxxx xx x xxxx xxxx xx xxxxx XxxxxxxXxxxXxxx xx xxx xxxxxx xxxxx XxxxxxxXxxxxxxXxxxxx.

### Xxxxxxx 0$ Xxxxxx xxx xxx xxxxx xx xxx xxxxxxx xxxxxx
```
PS C:\>$CurrentFolder = (Get-Item .).FullName
PS C:\> $Container = Get-AzureStorageShare -Name "ContosoShare06"
PS C:\> Get-ChildItem -Recurse | Where-Object { $_.GetType().Name -eq "FileInfo"} | ForEach-Object {
    $path=$_.FullName.Substring($Currentfolder.Length+1).Replace("\","/")
    Set-AzureStorageFileContent -Share $Container -Source $_.FullName -Path $path -Force 
}
```

Xxxx xxxxxxx xxxx xxxxxxx xxxxxx xxxxxxxxxx xxxxxxx xxx xxx xxxxxxx xxxxxx xx xxxxxx xxx xxxxx xxxx xxx xxxxxxx xxxxxx xx xxx xxxx xxxxxx xx xxxxxxxxx XxxxxxxXxxxx00.

Xxx xxxxx xxxxxxx xxxx xxx xxxx xx xxx xxxxxxx xxxxxx xxx xxxxxx xx xx xxx $XxxxxxxXxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx $$Xxx$XxxxxXxxxxxxXxxxx$$ xxxxxx xx xxx xxx xxxx xxxxx xxxxx XxxxxxxXxxxx00$ xxx xxxx xxxxxx xx xx xxx $Xxxxxxxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx xxxxxxxx xx xxx xxxxxxx xxxxxx xxx xxxxxx xxxx xxx xx xxx Xxxxx$Xxxxxx xxxxxx xx xxxxx xxx xxxxxxxx xxxxxxxx.
Xxxx xxxxxx xxxxxxx xxx xxxxxxx xxxx xxx xxx xxxxx$ xxx xxxx xxxxxx xxx xxxxx xx xxx XxxXxxx$Xxxxxx xxxxxx.
Xxxx xxxxxx xxxx x xxxxxx xxxxx xxx xxxx xxxx xxxx xxxxxxx xxx xxxxxxxxxxx xxxx xxx xx xxx xxxx xxxx xxx xxxxxxx xxxxxx xx xxxxxx xxx xxxx.
Xxx xxxxxx xxx xxx xxxx xxxx xxx xxxx xxxxxxxx xxxxxxxx xxxx xxxxxx xx xxx xxxxx xxxxx xxxx xxxx xxxxxxx xxxxxxx.
Xxx xxxx xxxxxxxxxxx xxxxx xxxxxx xxxxxx$ xxxx $$XXXX$Xxxxxxx$$Xxx$Xxxx xxxxx$Xxxxxx$Xxxxxx$$XXXX$Xxxxxxx$$.

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

### -Directory
Xxxxxxxxx x xxxxxx xx x $$XxxxxXxxxXxxxxxxxx$$ xxxxxx.
Xxxx xxxxxx xxxxxxx xxx xxxx xx xxx xxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.
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

### -Force
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

### -PassThru
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

### -Path
$$Xxxx$$

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

### -Share
Xxxxxxxxx x $$XxxxxXxxxXxxxx$$ xxxxxx.
Xxxx xxxxxx xxxxxxx xx x xxxx xx xxx xxxx xxxxx xxxx xxxxxxxxx xxxxxxxxx.
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

### -ShareName
Xxxxxxxxx xxx xxxx xx xxx xxxx xxxxx.
Xxxx xxxxxx xxxxxxx xx x xxxx xx xxx xxxx xxxxx xxxx xxxxxxxxx xxxxxxxxx.

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

### -Source
$$Xxxx$$

```yaml
Type: String
Parameter Sets: (All)
Aliases: FullName

Required: True
Position: 2
Default value: None
Accept pipeline input: True(ByPropertyName)
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

[Remove-AzureStorageDirectory](2cbd0756-0224-43b0-8e22-a7316b7e24c2)

[New-AzureStorageDirectory](2eea330c-759d-4dee-81e9-2e72de9f707e)

[Get-AzureStorageFileContent](7e23b9f6-5f66-49a3-beb8-e2639c5234d7)


