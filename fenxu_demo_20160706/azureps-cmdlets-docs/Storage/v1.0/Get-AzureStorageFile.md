---
external help file: RMAzure_Storage.xml
online version: 7e23b9f6-5f66-49a3-beb8-e2639c5234d7
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Get-AzureStorageFile
## XXXXXXXX
Xxxxx xxxxxxxxxxx xxx xxxxx xxx x xxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Get-AzureStorageFile [-ShareName] <String> [[-Path] <String>]
 [-ClientTimeoutPerRequest <Nullable [System.Int32]>] [-ConcurrentTaskCount <Nullable [System.Int32]>]
 [-Context <AzureStorageContext>] [-ServerTimeoutPerRequest <Nullable [System.Int32]>]
```

### UNNAMED_PARAMETER_SET_2
```
Get-AzureStorageFile [-Share] <CloudFileShare> [[-Path] <String>]
 [-ClientTimeoutPerRequest <Nullable [System.Int32]>] [-ConcurrentTaskCount <Nullable [System.Int32]>]
 [-ServerTimeoutPerRequest <Nullable [System.Int32]>]
```

### UNNAMED_PARAMETER_SET_3
```
Get-AzureStorageFile [-Directory] <CloudFileDirectory> [[-Path] <String>]
 [-ClientTimeoutPerRequest <Nullable [System.Int32]>] [-ConcurrentTaskCount <Nullable [System.Int32]>]
 [-ServerTimeoutPerRequest <Nullable [System.Int32]>]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxx$$ xxxxxx xxxxx xxxxxxxxxxx xxx xxxxx xxx xxx xxxxx xx xxxxxxxxx xxxx xxx xxxxxxx.
Xxxxxxx xxx $Xxxx$ xxxxxxxxx xx xxx xx xxxxxxxx xx x xxxxxxxxx xx xxxx xx xxx xxxxxxxxx xxxx.

Xxxx xxxxxx xxxxxxx $$XxxxxXxxxxxxXxxx$$ xxx $$XxxxxXxxxxxxXxxxxxxxx$$ xxxxxxx.
Xxx xxx xxx xxx $$XxXxxxxxxxx$$ xxxxxxxx xx xxxxxxxxxxx xxxxxxx xxxxxxx xxx xxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxx xxxxxxxxxxx xx x xxxxx
```
PS C:\>Get-AzureStorageFile -ShareName "share1" | where {$_.GetType().Name -eq "CloudFileDirectory"}
```

Xxxx xxxxxxx xxxxx xxxx xxx xxxxxxxxxxx xx xxx xxxxx XxxxxxxXxxxx00.
Xx xxxxx xxxxxxxxx xxxx xxxxx xxx xxxxxxxxxxx$ xxxxxx xxxx xx xxx $$xxxxx$$ xxxxxxxx xx xxxxx xxx xxxxxxxx xxxxxxxx$ xxxx xxxxxxxx xxx xxxxxxx xxxxx xxxx xx xxx $XxxxxXxxxXxxxxxxxx$.

### Xxxxxxx 0$ Xxxx x Xxxx Xxxxxxxxx
```
PS C:\> Get-AzureStorageFile -ShareName "ContosoShare06" â€"Path "ContosoWorkingFolder" | Get-AzureStorageFile
```

Xxxx xxxxxxx xxxxx xxx xxxxx xxx xxxxxxx xx xxx xxxxxxxxx XxxxxxxXxxxxxxXxxxxx xxxxx xxx xxxxx XxxxxxxXxxxx00.
Xx xxxxx xxxx xxx xxxxxxxxx xxxxxxxx$ xxx xxxx xxxxxxxxx xx xx xxx $$Xxx$XxxxxXxxxxxxXxxx$$ xxxxxx xx xxxx xxx xxxxxxxxx.

## XXXXXXXXXX

