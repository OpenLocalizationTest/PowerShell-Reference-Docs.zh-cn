---
external help file: RMAzure_Storage.xml
online version: 74bc4494-be41-4493-9939-e51e61dd09e6
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# New-AzureStorageContext
## XXXXXXXX
Xxxxxxx xx xxxxx$0 Xxxxxxx xxxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
New-AzureStorageContext [-StorageAccountName] <String> [-Protocol] [-Anonymous] -Environment <String>
```

### UNNAMED_PARAMETER_SET_2
```
New-AzureStorageContext [-StorageAccountName] <String> [-Endpoint <String>] [-Protocol] [-Anonymous]
```

### UNNAMED_PARAMETER_SET_3
```
New-AzureStorageContext -ConnectionString <String>
```

### UNNAMED_PARAMETER_SET_4
```
New-AzureStorageContext [-StorageAccountName] <String> [-StorageAccountKey] <String> [-Endpoint <String>]
 [-Protocol]
```

### UNNAMED_PARAMETER_SET_5
```
New-AzureStorageContext [-StorageAccountName] <String> [-Endpoint <String>] [-Protocol] -SasToken <String>
```

### UNNAMED_PARAMETER_SET_6
```
New-AzureStorageContext [-StorageAccountName] <String> [-StorageAccountKey] <String> [-Protocol]
 -Environment <String>
```

### UNNAMED_PARAMETER_SET_7
```
New-AzureStorageContext [-StorageAccountName] <String> -Environment <String> -SasToken <String>
```

### UNNAMED_PARAMETER_SET_8
```
New-AzureStorageContext [-Local]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxxxxx$$ xxxxxx xxxxxxx xx xxxxx$0 Xxxxxxx xxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxxxxxx xx xxxxxxxxxx x xxxxxxx xxxxxxx xxxx xxx xxx
```
C:\PS>New-AzureStorageContext -StorageAccountName "ContosoGeneral" -StorageAccountKey "< Storage Key for ContosoGeneral ends with == >"
```

Xxxx xxxxxxx xxxxxxx x xxxxxxx xxx xxx xxxxxxx xxxxx XxxxxxxXxxxxxx xxxx xxxx xxx xxxxxxxxx xxx.

### Xxxxxxx 0$ Xxxxxx x xxxxxxx xx xxxxxxxxxx x xxxxxxxxxx xxxxxx
```
C:\PS>New-AzureStorageContext -ConnectionString "DefaultEndpointsProtocol=https;AccountName=ContosoGeneral;AccountKey=< Storage Key for ContosoGeneral ends with == >;"
```

Xxxx xxxxxxx xxxxxxx x xxxxxxx xxxxx xx xxx xxxxxxxxx xxxxxxxxxx xxxxxx xxx xxx xxxxxxx XxxxxxxXxxxxxx.

### Xxxxxxx 0$ Xxxxxx x xxxxxxx xxx xx xxxxxxxxx xxxxxxx xxxxxxx
```
C:\PS>New-AzureStorageContext -StorageAccountName "ContosoGeneral" -Anonymous -Protocol "http"
```

Xxxx xxxxxxx xxxxxxx x xxxxxxx xxx xxxxxxxxx xxx xxx xxx xxxxxxx xxxxx XxxxxxxXxxxxxx.
Xxx xxxxxxx xxxxxxxxx XXXX xx x xxxxxxxxxx xxxxxxxx.

### Xxxxxxx 0$ Xxxxxx x xxxxxxx xx xxxxx xxx xxxxx xxxxxxxxxxx xxxxxxx xxxxxxx
```
C:\PS>New-AzureStorageContext -Local
```

Xxxx xxxxxxx xxxxxxx x xxxxxxx xx xxxxx xxx xxxxx xxxxxxxxxxx xxxxxxx xxxxxxx.
Xxx xxxxxxx xxxxxxxxx xxx $Xxxxx$ xxxxxxxxx.

