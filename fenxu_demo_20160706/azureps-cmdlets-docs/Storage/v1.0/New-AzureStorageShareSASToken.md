---
external help file: RMAzure_Storage.xml
online version: 10a13c83-d545-4729-99f9-048c774f32d7
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# New-AzureStorageShareSASToken
## XXXXXXXX
Xxxxxxxx Xxxxxx Xxxxxx Xxxxxxxxx xxxxx xxx xxxxx$0 Xxxxxxx xxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
New-AzureStorageShareSASToken [-ShareName] <String> [-Context <AzureStorageContext>] [-ExpiryTime <DateTime]>]
 [-FullUri] [-IPAddressOrRange <String>]
 [-Protocol <Nullable [Microsoft.WindowsAzure.Storage.SharedAccessProtocol]>] [-StartTime <DateTime]>]
 -Policy <String>
```

### UNNAMED_PARAMETER_SET_2
```
New-AzureStorageShareSASToken [-ShareName] <String> [-Context <AzureStorageContext>] [-ExpiryTime <DateTime]>]
 [-FullUri] [-IPAddressOrRange <String>] [-Permission <String>]
 [-Protocol <Nullable [Microsoft.WindowsAzure.Storage.SharedAccessProtocol]>] [-StartTime <DateTime]>]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxxxXXXXxxxx$$ xxxxxx xxxxxxxxx x xxxxxx xxxxxx xxxxxxxxx xxxxx xxx xx xxxxx$0 Xxxxxxx xxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxxxx x xxxxxx xxxxxx xxxxxxxxx xxxxx xxx x xxxxx
```
PS C:\>New-AzureStorageShareSASToken -ShareName "ContosoShare" -Permission "rwdl"
```

Xxxx xxxxxxx xxxxxxx x xxxxxx xxxxxx xxxxxxxxx xxxxx xxx xxx xxxxx xxxxx XxxxxxxXxxxx.

### Xxxxxxx 0$ Xxxxxxxx xxxxxxxx xxxxxx xxxxxx xxxxxxxxx xxxxx xx xxxxx xxx xxxxxxxx
```
PS C:\>Get-AzureStorageShare -Prefix "test" | New-AzureStorageShareSASToken -Permission "rwdl"
```

Xxxx xxxxxxx xxxx xxx xxx Xxxxxxx xxxxxx xxxx xxxxx xxx xxxxxx xxxx.
Xxx xxxxxxx xxxxxx xxxx xx xxx xxxxxxx xxxxxx xx xxxxx xxx xxxxxxxx xxxxxxxx.
Xxx xxxxxxx xxxxxx xxxxxxx x xxxxxx xxxxxx xxxxx xxx xxxx Xxxxxxx xxxxx xxxx xxx xxx xxxxxxxxx xxxxxxxxxxx.

### Xxxxxxx 0$ Xxxxxxxx x xxxxxx xxxxxx xxxxxxxxx xxxxx xxxx xxxx x xxxxxx xxxxxx xxxxxx
```
PS C:\>New-AzureStorageShareSASToken -ShareName "ContosoShare" -Policy "ContosoPolicy03"
```

Xxxx xxxxxxx xxxxxxx x xxxxxx xxxxxx xxxxxxxxx xxxxx xxx xxx Xxxxxxx xxxxx xxxxx XxxxxxxXxxxx xxxx xxx xxx xxxxxx xxxxx XxxxxxxXxxxxx00.

## XXXXXXXXXX

### -Context
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

### -ExpiryTime
Xxxxxxxxx xxx xxxx xx xxxxx xxx xxxxxx xxxxxx xxxxxxxxx xxxxxxx xxxxxxx.

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

### -FullUri
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxx xxx xxxx xxxx XXX xxx xxx xxxxxx xxxxxx xxxxxxxxx xxxxx.

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

### -IPAddressOrRange
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

### -Permission
Xxxxxxxxx xxx xxxxxxxxxxx xx xxx xxxxx xx xxxxxx xxx xxxxx xxx xxxxx xxxxx xxx xxxxx.

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

### -Policy
Xxxxxxxxx xxx xxxxxx xxxxxx xxxxxx xxx x xxxxx.

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

### -Protocol
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

### -ShareName
Xxxxxxxxx xxx xxxx xx xxx Xxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: N,Name

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByValue,ByPropertyName)
Accept wildcard characters: False
```

### -StartTime
Xxxxxxxxx xxx xxxx xx xxxxx xxx xxxxxx xxxxxx xxxxxxxxx xxxxxxx xxxxx.

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
Xxxxxxxx$ xxxxxx$ xxxxx$ xxxxxxxx$ xxxx$ xxxxxxx$ xxxx$ xxxxx$ xxxxx

## XXXXXXX XXXXX

[Get-AzureStorageShare](10a13c83-d545-4729-99f9-048c774f32d7)

[New-AzureStorageFileSASToken](4fb064f5-94bc-4d8f-9ef6-2611f8aab99c)


