---
external help file: RMAzure_Storage.xml
online version: f08d2de2-a276-439c-b9a8-ee187a8c334e
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# New-AzureStorageContainerSASToken
## XXXXXXXX
Xxxxxxxxx xx XXX xxxxx xxx xx xxxxx$0 xxxxxxx xxxxxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
New-AzureStorageContainerSASToken [-Name] <String> [-Context <AzureStorageContext>] [-ExpiryTime <DateTime]>]
 [-FullUri] [-IPAddressOrRange <String>]
 [-Protocol <Nullable [Microsoft.WindowsAzure.Storage.SharedAccessProtocol]>] [-StartTime <DateTime]>]
 -Policy <String>
```

### UNNAMED_PARAMETER_SET_2
```
New-AzureStorageContainerSASToken [-Name] <String> [-Context <AzureStorageContext>] [-ExpiryTime <DateTime]>]
 [-FullUri] [-IPAddressOrRange <String>] [-Permission <String>]
 [-Protocol <Nullable [Microsoft.WindowsAzure.Storage.SharedAccessProtocol]>] [-StartTime <DateTime]>]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxxxxxxxXXXXxxxx$$ xxxxxx xxxxxxxxx x Xxxxxx Xxxxxx Xxxxxxxxx $XXX$ xxxxx xxx xx xxxxx$0 xxxxxxx xxxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxxxx x xxxxxxxxx XXX xxxxx xxxx xxxx xxxxxxxxx xxxxxxxxxx
```
PS C:\>New-AzureStorageContainerSASToken -Name "Test" -Permission rwdl
```

Xxxx xxxxxxx xxxxxxxxx x xxxxxxxxx XXX xxxxx xxxx xxxx xxxxxxxxx xxxxxxxxxx.

### Xxxxxxx 0$ Xxxxxxxx xxxxxxxx xxxxxxxxx XXX xxxxx xx xxxxxxxx
```
PS C:\>Get-AzureStorageContainer -Container test* | New-AzureStorageContainerSASToken -Permission rwdl
```

Xxxx xxxxxxx xxxxxxxxx xxxxxxxx xxxxxxxxx XXX xxxxxx xx xxxxx xxx xxxxxxxx.

### Xxxxxxx 0$ Xxxxxxxx xxxxxxxxx XXX xxxxx xxxx xxxxxx xxxxxx xxxxxx
```
PS C:\>New-AzureStorageContainerSASToken -Name "Test" -Policy "PolicyName"
```

Xxxx xxxxxxx xxxxxxxxx x xxxxxxxxx XXX xxxxx xxxx xxxxxx xxxxxx xxxxxx.

## XXXXXXXXXX

### -Context
Xxxxxxxxx xx xxxxx$0 xxxxxxx xxxxxxx.
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

### -ExpiryTime
Xxxxxxxxx xxx xxxx xx xxxxx xxx xxxxxx xxxxxx xxxxxxxxx xxxxxxx xxxxxxx.

Xx xxx xxxx xxxx xxx xxxxx xxxx xxx xxx xxx xxxxxx xxxx$ xxx xxxxxx xxxx xx xxx xx xxx xxxxx xxxx xxxx xxx xxxx.
Xx xxxxxxx xxx xxxxx xxxx xxx xxx xxxxxx xxxx xx xxxxxxxxx$ xxx xxxxxx xxxx xx xxx xx xxx xxxxxxx xxxx xxxx xxx xxxx.

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

### -Name
Xxxxxxxxx xx xxxxx$0 xxxxxxx xxxxxxxxx xxxx.

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

### -Permission
Xxxxxxxxx xxxxxxxxxxx xxx x xxxxxxx xxxxxxxxx.

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
Xxxxxxxxx xx xxxxx$0 Xxxxxx Xxxxxx Xxxxxx.

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

## XXXXXXX XXXXX

[New-AzureStorageBlobSASToken](f08d2de2-a276-439c-b9a8-ee187a8c334e)