### Xxxxxxx 0$ Xxx xxx xxxxxxxxx xxx xxx xxxxx xxxxxxxxx xxxxxxx xxxxxxx
```
C:\PS>New-AzureStorageContext -Local | Get-AzureStorageContainer
```

Xxxx xxxxxxx xxxxxxx x xxxxxxx xx xxxxx xxx xxxxx xxxxxxxxxxx xxxxxxx xxxxxxx$ xxx xxxx xxxxxx xxx xxx xxxxxxx xx xxx $$Xxx$XxxxxXxxxxxxXxxxxxxxx$$ xxxxxx xx xxxxx xxx xxxxxxxx xxxxxxxx.
Xxx xxxxxxx xxxx xxx xxxxx$0 Xxxxxxx xxxxxxxxx xxx xxx xxxxx xxxxxxxxx xxxxxxx xxxxxxx.

### Xxxxxxx 0$ Xxx xxxxxxxx xxxxxxxxxx
```
C:\PS>$Context01 = New-AzureStorageContext -Local 
PS C:\> $Context02 = New-AzureStorageContext -StorageAccountName "ContosoGeneral" -StorageAccountKey "< Storage Key for ContosoGeneral ends with == >"
PS C:\> ($Context01, $Context02) | Get-AzureStorageContainer
```

Xxx xxxxx xxxxxxx xxxxxxx x xxxxxxx xx xxxxx xxx xxxxx xxxxxxxxxxx xxxxxxx xxxxxxx$ xxx xxxx xxxxxx xxxx xxxxxxx xx xxx $Xxxxxxx00 xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxxx x xxxxxxx xxx xxx xxxxxxx xxxxx XxxxxxxXxxxxxx xxxx xxxx xxx xxxxxxxxx xxx$ xxx xxxx xxxxxx xxxx xxxxxxx xx xxx $Xxxxxxx00 xxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx xxxxxxxxxx xxx xxx xxxxxxxx xxxxxx xx $Xxxxxxx00 xxx $Xxxxxxx00 xx xxxxx $$Xxx$XxxxxXxxxxxxXxxxxxxxx$$.

### Xxxxxxx 0$ Xxxxxx x xxxxxxx xxxx xx xxxxxxxx
```
C:\PS>New-AzureStorageContext -StorageAccountName "ContosoGeneral" -StorageAccountKey "< Storage Key for ContosoGeneral ends with == >" -Endpoint "contosoaccount.core.windows.net"
```

Xxxx xxxxxxx xxxxxxx xx xxxxx$0 Xxxxxxx xxxxxxx xxxx xxx xxx xxxxxxxxx xxxxxxx xxxxxxxx.
Xxx xxxxxxx xxxxxxx xxx xxxxxxx xxx xxx xxxxxxx xxxxx XxxxxxxXxxxxxx xxxx xxxx xxx xxxxxxxxx xxx.

### Xxxxxxx 0$ Xxxxxx x xxxxxxx xxxx x xxxxxxxxx xxxxxxxxxxx
```
C:\PS>New-AzureStorageContext -StorageAccountName "ContosoGeneral" -StorageAccountKey "< Storage Key for ContosoGeneral ends with == >" -Environment "AzureChinaCloud"
```

Xxxx xxxxxxx xxxxxxx xx xxxxx$0 xxxxxxx xxxxxxx xxxx xxx xxx xxxxxxxxx xxxxx$0 xxxxxxxxxxx.
Xxx xxxxxxx xxxxxxx xxx xxxxxxx xxx xxx xxxxxxx xxxxx XxxxxxxXxxxxxx xxxx xxxx xxx xxxxxxxxx xxx.

### Xxxxxxx 0$ Xxxxxx x xxxxxxx xx xxxxx xx XXX xxxxx
```
C:\PS>$SasToken = New-AzureStorageContainerSASToken -Name "ContosoMain" -Permission "raud"
PS C:\> $Context = New-AzureStorageContext -StorageAccountName "ContosoGeneral" -SasToken $SasToken
PS C:\> $Context | Get-AzureStorageBlob -Container "ContosoMain"
```

