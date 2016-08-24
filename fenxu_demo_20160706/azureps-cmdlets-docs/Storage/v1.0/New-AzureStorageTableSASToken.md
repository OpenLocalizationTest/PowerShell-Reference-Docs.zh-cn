---
external help file: RMAzure_Storage.xml
online version: 671aeec8-b7f9-49c5-866f-da84f189ab5b
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXxxxxxxXxxxxXXXXxxxx
## XXXXXXXX
Xxxxxxxxx xx XXX xxxxx xxx xx xxxxx$0 Xxxxxxx xxxxx.

## XXXXXX

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureStorageTableSASToken [-Name] <String> [-Context <AzureStorageContext>] [-EndPartitionKey <String>]
 [-EndRowKey <String>] [-ExpiryTime <DateTime]>] [-FullUri] [-IPAddressOrRange <String>]
 [-Protocol <Nullable [Microsoft.WindowsAzure.Storage.SharedAccessProtocol]>] [-StartPartitionKey <String>]
 [-StartRowKey <String>] [-StartTime <DateTime]>] -Policy <String>
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureStorageTableSASToken [-Name] <String> [-Context <AzureStorageContext>] [-EndPartitionKey <String>]
 [-EndRowKey <String>] [-ExpiryTime <DateTime]>] [-FullUri] [-IPAddressOrRange <String>] [-Permission <String>]
 [-Protocol <Nullable [Microsoft.WindowsAzure.Storage.SharedAccessProtocol]>] [-StartPartitionKey <String>]
 [-StartRowKey <String>] [-StartTime <DateTime]>]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxxxXXXXxxxx$$ xxxxxx xxxxxxxxx x Xxxxxx Xxxxxx Xxxxxxxxx $XXX$ xxxxx xxx xx xxxxx$0 Xxxxxxx xxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxxxx xx XXX xxxxx xxxx xxx xxxx xxxxxxxxxxx xxx x xxxxx
```
C:\PS>New-AzureStorageTableSASToken -Name "ContosoResources" -Permission "raud"
```

Xxxx xxxxxxx xxxxxxxxx xx XXX xxxxx xxxx xxxx xxxxxxxxxxx xxx xxx xxxxx xxxxx XxxxxxxXxxxxxxxx.
Xxxx xxxxx xx xxx xxxx$ xxx$ xxxxxx$ xxx xxxxxx xxxxxxxxxxx.

### Xxxxxxx 0$ Xxxxxxxx xx XXX xxxxx xxx x xxxxx xx xxxxxxxxxx
```
C:\PS>New-AzureStorageTableSASToken -Name "ContosoResources" -Permission "raud" -StartPartitionKey "a" -EndPartitionKey "b"
```

Xxxx xxxxxxx xxxxxxxxx xxx XXX xxxxx xxxx xxxx xxxxxxxxxxx xxx xxx xxxxx xxxxx XxxxxxxXxxxxxxxx.
Xxx xxxxxxx xxxxxx xxx xxxxx xx xxx xxxxx xxxx xxx $XxxxxXxxxxxxxxXxx$ xxx $XxxXxxxxxxxxXxx$ xxxxxxxxxx xxxxxxx.

### Xxxxxxx 0$ Xxxxxxxx xx XXX xxxxx xxxx xxx x xxxxxx xxxxxx xxxxxx xxx x xxxxx
```
C:\PS>New-AzureStorageTableSASToken -Name "ContosoResources" -Policy "ClientPolicy01"
```

Xxxx xxxxxxx xxxxxxxxx xx XXX xxxxx xxx xxx xxxxx xxxxx XxxxxxxXxxxxxxxx.
Xxx xxxxxxx xxxxxxxxx xxx xxxxxx xxxxxx xxxxxx xxxxx XxxxxxXxxxxx00.

## XXXXXXXXXX

### $Xxxxxxx
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

### $XxxXxxxxxxxxXxx
Xxxxxxxxx xxx xxxxxxxxx xxx xx xxx xxx xx xxx xxxxx xxx xxx xxxxx xxxx xxxx xxxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: endpk

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxXxxXxx
Xxxxxxxxx xxx xxx xxx xxx xxx xxx xx xxx xxxxx xxx xxx xxxxx xxxx xxxx xxxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: endrk

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxXxxx
Xxxxxxxxx xxxx xxx XXX xxxxx xxxxxxx.

```yaml
Type: DateTime]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxx
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxxx xxx xxxx xxxxx XXX xxxx xxx XXX xxxxx.

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

### $XXXxxxxxxXxXxxxx
$$Xxxx$$

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

### $Xxxx
Xxxxxxxxx xxx xxxx xx xx xxxxx$0 Xxxxxxx xxxxx.
Xxxx xxxxxx xxxxxxx xx XXX xxxxx xxx xxx xxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: N,Table

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByValue,ByPropertyName)
Accept wildcard characters: False
```

### $Xxxxxxxxxx
Xxxxxxxxx xxxxxxxxxxx xxx xx xxxxx$0 Xxxxxxx xxxxx.

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

### $Xxxxxx
Xxxxxxxxx x xxxxxx xxxxxx xxxxxx$ xxxxx xxxxxxxx xxx xxxxxxxxxxx xxx xxxx XXX xxxxx.

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

### $Xxxxxxxx
$$Xxxx$$

```yaml
Type: Nullable [Microsoft.WindowsAzure.Storage.SharedAccessProtocol]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxXxxxxxxxxXxx
Xxxxxxxxx xxx xxxxxxxxx xxx xx xxx xxxxx xx xxx xxxxx xxx xxx xxxxx xxxx xxxx xxxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: startpk

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxXxxXxx
Xxxxxxxxx xxx xxx xxx xxx xxx xxxxx xx xxx xxxxx xxx xxx xxxxx xxxx xxxx xxxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: startrk

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxXxxx
Xxxxxxxxx xxxx xxx XXX xxxxx xxxxxxx xxxxx.

```yaml
Type: DateTime]
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

[Xxx$XxxxxXxxxxxxXxxxxxx](671aeec8-b7f9-49c5-866f-da84f189ab5b)


