---
external help file: RMAzure_Storage.xml
online version: 15371eb7-da6a-4b26-bbda-b59a2eeedb1d
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXxxxxxxXxxx
## XXXXXXXX
Xxxxx xxxxx xx x xxxxxxxxx.

## XXXXXX

### XXXXXXX$XXXXXXXXX$XXX$0
```
Get-AzureStorageBlob [[-Blob] <String>] [-Container] <String> [-ClientTimeoutPerRequest <Int32]>]
 [-ConcurrentTaskCount <Int32]>] [-Context <AzureStorageContext>] [-ContinuationToken <BlobContinuationToken>]
 [-MaxCount <Int32]>] [-ServerTimeoutPerRequest <Int32]>]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Get-AzureStorageBlob [-Container] <String> [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-Context <AzureStorageContext>] [-ContinuationToken <BlobContinuationToken>] [-MaxCount <Int32]>]
 [-Prefix <String>] [-ServerTimeoutPerRequest <Int32]>]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxx$$ xxxxxx xxxxx xxxxx xx xxx xxxxxxxxx xxxxxxxxx xx xx Xxxxx xxxxxxx xxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx x xxxx xx xxxx xxxx
```
PS C:\>Get-AzureStorageBlob -Container "ContainerName" -Blob blob*
```

Xxxx xxxxxxx xxxx x xxxx xxxx xxx xxxxxxxx xx xxx x xxxx.

### Xxxxxxx 0$ Xxx x xxxx xx xxxxx xxx xxxxxxxx
```
PS C:\>Get-AzureStorageContainer -Name container* | Get-AzureStorageBlob
```

Xxxx xxxxxxx xxxx xxx xxxxxxxx xx xxx x xxxx.

### Xxxxxxx 0$ Xxx x xxxx xx xxxx xxxxxx
```
PS C:\>Get-AzureStorageBlob -Container "ContainerName" -Prefix "blob"
```

Xxxx xxxxxxx xxxx x xxxx xxxxxx xx xxx x xxxx.

### Xxxxxxx 0$ Xxxx xxxxx xx xxxxxxxx xxxxxxx
```
PS C:\>$MaxReturn = 10000
PS C:\> $ContainerName = "abc"
PS C:\> $Total = 0
PS C:\> $Token = $Null
PS C:\> do
 {
     $Blobs = Get-AzureStorageBlob -Container $ContainerName -MaxCount $MaxReturn  -ContinuationToken $Token
     $Total += $Blobs.Count
     if($Blobs.Length -le 0) { Break;}
     $Token = $Blobs[$blobs.Count -1].ContinuationToken;
 }
 While ($Token -ne $Null)
PS C:\> Echo "Total $Total blobs in container $ContainerName"
```

Xxxx xxxxxxx xxxx xxx $XxxXxxxx$ xxx $XxxxxxxxxxxxXxxxx$ xxxxxxxxxx xx xxxx xxxxx$0 Xxxxxxx xxxxx xx xxxxxxxx xxxxxxx.
Xxx xxxxx xxxx xxxxxxxx xxxxxx xxxxxx xx xxxxxxxxx xx xxx xx xxx xxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxxxx x $$Xx$Xxxxx$$ xxxxxxxxx xxxx xxxx xxx $$Xxx$XxxxxXxxxxxxXxxx$$ xxxxxx xx xxx xxxxx.
Xxx xxxxxxxxx xxxxxxxx xxx xxxxxxxxxxxx xxxxx xxxxxx xx xxx $Xxxxx xxxxxxxx.
$Xxxxx xxxxxxx xxxxx xx xxx xxxx xxxx.
Xxx xxxx xxxxxxxxxxx$ xxxx $$XXXX$Xxxxxxx$$Xxx$Xxxx Xxxxx$Xx$$XXXX$Xxxxxxx$$.

Xxx xxxxx xxxxxxx xxxx xxx $$Xxxx$$ xxxxxxx xx xxxxxxx xxx xxxxx.

## XXXXXXXXXX

### $Xxxx
Xxxxxxxxx x xxxx xx xxxx xxxxxxx$ xxxxx xxx xx xxxx xxx x xxxxxxxx xxxxxx.
Xx xx xxxx xxxx xx xxxxxxxxx$ xxx xxxxxx xxxxx xxx xxx xxxxx xx xxx xxxxxxxxx xxxxxxxxx.
Xx x xxxxx xx xxxxxxxxx xxx xxxx xxxxxxxxx$ xxx xxxxxx xxxxx xxx xxxxx xxxx xxxxx xxxx xxxxx xxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
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
Parameter Sets: (All)
Aliases: N,Name

Required: True
Position: 2
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $Xxxxxxx
Xxxxxxxxx xxx Xxxxx xxxxxxx xxxxxxx xxxx xxxxx xxx xxxx xx xxx x xxxx xx xxxxx.
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

### $XxxxxxxxxxxxXxxxx
Xxxxxxxxx x xxxxxxxxxxxx xxxxx xxx xxx xxxx xxxx.
Xxx xxxx xxxxxxxxx xxx xxx $XxxXxxxx$ xxxxxxxxx xx xxxx xxxxx xx xxxxxxxx xxxxxxx.

```yaml
Type: BlobContinuationToken
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxXxxxx
Xxxxxxxxx xxx xxxxxxx xxxxxx xx xxxxxxx xxxx xxxx xxxxxx xxxxxxx.

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

### $Xxxxxx
Xxxxxxxxx x xxxxxx xxx xxx xxxx xxxxx xxxx xxx xxxx xx xxx.
Xxxx xxxxxxxxx xxxx xxx xxxxxxx xxxxx xxxxxxx xxxxxxxxxxx xx xxxxxxxx xxxxxxxxxx xx xxxxxx.
Xxxx xxxxx xxxx xx xxx xxxxxxxxx xxx xxxx xxxxx xxxxx $Xx$$ $XxXxxx0$$ xxx $XxXxxx0$ xxx xxx xxxxxxx $$Xxxxxx Xx$$$ xxx xxxxxx xxxxxxx xx xxxxx.
Xxxxxxx$ xx xxx xxxxxxx $$Xxxxxx Xx$$ xxx xxxxxx xxxxxxx $Xx$$ $XxXxxx0$$ xxx $XxXxxx0$.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
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

## XXXXXX

## XXXXXXX

### XxxxxXxxxxxxXxxx

## XXXXX
XXXXXXXX

## XXXXXXX XXXXX

[Xxx$XxxxxXxxxxxxXxxxXxxxxxx](15371eb7-da6a-4b26-bbda-b59a2eeedb1d)

[Xxxxxx$XxxxxXxxxxxxXxxx](fddc1b9e-caf4-47d7-a6b2-a2b2bb50113a)

[Xxx$XxxxxXxxxxxxXxxxXxxxxxx](c3d50900-70d6-44af-b939-abe86fcf89e6)