Xxx xxxxx xxxxxxx xxxxxxxxx xx XXX xxxxx xx xxxxx xxx $$Xxx$XxxxxXxxxxxxXxxxxxxxxXXXXxxxx$$ xxxxxx xxx xxx xxxxxxxxx xxxxx XxxxxxxXxxx$ xxx xxxx xxxxxx xxxx xxxxx xx xxx $XxxXxxxx xxxxxxxx.
Xxxx xxxxx xx xxx xxxx$ xxx$ xxxxxx$ xxx xxxxxx xxxxxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxxx x xxxxxxx xxx xxx xxxxxxx xxxxx XxxxxxxXxxxxxx xxxx xxxx xxx XXX xxxxx xxxxxx xx $XxxXxxxx$ xxx xxxx xxxxxx xxxx xxxxxxx xx xxx $Xxxxxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxxx xxx xxx xxxxx xxxxxxxxxx xxxx xxx xxxxxxxxx xxxxx XxxxxxxXxxx xx xxxxx xxx xxxxxxx xxxxxx xx $Xxxxxxx.

## XXXXXXXXXX

### -Anonymous
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxxx xx xxxxx$0 Xxxxxxx xxxxxxx xxx xxxxxxxxx xxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConnectionString
Xxxxxxxxx x xxxxxxxxxx xxxxxx xxx xxx xxxxx$0 Xxxxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Endpoint
Xxxxxxxxx xxx xxxxxxxx xxx xxx xxxxx$0 Xxxxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_4, UNNAMED_PARAMETER_SET_5
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Environment
Xxxxxxxxx xxx xxxxx$0 xxxxxxxxxxx.
xxxx$xxxxxxxxxxx XxxxxXxxxx xxx XxxxxXxxxxXxxxx.
Xxx xxxx xxxxxxxxxxx$ xxxx $$XXXX$Xxxxxxx$$Xxx$Xxxx Xxx$XxxxxXxxxxxxxxxx$$XXXX$Xxxxxxx$$.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_6
Aliases: Name,EnvironmentName

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_7
Aliases: Name,EnvironmentName

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Local
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxxx x xxxxxxx xx xxxxx xxx xxxxx xxxxxxxxxxx xxxxxxx xxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_8
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Protocol
Xxxxxxxxx xxx xxxxxxxx xxxxxxxxx xxx x xxxxxxx xxxx xxxx xxx xxxxxxx XXX.
xxxx$xxxxxxxxxxx

$$ XxxxxXxxx $$ XxxxxXxXxxx

Xxx xxxxxxx xxxxx xx XxxxxXxXxxx.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_4, UNNAMED_PARAMETER_SET_5, UNNAMED_PARAMETER_SET_6
Aliases: 
Accepted values: Http, Https

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SasToken
Xxxxxxxxx x Xxxxxx Xxxxxx Xxxxxxxxx $XXX$ xxxxx xxx xxx xxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_5, UNNAMED_PARAMETER_SET_7
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StorageAccountKey
Xxxxxxxxx xx xxxxx$0 Xxxxxxx xxxxxxx xxx.
Xxxx xxxxxx xxxxxxx x xxxxxxx xxx xxx xxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_4, UNNAMED_PARAMETER_SET_6
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StorageAccountName
Xxxxxxxxx xx xxxxx$0 Xxxxxxx xxxxxxx xxxx.
Xxxx xxxxxx xxxxxxx x xxxxxxx xxx xxx xxxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_4, UNNAMED_PARAMETER_SET_5, UNNAMED_PARAMETER_SET_6, UNNAMED_PARAMETER_SET_7
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

### AzureStorageContext

## XXXXX

## XXXXXXX XXXXX

[Get-AzureStorageBlob](74bc4494-be41-4493-9939-e51e61dd09e6)

[New-AzureStorageContainerSASToken](dc3564e2-9ede-4901-8d62-f49017a03281)


