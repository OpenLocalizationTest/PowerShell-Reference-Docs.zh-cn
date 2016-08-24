---
external help file: RMAzure_Storage.xml
online version: f08d2de2-a276-439c-b9a8-ee187a8c334e
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXxxxxxxXxxxxxxXXXXxxxx
## XXXXXXXX
Xxxxxxx xx XXX xxxxx.

## XXXXXX

```
New-AzureStorageAccountSASToken [-Context <AzureStorageContext>] [-ExpiryTime <DateTime>]
 [-IPAddressOrRange <String>] [-Permission <String>] [-Protocol <SharedAccessProtocol>] [-StartTime <DateTime>]
 [-ResourceType] [-Service]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXXXXxxxx$$ xxxxxx xxxxxxx xx xxxxxxx$xxxxx xxxxxx xxxxxx xxxxxxxxx $XXX$ xxxxx xxx xx xxxxx$0 Xxxxxxx xxxxxxx.

Xxx xxx xxx xxx XXX xxxxx xx xxxxxxxx xxxxxxxxxxx xxx xxxxxxxx xxxxxxxx$ xx xx xxxxxxxx xxxxxxxxxxx xxx xxxxxxxx xxx xxxxxxxxx xxxx xx xxxxxx$xxxxx XXX xxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx xx XXX xxxxx
```
PS C:\> New-AzureStorageAccountSASToken -Service Blob,File,Table,Queue -ResourceType Service,Container,Object -Permission "racwdlup"
```

Xxxx xxxxxxx xxxxxxx xx xxxxxxx$xxxxx XXX xxxxx xxxx xxxx xxxxxxxxxx.

### Xxxxxxx 0$ Xxxxxx xx XXX xxxxx xxx x xxxxx xx XX xxxxxxxxx
```
PS C:\> New-AzureStorageAccountSASToken -Service Blob,File,Table,Queue -ResourceType Service,Container,Object -Permission "racwdlup" -Protocol HttpsOnly -IPAddressOrRange 168.1.5.60-168.1.5.70
```

Xxxx xxxxxxx xxxxxxx xx XXX xxxxx xxx XXXXX$xxxx xxxxxxxx xxxx xxx xxxxxxxxx xxxxx xx XX xxxxxxxxx.

## XXXXXXXXXX

### $Xxxxxxx
Xxxxxxxxx xxx xxxxx$0 xxxxxxx xxxxxxx.
Xxx xxx xxx xxx Xxx$XxxxxXxxxxxxXxxxxxx xxxxxx xx xxx xx $$XxxxxXxxxxxxXxxxxxx$$ xxxxxx.

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

### $XxxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxxxx xxx xxxxxx xxxxxx xxxxxxxxx xxxxxxx xxxxxxx.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XXXxxxxxxXxXxxxx
Xxxxxxxxx xxx XX xxxxxxx xx xxxxx xx XX xxxxxxxxx xxxx xxxxx xx xxxxxx xxxxxxxx$ xxxx xx 000.0.0.00 xx 000.0.0.00$000.0.0.00.
Xxx xxxxx xx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxxxxx
Xxxxxxxxx xxx xxxxxxxxxxx xxx Xxxxxxx xxxxxxx.
Xxxxxxxxxxx xxx xxxxx xxxx xx xxxx xxxxx xxx xxxxxxxxx xxxxxxxx xxxx.
Xxx xxxx xxxxxxxxxxx xxxxx xxxxxxxxxx xxxxxxxxxx xxxxxx$ xxx Xxxxxxxxxxxx xx Xxxxxxx XXXxxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXx$000000

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxxx
Xxxxxxxxx xxx xxxxxxxx xxxxxxxxx xxx x xxxxxxx xxxx xxxx xxx xxxxxxx XXX.
xxxx$xxxxxxxxxxx

$$ XxxxxXxxx $$ XxxxxXxXxxx

Xxx xxxxxxx xxxxx xx XxxxxXxXxxx.

```yaml
Type: SharedAccessProtocol
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxXxxx
Xxxxxxxxx xxx xxxxxxxx xxxxx xxxx xxx xxxxxxxxx xxxx xxx XXX xxxxx.
xxxx$xxxxxxxxxxx

$$ Xxxx $$ Xxxxxxx $$ Xxxxxxxxx $$ Xxxxxx

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Accepted values: None, Service, Container, Object

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxx
Xxxxxxxxx xxx xxxxxxx.
xxxx$xxxxxxxxxxx

$$ Xxxx $$ Xxxx $$ Xxxx $$ Xxxxx $$ Xxxxx

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Accepted values: None, Blob, File, Queue, Table

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxXxxx
Xxxxxxxxx xxx xxxx$ xx x $$XxxxXxxx$$ xxxxxx$ xx xxxxx xxx XXX xxxxxxx xxxxx.
Xx xxx x $$XxxxXxxx$$ xxxxxx$ xxx xxx Xxx$Xxxx xxxxxx.

```yaml
Type: DateTime
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

[Xxx$XxxxxXxxxxxxXxxxXXXXxxxx](f08d2de2-a276-439c-b9a8-ee187a8c334e)

[Xxx$XxxxxXxxxxxxXxxxxxxxxXXXXxxxx](dc3564e2-9ede-4901-8d62-f49017a03281)

[Xxx$XxxxxXxxxxxxXxxxXXXXxxxx](4fb064f5-94bc-4d8f-9ef6-2611f8aab99c)

[Xxx$XxxxxXxxxxxxXxxxxXXXXxxxx](6cae6e32-2800-4c20-88ae-d40271476628)

[Xxx$XxxxxXxxxxxxXxxxxXXXXxxxx](07c8ad4e-7a32-4407-9120-1432126b7376)

[Xxx$XxxxxXxxxxxxXxxxxXXXXxxxx](abee1cab-f04a-400e-8fb1-caed1ee02ee7)


