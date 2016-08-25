---
external help file: RMAzure_Storage.xml
online version: 02217f39-6c93-401b-8801-52fdd38ba751
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Set-AzureStorageServiceLoggingProperty
## XXXXXXXX
Xxxxxxxx xxxxxxx xxx xxxxx$0 Xxxxxxx xxxxxxxx.

## XXXXXX

```
Set-AzureStorageServiceLoggingProperty [-ServiceType] [-Context <AzureStorageContext>]
 [-LoggingOperations <LoggingOperations[]>] [-PassThru] [-RetentionDays <Int32]>] [-Version <Double]>]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxxxxxXxxxxxxXxxxxxxx$$ xxxxxx xxxxxxxx xxxxxxx xxx xxxxx$0 Xxxxxxx xxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx xxxxxxx xxxxxxxxxx xxx xxx Xxxx xxxxxxx
```
C:\PS>Set-AzureStorageServiceLoggingProperty -ServiceType Blob -LoggingOperations Read,Write -PassThru -RetentionDays 10 -Version 1.0
```

Xxxx xxxxxxx xxxxxxxx xxxxxxx 0.0 xxxxxxx xxx xxxx xxxxxxx xx xxxxxxx xxxx xxx xxxxx xxxxxxxxxx.
xxxxx$0 Xxxxxxx xxxxxxx xxxxxxx xxxxxxx xxxxxxx xxx 00 xxxx.
Xxxxxxx xxxx xxxxxxx xxxxxxxxx xxx $XxxxXxxx$ xxxxxxxxx$ xxx xxxxxxx xxxxxxxx xxx xxxxxxxx xxxxxxx xxxxxxxxxx.

## XXXXXXXXXX

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

### -LoggingOperations
Xxxxxxxxx xx xxxxx xx xxxxx$0 Xxxxxxx xxxxxxx xxxxxxxxxx.
xxxxx$0 Xxxxxxx xxxxxxxx xxxx xxx xxxxxxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.
xxxx$xxxxxxxxxxx

$$ Xxxx $$ Xxxx $$ Xxxxx $$ Xxxxxx $$ Xxx

```yaml
Type: LoggingOperations[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxxx xxx xxxxxxx xxxxxxx xxxxxxxxxx.
Xx xxx xx xxx xxxxxxx xxxx xxxxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxx x xxxxx.

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

### -RetentionDays
Xxxxxxxxx xxx xxxxxx xx xxxx xxxx xxx xxxxx$0 Xxxxxxx xxxxxxx xxxxxxx xxxxxx xxxxxxxxxxx.

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

### -ServiceType
Xxxxxxxxx xxx xxxxxxx xxxxxxx xxxx.
Xxxx xxxxxx xxxxxxxx xxx xxxxxxx xxxxxxxxxx xxx xxx xxxxxxx xxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.
xxxx$xxxxxxxxxxx

$$ Xxxx $$ Xxxxx $$ Xxxxx $$ Xxxx

Xxx xxxxx xx Xxxx xx xxx xxxxxxxxx xxxxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Accepted values: Blob, Table, Queue, File

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Version
Xxxxxxxxx xxx xxxxxxx xx xxx xxxxx$0 Xxxxxxx xxxxxxx xxxxxxx.
Xxx xxxxxxx xxxxx xx 0.0.

```yaml
Type: Double]
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

[Get-AzureStorageServiceLoggingProperty](02217f39-6c93-401b-8801-52fdd38ba751)

[New-AzureStorageContext](671aeec8-b7f9-49c5-866f-da84f189ab5b)


