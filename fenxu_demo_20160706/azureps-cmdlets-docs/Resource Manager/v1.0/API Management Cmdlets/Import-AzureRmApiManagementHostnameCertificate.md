---
external help file: RMAzure_Apimanagement.xml
online version: 73f73a6f-470c-4dd6-95c4-a1302fabb0dd
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Import-AzureRmApiManagementHostnameCertificate
## XXXXXXXX
Xxxxxxx x xxxxxxxxxxx xx x XXX xxxxxx xxx xx XXX Xxxxxxxxxx Xxxxxxx.

## XXXXXX

```
Import-AzureRmApiManagementHostnameCertificate [-PassThru] [-HostnameType] -Name <String> -PfxPassword <String>
 -PfxPath <String> -ResourceGroupName <String>
```

## XXXXXXXXXXX
Xxx $$Xxxxxx$XxxxxXxXxxXxxxxxxxxxXxxxxxxxXxxxxxxxxxx$$ xxxxxx xxxxxxx x xxxxxxxxxxx xx x XXX xxxxxx xxx xx XXX Xxxxxxxxxx Xxxxxxx.
Xxx xxxxxxxxxxx xx xx xx xxxx xxx xxxxxx xxxxxxxxx xxxxxxxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x XXX Xxxxxxxxxx xxxxxxxx xxxxxxxxxxx
```
PS C:\>Import-AzureRmApiManagementHostnameCertificate -Name "ContosoApi" -ResourceGroupName Contoso -HostnameType "Proxy" -PfxPath "C:\proxycert.pfx" -PfxPassword "CertSecret"
```

Xxxx xxxxxxx xxxxxxx x xxxxxxxxxxx xxx x xxxxx xxxxxx xxxxxxxx.

## XXXXXXXXXX

### -HostnameType
Xxxxxxxxx xxx xxxx xxxx xxxx xxxx xxxx xxxxxx xxxxx xxx xxxxxxxxxxx xxx.

Xxxxx xxxxxx xxx$ 

$$ Xxxxx $$ Xxxxxx

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Accepted values: Proxy, Portal

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Name
Xxxxxxxxx xxx xxxx xx xxx XXX Xxxxxxxxxx xxxxxxxxxx xxxx xxxx xxxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
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

### -PfxPassword
Xxxxxxxxx xxx xxxxxxxx xxx xxx .xxx xxxxxxxxxxx xxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PfxPath
Xxxxxxxxx xxx xxxx xx x .xxx xxxxxxxxxxx xxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
Xxxxxxxxx xxx xxxx xx xxx xx xxxxxxxx xxxxx xxxxx xxxxx xxx XXX Xxxxxxxxxx xxxxxxxxxx xxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[New-AzureRmApiManagementHostnameConfiguration](73f73a6f-470c-4dd6-95c4-a1302fabb0dd)

[Set-AzureRmApiManagementHostnames](dd997f04-b85b-409c-8c69-a5e659c768e3)


