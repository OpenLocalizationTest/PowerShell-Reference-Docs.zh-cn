---
external help file: RMAzure_Storage.xml
online version: 671aeec8-b7f9-49c5-866f-da84f189ab5b
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXxxxxxxXxxxXXXXxxxx
## XXXXXXXX
Xxxxxxxxx x xxxxxx xxxxxx xxxxxxxxx xxxxx xxx x Xxxxxxx xxxx.

## XXXXXX

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureStorageFileSASToken [-ShareName] <String> [-Path] <String> [-Context <AzureStorageContext>]
 [-ExpiryTime <DateTime]>] [-FullUri] [-IPAddressOrRange <String>] [-Permission <String>]
 [-Protocol <Nullable [Microsoft.WindowsAzure.Storage.SharedAccessProtocol]>] [-StartTime <DateTime]>]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureStorageFileSASToken [-ShareName] <String> [-Path] <String> [-Context <AzureStorageContext>]
 [-ExpiryTime <DateTime]>] [-FullUri] [-IPAddressOrRange <String>]
 [-Protocol <Nullable [Microsoft.WindowsAzure.Storage.SharedAccessProtocol]>] [-StartTime <DateTime]>]
 -Policy <String>
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureStorageFileSASToken [-ExpiryTime <DateTime]>] [-FullUri] [-IPAddressOrRange <String>]
 [-Permission <String>] [-Protocol <Nullable [Microsoft.WindowsAzure.Storage.SharedAccessProtocol]>]
 [-StartTime <DateTime]>] -File <CloudFile>
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureStorageFileSASToken [-ExpiryTime <DateTime]>] [-FullUri] [-IPAddressOrRange <String>]
 [-Protocol <Nullable [Microsoft.WindowsAzure.Storage.SharedAccessProtocol]>] [-StartTime <DateTime]>]
 -File <CloudFile> -Policy <String>
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxxXXXXxxxx$$ xxxxxx xxxxxxxxx x xxxxxx xxxxxx xxxxxxxxx xxxxx xxx xx xxxxx$0 Xxxxxxx xxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxxxx x xxxxxx xxxxxx xxxxxxxxx xxxxx xxxx xxx xxxx xxxx xxxxxxxxxxx
```
PS C:\> New-AzureStorageFileSASToken -ShareName "ContosoShare" -Path "FilePath" -Permission "rwd"
```

Xxxx xxxxxxx xxxxxxxxx x xxxxxx xxxxxx xxxxxxxxx xxxxx xxxx xxx xxxx xxxxxxxxxxx xxx xxx xxxx xxxx xx xxxxx XxxxXxxx.

### Xxxxxxx 0$ Xxxxxxxx x xxxxxx xxxxxx xxxxxxxxx xxxxx xxxx xxx x xxxx xxxxx
```
PS C:\> $StartTime = Get-Date
PS C:\> $EndTime = $StartTime.AddHours(2.0)
PS C:\> New-AzureStorageFileSASToken -ShareName "ContosoShare" -Path "FilePath" -Permission "rwd" -StartTime $StartTime -ExpiryTime $EndTime
```

Xxx xxxxx xxxxxxx xxxxxxx x $$XxxxXxxx$$ xxxxxx xx xxxxx xxx Xxx$Xxxx xxxxxx.
Xxx xxxxxxx xxxxxx xxx xxxxxxx xxxx xx xxx $XxxxxXxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx xxxxx xx xxx xxxxxx xx $XxxxxXxxx$ xxx xxxx xxxxxx xxx xxxxxx xx xxx $XxxXxxx xxxxxxxx.
Xxxx xxxxxx xx x xxxx xxx xxxxx xx xxx xxxxxx.

Xxx xxxxx xxxxxxx xxxxxxxxx x xxxxxx xxxxxx xxxxxxxxx xxxxx xxxx xxx xxx xxxxxxxxx xxxxxxxxxxx.
Xxxx xxxxx xxxxxxx xxxxx xx xxx xxxxxxx xxxx.
Xxx xxxxx xxxxxxx xxxxx xxxxx xxxx xxxxxx xx $XxxXxxx.

## XXXXXXXXXX

### $Xxxxxxx
Xxxxxxxxx xx xxxxx$0 Xxxxxxx xxxxxxx.
Xx xxxxxx x xxxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxxxxx xxxxxx.

```yaml
Type: AzureStorageContext
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

```yaml
Type: AzureStorageContext
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### $XxxxxxXxxx
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

### $Xxxx
Xxxxxxxxx x $$XxxxxXxxx$$ xxxxxx.
Xxx xxx xxxxxx x xxxxx xxxx xx xxxxxx xxx xx xxxxx xxx Xxx$XxxxxXxxxxxxXxxx xxxxxx.

```yaml
Type: CloudFile
Parameter Sets: UNNAMED_PARAMETER_SET_3, UNNAMED_PARAMETER_SET_4
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByValue,ByPropertyName)
Accept wildcard characters: False
```

### $XxxxXxx
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
Xxxxxxxxx xxx xxxx xx xxx xxxx xxxxxxxx xx x Xxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByValue, ByPropertyName)
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByValue, ByPropertyName)
Accept wildcard characters: False
```

### $Xxxxxxxxxx
Xxxxxxxxx xxx xxxxxxxxxxx xxx x Xxxxxxx xxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_3
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxx
Xxxxxxxxx xxx xxxxxx xxxxxx xxxxxx xxx x xxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_4
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

### $XxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxx Xxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue, ByPropertyName)
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue, ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxXxxx
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

[Xxx$XxxxxXxxxxxxXxxxxxx](671aeec8-b7f9-49c5-866f-da84f189ab5b)

[Xxx$XxxxxXxxxxxxXxxxxXXXXxxxx](07c8ad4e-7a32-4407-9120-1432126b7376)


