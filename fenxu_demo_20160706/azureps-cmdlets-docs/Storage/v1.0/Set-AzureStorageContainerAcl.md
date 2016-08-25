---
external help file: RMAzure_Storage.xml
online version: 4880a1a4-c947-4310-8317-0a837b8acb7f
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Set-AzureStorageContainerAcl
## XXXXXXXX
Xxxx xxx xxxxxx xxxxxx xxxxxxxxxx xx x xxxxxxx xxxxxxxxx.

## XXXXXX

```
Set-AzureStorageContainerAcl [-Name] <String> [-Permission] [-ClientTimeoutPerRequest <Int32]>]
 [-ConcurrentTaskCount <Int32]>] [-Context <AzureStorageContext>] [-PassThru]
 [-ServerTimeoutPerRequest <Int32]>]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxxxxxxxXxx$$ xxxxxx xxxx xxx xxxxxx xxxxxx xxxxxxxxxx xx xxx xxxxxxxxx xxxxxxx xxxxxxxxx xx xxxxx$0.

## XXXXXXXX

### Xxxxxxx 0$ Xxx xxxxx xxxxxxx xxxxxxxxx XXX xx xxxx
```
PS C:\>Set-AzureStorageContainerAcl -Container "Container01" -Permission Off -PassThru
```

Xxxx xxxxxxx xxxxxxx x xxxxxxxxx xxxx xxx xx xxxxxx xxxxxx.

### Xxxxxxx 0$ Xxx xxxxx xxxxxxx xxxxxxxxx XXX xx xxxxx xxx xxxxxxxx
```
PS C:\>Get-AzureStorageContainer container* | Set-AzureStorageContainerAcl -Permission Blob -PassThru
```

Xxxx xxxxxxx xxxx xxx xxxxxxx xxxxxxxxxx xxxxx xxxx xxxxxx xxxx xxxxxxxxx xxx xxxx xxxxxx xxx xxxxxx xx xxx xxxxxxxx xx xxx xxx xxxxxxxxxx xxx xxxx xxx xx Xxxx xxxxxx.

## XXXXXXXXXX

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
Xxxxxxxxx xxx xxxxx$0 xxxxxxx xxxxxxx.
Xxx xxx xxxxxx xx xx xxxxx xxx Xxx$XxxxxXxxxxxxXxxxxxx xxxxxx.

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

### -Name
Xxxxxxxxx x xxxxxxxxx xxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: N,Container

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByValue,ByPropertyName)
Accept wildcard characters: False
```

### -PassThru
xxxxxxxx

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

### -Permission
Xxxxxxxxx xxx xxxxx xx xxxxxx xxxxxx xx xxxx xxxxxxxxx.
Xx xxxxxxx$ xxx xxxxxxxxx xxx xxx xxxxx xx xx xxx xx xxxxxxxx xxxx xx xxx xxxxx xx xxx xxxxxxx xxxxxxx.
Xx xxxxx xxxxxxxxx xxxxx xxxx xxxxxxxxxxx xx x xxxxxxxxx xxx xxx xxxxx$ xxx xxx xxx xxx xxxxxxxxx xxxxxxxxxxx xx xxxxxx xxxxxx xxxxxx.
Xxxxxxxxx xxxxx xxx xxxx xxxxx xx x xxxxxxxx xxxxxxxxx xxxxxxxxx xxxxxxx xxxxxxxxxxxxxx xxx xxxxxxx.
xxxx$xxxxxxxxxxx

$$Xxxxxxxxx.
Xxxxxxxx xxxx xxxx xxxxxx xx x xxxxxxxxx xxx xxx xxxxx.
Xxxxxxx xxx xxxxxxxxx xxxxx xx xxx xxxxxxxxx xxxxxxx xxxxxxxxx xxxxxxx$ xxx xxxxxx xxxxxxxxx xxxxxxxxxx xx xxx xxxxxxx xxxxxxx. $$Xxxx.
Xxxxxxxx xxxx xxxxxx xx xxxx xxxx xx x xxxxxxxxx xxxxxxx xxxxxxxxx xxxxxxx$ xxx xxxx xxx xxxxxxx xxxxxx xx xxxxxxxxx xxxx.
Xxxxxxx xxxxxx xxxxxxxxx xxxxx xx xxx xxxxxxxxx xx xxxxx xxxxxxxxx xxxxxxx. $$Xxx.
Xxxxxxxxx xxxxxx xx xxxx xxx xxxxxxx xxxxxxx xxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: PublicAccess
Accepted values: Off, Container, Blob

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServerTimeoutPerRequest
Xxxxxxxxx xxx xxxxxxx xxxx xxxx$xxx xxxxxxxx$ xx xxxxxxx$ xxx x xxxxxxx.
Xx xxx xxxxxxxxx xxxxxxxx xxxxxxx xxxxxx xxx xxxxxxx xxxxxxxxx xxx xxxxxxx$ xxx xxxxxxx xxxxxxx xxxxxxx xx xxxxx.
Xxxxxx xxxx xxxx xxx xxx xxxx xxxxxxx.

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

## XXXXX

## XXXXXXX XXXXX

[Get-AzureStorageContainer](4880a1a4-c947-4310-8317-0a837b8acb7f)

[New-AzureStorageContainer](f3da4bf0-aa3a-4853-a362-e3fc479688d6)

[Remove-AzureStorageContainer](89d7ed7c-1db6-4e01-8981-8f34483039fd)