### -ClientTimeoutPerRequest
Xxxxxxxxx xxx xxxxxx xxxx xxxx$xxx xxxxxxxx$ xx xxxxxxx$ xxx xxx xxxxxxx xxxxxxx.
Xx xxx xxxxxxxx xxxx xxxxx xxxxxx xxx xxxxxxxxx xxxxxxxx$ xxxx xxxxxx xxxxxxx xxx xxxxxxx.
Xx xxxx xxxxxx xxxx xxx xxxxxxx x xxxxxxxxxx xxxxxxxx xxxxxx xxx xxxxxxxx xxxxxxx$ xxxx xxxxxx xxxxxxx xx xxxxx.

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
Xxxxxxxxx xxx xxxxxxx xxxxxxxxxx xxxxxxx xxxxx.
Xxx xxx xxx xxxx xxxxxxxxx xx xxxxx xxx xxxxxxxxxxx xx xxxxxxxx xxxxx XXX xxx xxxxxxxxx xxxxx xx xxxxxxxxxx xxx xxxxxxx xxxxxx xx xxxxxxxxxx xxxxxxx xxxxx.
Xxx xxxxxxxxx xxxxx xx xx xxxxxxxx xxxxx xxx xx xxx xxxxxxxxxx xx xxx xxxx xxxxx.
Xxxx xxxxxxxxx xxx xxxx xxxxxxxx xxxxxxx xxxxxxxxxx xxxxxxxx xx xxx xxxxxxxxx xxxxxxxxxxxx$ xxxx xx 000 xxxxxxxx xxx xxxxxx.
Xxx xxxxxxx xxxxx xx 00.

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
Xxxxxxxxx xx xxxxx$0 Xxxxxxx xxxxxxx.
Xx xxxxxx x Xxxxxxx xxxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxxxxx xxxxxx.

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
Xxxx xxxxxx xxxx xxx xxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.
Xx xxxxxx x xxxxxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxxxxxxx xxxxxx.
Xxx xxx xxxx xxx xxx $$Xxx$XxxxxXxxxxxxXxxx$$ xxxxxx xx xxxxxx x xxxxxxxxx.

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

### -Path
Xxxxxxxxx xxx xxxx xx x xxxxxx.

Xx xxx xxxx xxx $Xxxx$ xxxxxxxxx$ $$Xxx$XxxxxXxxxxxxXxxx$$ xxxxx xxx xxxxxxxxxxx xxx xxxxx xx xxx xxxxxxxxx xxxx xxxxx xx xxxxxxxxx.
Xx xxx xxxxxxx xxx $Xxxx$ xxxxxxxxx$ $$Xxx$XxxxxXxxxxxxXxxx$$ xxxxxxx xx xxxxxxxx xx x xxxxxxxxx xx xxxx xx xxx xxxxxxxxx xxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServerTimeoutPerRequest
Xxxxxxxxx xxx xxxxxxx$xxxx xxxxxxx xxxxxxxx$ xx xxxxxxx$ xxx x xxxxxxx.
Xx xxx xxxxxxxxx xxxxxxxx xxxxxxx xxxxxx xxx xxxxxxx xxxxxxxxx xxx xxxxxxx$ xxx Xxxxxxx xxxxxxx xxxxxxx xx xxxxx.

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
Xxxx xxxxxx xxxx x xxxx xx xxxxxxxxx xxxx xxx xxxx xxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.
Xx xxxxxx x $$XxxxxXxxxXxxxx$$ xxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxxx xxxxxx.
Xxxx xxxxxx xxxxxxxx xxx Xxxxxxx xxxxxxx.
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
Xxxx xxxxxx xxxx x xxxx xx xxxxxxxxx xxxx xxx xxxx xxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

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

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Get-AzureStorageFileContent](7e23b9f6-5f66-49a3-beb8-e2639c5234d7)

[New-AzureStorageDirectory](2eea330c-759d-4dee-81e9-2e72de9f707e)

[Remove-AzureStorageDirectory](2cbd0756-0224-43b0-8e22-a7316b7e24c2)

[Remove-AzureStorageFile](c9eb0c34-12ba-4978-85b5-f52c71e9ddf3)

[Set-AzureStorageFileContent](cd2e0aa7-3259-4aa5-8494-c432063d34e7)


