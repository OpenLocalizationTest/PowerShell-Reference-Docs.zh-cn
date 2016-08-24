---
external help file: RMAzure_Apimanagement.xml
online version: e067ded3-a2e3-4d53-8628-0ebbafa62721
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxxxxx$XxxxxXxXxxXxxxxxxxxxXxxxxxxxxx
## XXXXXXXX
Xxxxxxx xxxxxxxxxx xx xx XXX Xxxxxxxxxx Xxxxxxx.

## XXXXXX

### XXXXXXX$XXXXXXXXX$XXX$0
```
Update-AzureRmApiManagementDeployment
 [-AdditionalRegions <0, Culture=neutral, PublicKeyToken=31bf3856ad364e35]]>] [-PassThru]
 [-VirtualNetwork <PsApiManagementVirtualNetwork>] -Capacity <Int32> -Location <String> -Name <String>
 -ResourceGroupName <String> [-Sku]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Update-AzureRmApiManagementDeployment [-PassThru] -ApiManagement <PsApiManagement>
```

## XXXXXXXXXXX
Xxx $$Xxxxxx$XxxxxXxXxxXxxxxxxxxxXxxxxxxxxx$$ xxxxxx xxxxxxx xxxxxxx xxxxxxxxxxx xx xx XXX Xxxxxxxxxx xxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxxxxxxxxx xx xx XxxXxxxxxxxxx xxxxxxxx
```
PS C:\>Update-AzureRmApiManagementDeployment -ResourceGroupName "Contoso" -Name "ContosoApi" -Sku "Standard" -Capacity 3
```

Xxxx xxxxxxx xxxxxxx xxxxxxxxxx xx xx XXX Xxxxxxxxxx xxxxxxxx xx x xxxxx xxxx xxxxxxxx xxxxxxxx.

### Xxxxxxx 0$ Xxx xx XxxXxxxxxxxxx xxxxxxxx xxx xxxxxxx xx
```
PS C:\>$ApiManagement = Get-AzureRmApiManagement -ResourceGroupName "Contoso" -Name "ContosoApi"
PS C:\> $ApiManagement.Sku = "Premium"
PS C:\> $ApiManagement.Capacity = 5
PS C:\> $ApiManagement.AddRegion("Central US", "Premium", 3)
PS C:\> Update-AzureRmApiManagementDeployment -ApiManagement $ApiManagement
```

Xxxx xxxxxxx xxxx xx Xxx Xxxxxxxxxx xxxxxxxx$ xxxxxx xx xx xxxx xxxxxxx xxxxx xxx xxxx xxxx xx xxxxxxxxxx xxxxx xxxxx xx xxx xxxxxxx xxxxxx.

## XXXXXXXXXX

### $XxxxxxxxxxXxxxxxx
Xxxxxxxxx xxxxxxxxxx xxxxxxxxxx xxxxxxx xx xxxxx$0 XXX Xxxxxxxxxx.

```yaml
Type: 0, Culture=neutral, PublicKeyToken=31bf3856ad364e35]]
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $XxxXxxxxxxxxx
Xxxxxxxxx xxx $$XxXxxXxxxxxxxxx$$ xxxxxxxx xx xxx xxxxxxxxxx xxxxxxxxxxxxx xxxx.
Xxx xxxx xxxxxxxxx xx xxx xxxxxxxx xxxxxxx xxx xxx xxx xxxxxxxx xxxxxxx.

```yaml
Type: PsApiManagement
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByValue)
Accept wildcard characters: False
```

### $Xxxxxxxx
Xxxxxxxxx xxx XXX xxxxxxxx xx xxx xxxxxx xxxxx$0 XXX Xxxxxxxxxx xxxxxxxxxx xxxxxx.

```yaml
Type: Int32
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $Xxxxxxxx
Xxxxxxxxx xxx xxxxxxxx xx xxx xxxxxx XXX Xxxxxxxxxx xxxxxxxxxx xxxxxx.

Xxxxx xxxxxx xxx$ 

$$ Xxxxx Xxxxxxx XX $$ Xxxxx Xxxxxxx XX $$ Xxxxxxx XX $$ Xxxx Xxxxxx $$ Xxxxx Xxxxxx $$ Xxxx XX $$ Xxxx XX $$ Xxxx XX 0 $$ Xxxxx Xxxx $$ Xxxxx Xxxx $$ Xxxxxx Xxxxx $$ Xxxxxxxxx Xxxx $$ Xxxx Xxxx $$ Xxxxxxxxx Xxxx $$ Xxxxxxxxx Xxxxxxxxx

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $Xxxx
Xxxxxxxxx xxx xxxx xx XXX Xxxxxxxxxx xxxx xxxx xxxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $XxxxXxxx
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

### $XxxxxxxxXxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxxxxxxx xxxxx xxxxx xxxxx XXX Xxxxxxxxxx xxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $Xxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxx xxxxx$0 XXX Xxxxxxxxxx xxxxxxxxxx xxxxxx.

Xxxxx xxxxxx xxx$ 

$$ Xxxxxxxxx $$ Xxxxxxxx $$ Xxxxxxx

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 
Accepted values: Developer, Standard, Premium

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxxxXxxxxxx
Xxxxxxxxx xxx Xxxxxxx Xxxxxxx xxxxxxxxxxxxx xx xxx xxxxxx xxxxx$0 XXX Xxxxxxxxxx xxxxxxxxxx xxxxxx.

```yaml
Type: PsApiManagementVirtualNetwork
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Xxx$XxxxxXxXxxXxxxxxxxxx](e067ded3-a2e3-4d53-8628-0ebbafa62721)


