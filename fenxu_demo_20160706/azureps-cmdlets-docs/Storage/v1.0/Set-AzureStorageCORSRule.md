---
external help file: RMAzure_Storage.xml
online version: accfb0fd-ad3a-4415-abce-a98b8073e82b
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXxxxxxxXXXXXxxx
## XXXXXXXX
Xxxx xxx XXXX xxxxx xxx x xxxx xx Xxxxxxx xxxxxxx.

## XXXXXX

```
Set-AzureStorageCORSRule [-ServiceType] [-ClientTimeoutPerRequest <Int32]>] [-ConcurrentTaskCount <Int32]>]
 [-Context <AzureStorageContext>] [-PassThru] [-ServerTimeoutPerRequest <Int32]>] -CorsRules <PSCorsRule[]>
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXXXXXxxx$$ xxxxxx xxxx xxx Xxxxx$Xxxxxx Xxxxxxxx Xxxxxxx $XXXX$ xxxxx xxx x xxxx xx xxxxx$0 Xxxxxxx xxxxxxx.
Xxx xxxxx xx xxxxxxx xxxxxxxx xxx xxxx xxxxxx xxx Xxxx$ Xxxxx$ Xxxxx$ xxx Xxxx.
Xxxx xxxxxx xxxxxxxxxx xxx xxxxxxxx xxxxx.
Xx xxx xxx xxxxxxx xxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXXXXXxxx xxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx XXXX xxxxx xx xxx xxxx xxxxxxx
```
PS C:\>$CorsRules = (@{
    AllowedHeaders=@("x-ms-blob-content-type","x-ms-blob-content-disposition");
    AllowedOrigins=@("*");
    MaxAgeInSeconds=30;
    AllowedMethods=@("Get","Connect")},
    @{
    AllowedOrigins=@("http://www.fabrikam.com","http://www.contoso.com"); 
    ExposedHeaders=@("x-ms-meta-data*","x-ms-meta-customheader"); 
    AllowedHeaders=@("x-ms-meta-target*","x-ms-meta-customheader");
    MaxAgeInSeconds=30;
    AllowedMethods=@("Put")})
PS C:\> Set-AzureStorageCORSRule -ServiceType Blob -CorsRules $CorsRules
```

Xxx xxxxx xxxxxxx xxxxxxx xx xxxxx xx xxxxx xx xxx $XxxxXxxxx xxxxxxxx.
Xxxx xxxxxxx xxxx xxxxxxxx xxxxxxx xxxx xxxxxxx xxxxx xx xxxx xxxx xxxxx.

Xxx xxxxxx xxxxxxx xxxxxxx xxx xxxxx xx $XxxxXxxxx xx xxx Xxxx xxxxxxx xxxx.

### Xxxxxxx 0$ Xxxxxx xxxxxxxxxx xx x XXXX xxxx xxx xxxx xxxxxxx
```
PS C:\>$CorsRules = Get-AzureStorageCORSRule -ServiceType Blob
PS C:\> $CorsRules[0].AllowedHeaders = @("x-ms-blob-content-type", "x-ms-blob-content-disposition")
PS C:\> $CorsRules[0].AllowedMethods = @("Get", "Connect", "Merge")
PS C:\> Set-AzureStorageCORSRule -ServiceType Blob -CorsRules $CorsRules
```

Xxx xxxxx xxxxxxx xxxx xxx xxxxxxx XXXX xxxxx xxx xxx Xxxx xxxx xx xxxxx xxx $$Xxx$XxxxxXxxxxxxXXXXXxxx$$ xxxxxx.
Xxx xxxxxxx xxxxxx xxx xxxxx xx xxx $XxxxXxxxx xxxxx xxxxxxxx.

Xxx xxxxxx xxx xxxxx xxxxxxxx xxxxxx xxx xxxxx xxxx xx $XxxxXxxxx.

Xxx xxxxx xxxxxxx xxxxxxx xxx xxxxx xx $XxxxXxxxx xx xxx Xxxx xxxxxxx xxxx.
Xxx xxxxxxx xxxxx xxxxxxxxx xxx xxxxxxx XXXX xxxxx.

## XXXXXXXXXX

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

### $Xxxxxxx
Xxxxxxxxx xx xxxxx$0 Xxxxxxx xxxxxxx.
Xx xxxxxx x xxxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxxxxx xxxxxx.

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

### $XxxxXxxxx
Xxxxxxxxx xx xxxxx xx XXXX xxxxx.
Xxx xxx xxxxxxxx xxx xxxxxxxx xxxxx xxxxx xxx Xxx$XxxxxXxxxxxxXXXXXxxx xxxxxx.

```yaml
Type: PSCorsRule[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxx
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxxx x Xxxxxxx xxxx xxxxxxxx xxx xxxxxxx xx xxx xxxxxxxxx.
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

### $XxxxxxxXxxx
Xxxxxxxxx xxx xxxxx$0 Xxxxxxx xxxxxxx xxxx xxx xxxxx xxxx xxxxxx xxxxxxx xxxxx.
xxxx$xxxxxxxxxxx

$$ Xxxx $$ Xxxxx $$ Xxxxx $$ Xxxx

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

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Xxx$XxxxxXxxxxxxXXXXXxxx](accfb0fd-ad3a-4415-abce-a98b8073e82b)

[Xxx$XxxxxXxxxxxxXxxxxxx](671aeec8-b7f9-49c5-866f-da84f189ab5b)

[Xxxxxx$XxxxxXxxxxxxXXXXXxxx](ea872c93-797e-49a5-8e97-640a56aadceb)


