---
external help file: RMAzure_Apimanagement.xml
online version: 6df0b014-03b0-47aa-9d34-9d0fceee2247
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXxXxxXxxxxxxxxxXxxxxx
## XXXXXXXX
Xxxx xxx xxxxxxxxxx xxxxxxx xx x XxXxxXxxxxxxxxx xxxxxxxx.

## XXXXXX

```
Add-AzureRmApiManagementRegion [-Capacity <Int32]>] [-Sku <PsApiManagementSku]>]
 [-VirtualNetwork <PsApiManagementVirtualNetwork>] -ApiManagement <PsApiManagement> -Location <String>
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxXxxXxxxxxxxxxXxxxxx$$ xxxxxx xxxx xxx xxxxxxxx xx xxxx $$XxXxxXxxxxxxxxxXxxxxx$$ xx xxx xxxxxxxxxx xx $$XxxxxxxxxxXxxxxxx$$ xx xxxxxxxx xxxxxxxx xx xxxx $$Xxxxxxxxx.Xxxxx.Xxxxxxxx.XxxXxxxxxxxxx.Xxxxxx.XxXxxXxxxxxxxxx$$.
Xxxx xxxxxx xxxx xxx xxxxxx xxxxxxxx xx xxxxxx xxx xxxxxxx xxxxxxxx xx $$XxXxxXxxxxxxxxx$$ xx$xxxxxx.
Xx xxxxxx x xxxxxxxxxx xx xx XXX Xxxxxxxxxx xxxx xxx xxxxxxxx $$XxXxxXxxxxxxxxx$$ Xxxxxxxx xx Xxxxxx$XxxxxXxXxxXxxxxxxxxxXxxxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx xxx xxxxxxxxxx xxxxxxx xx x XxXxxXxxxxxxxxx xxxxxxxx
```
PS C:\>Add-AzureRmApiManagementRegion -ApiManagement $ApiManagement -Location "East US" -Sku "Premium" -Capacity 2
```

Xxxx xxxxxxx xxxx xxx xxxxxxx XXX xxxxx xxx xxx xxxxxx xxxxx Xxxx XX xx xxx $$XxXxxXxxxxxxxxx$$ xxxxxxxx.

### Xxxxxxx 0$ Xxx xxx xxxxxxxxxx xxxxxxx xx x XxXxxXxxxxxxxxx xxxxxxxx xxx xxxx xxxxxx xxxxxxxxxx
```
PS C:\>Get-AzureRmApiManagement -ResourceGroupName "Contoso" -Name "ContosoApi" | Add-AzureRmApiManagementRegion -Location "East US" -Sku "Premium" -Capacity 2 | Update-AzureRmApiManagementDeployments
```

Xxxx xxxxxxx xxxx x $$XxXxxXxxxxxxxxx$$ xxxxxx$ xxxx xxx xxxxxxx XXX xxxxx xxx xxx xxxxxx xxxxx Xxxx XX$ xxx xxxx xxxxxxx xxxxxxxxxx.

## XXXXXXXXXX

### $XxxXxxxxxxxxx
Xxxxxxxxx xxx $$XxXxxXxxxxxxxxx$$ xxxxxxxx xxxx xxxx xxxxxx xxxx xxxxxxxxxx xxxxxxxxxx xxxxxxx xx.

```yaml
Type: PsApiManagement
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByValue)
Accept wildcard characters: False
```

### $Xxxxxxxx
Xxxxxxxxx xxx XXX xxxxxxxx xx xxx xxxxxxxxxx xxxxxx.

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

### $Xxxxxxxx
Xxxxxxxxx xxx xxxxxxxx xx xxx xxx xxxxxxxxxx xxxxxx.

Xxxxx xxxxxx xxx$ 

$$ Xxxxx Xxxxxxx XX $$ Xxxxx Xxxxxxx XX $$ Xxxxxxx XX $$ Xxxx Xxxxxx $$ Xxxxx Xxxxxx $$ Xxxx XX $$ Xxxx XX $$ Xxxx XX 0 $$ Xxxxx Xxxx $$ Xxxxx Xxxx $$ Xxxxxx Xxxxx $$ Xxxxxxxxx Xxxx $$ Xxxx Xxxx $$ Xxxxxxxxx Xxxx $$ Xxxxxxxxx Xxxxxxxxx

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

### $Xxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxxxx xxxxxx.
Xxxxx xxxxxx xxx$ 

$$ Xxxxxxxxx $$ Xxxxxxxx $$ Xxxxxxx

```yaml
Type: PsApiManagementSku]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxXxxxxxx
Xxxxxxxxx x xxxxxxx xxxxxxx xxxxxxxxxxxxx.

```yaml
Type: PsApiManagementVirtualNetwork
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
Xxx xxxxxx xxxxxx xxxxxxx $$XxXxxXxxxxxxxxx$$ xxxxxxxx xx xxxxxxxx.

## XXXXXXX XXXXX

[Xxxxxx$XxxxxXxXxxXxxxxxxxxxXxxxxx](6df0b014-03b0-47aa-9d34-9d0fceee2247)

[Xxxxxx$XxxxxXxXxxXxxxxxxxxxXxxxxx](bf37a79f-38a4-433e-b847-beb564ad781c)

[Xxxxxx$XxxxxXxXxxXxxxxxxxxxXxxxxxxxxx](166e3bd3-929d-4213-aebc-411e2e8f50a2)


