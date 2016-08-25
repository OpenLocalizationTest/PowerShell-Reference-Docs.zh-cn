---
external help file: RMAzure_Apimanagement.xml
online version: 2a7ef835-586c-4e86-a243-3cc0e9623d71
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Set-AzureRmApiManagementHostnames
## XXXXXXXX
Xxxx x xxxxxx xxxxxxxx xxxxxxxxxxxxx xxx xx XXX Xxxxxxxxxx xxxxxxx xxxxx xx xxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Set-AzureRmApiManagementHostnames [-PassThru] -ApiManagement <PsApiManagement>
```

### UNNAMED_PARAMETER_SET_2
```
Set-AzureRmApiManagementHostnames [-PassThru]
 [-PortalHostnameConfiguration <PsApiManagementHostnameConfiguration>]
 [-ProxyHostnameConfiguration <PsApiManagementHostnameConfiguration>] -Name <String>
 -ResourceGroupName <String>
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxXxxXxxxxxxxxxXxxxxxxxx$$ xxxxxx xxxxxxx x xxxxxx xxxxxxxx xxxxxxxxxxxxx xxx xx XXX Xxxxxxxxxx xxxxxxx xxxxx xx xxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx xxx xxxxxx xxxxxxxx xxxxxxxxxxxxx xxx x xxxxx xxx xxxxxx
```
PS C:\>Set-AzureRmApiManagementHostnames -Name ContosoApi -ResourceGroupName Contoso -PortalHostnameConfiguration $portalHostnameConf -ProxyHostnameConfiguration $proxyHostnameConf
```

Xxxx xxxxxxx xxxx xxx xxxxxx xxxxxxxx xxxxxxxxxxxxx xxx xxxxx xxx xxxxxx.

### Xxxxxxx 0$ Xxxxxxxxx x xxxxxx xxxxxxxx xxx x xxxxx xxx xxxxxx
```
PS C:\>Import-AzureRmApiManagementHostnameCertificate -Name ContosoApi -ResourceGroupName "Contoso" -HostnameType "Proxy" -PfxPath "C:\proxycert.pfx" -PfxPassword "CertSecret"
PS C:\> Import-AzureRmApiManagementHostnameCertificate -Name "ContosoApi" -ResourceGroupName "Contoso" -HostnameType "Portal" -PfxPath "C:\portalcert.pfx" -PfxPassword "CertSecret"
PS C:\> $PortalHostnameConf = New-AzureRmApiManagementHostnameConfiguration -Hostname "portal.contoso.com" -CertificateThumbprint "33CC47C6FCA848DC9B14A6F071C1EF7C"
PS C:\> $ProxyHostnameConf = New-AzureRmApiManagementHostnameConfiguration -Hostname "proxy.contoso.com" -CertificateThumbprint "5DD7CCF6A1E74E0987DD2873406B7264"
PS C:\> Set-AzureRmApiManagementHostnames -Name "ContosoApi" -ResourceGroupName "Contoso" -PortalHostnameConfiguration $PortalHostnameConf -ProxyHostnameConfiguration $ProxyHostnameConf
```

Xxxx xxxxxxx xxxxxxxxxx x xxxxxx xxxxxxxx xxx xxxxx xxx xxxxxx.
Xxx xxxx xx xxxxxx xxxxxxxxxxxxx xxxxxxxxxxxx xxx xxxx xxxxx xxx xxxxxx xxxxxxxxx.

## XXXXXXXXXX

### -ApiManagement
Xxxxxxxxx xxx $$XxXxxXxxxxxxxxx$$ xxxxxxxx xxxx xxxx xxxxxx xxxx xxx $XxxxxxXxxxxxxxXxxxxxxxxxxxx$ xxx $XxxxxXxxxxxxxXxxxxxxxxxxxx$ xxxxxxxxxx xxxx.

```yaml
Type: PsApiManagement
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByValue)
Accept wildcard characters: False
```

### -Name
Xxxxxxxxx xxx xxxx xx xxx XXX Xxxxxxxxxx xxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
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

### -PortalHostnameConfiguration
Xxxxxxxxx xxx xxxxxx xxxxxx xxxxxxxx xxxxxxxxxxxxx.
Xxxxxxx $xxxx xx xxx xxxxxx xxxx xxx xxxxxxx xxxxxxxx.

```yaml
Type: PsApiManagementHostnameConfiguration
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ProxyHostnameConfiguration
Xxxxxxxxx xxx xxxxxx xxxxx xxxxxxxx xxxxxxxxxxxxx.
Xxxxxxx $xxxx xxxx xxx xxxxxxx xxxxxxxx.

```yaml
Type: PsApiManagementHostnameConfiguration
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxx xxxxx xxxxx xxxxx xxx XXX Xxxxxxxxxx xxxxxxxx xxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
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

[Import-AzureRmApiManagementHostnameCertificate](2a7ef835-586c-4e86-a243-3cc0e9623d71)

[New-AzureRmApiManagementHostnameConfiguration](73f73a6f-470c-4dd6-95c4-a1302fabb0dd)


