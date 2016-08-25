---
external help file: RMAzure_Apimanagement.xml
online version: a6e4fc8a-f5c6-4f8e-8ed9-5ee80150b119
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Remove-AzureRmApiManagementRegion
## XXXXXXXX
Xxxxxxx xx xxxxxxxx xxxxxxxxxx xxxxxx xxxx XxXxxXxxxxxxxxx xxxxxxxx.

## XXXXXX

```
Remove-AzureRmApiManagementRegion -ApiManagement <PsApiManagement> -Location <String>
```

## XXXXXXXXXXX
Xxx $$Xxxxxx$XxxxxXxXxxXxxxxxxxxxXxxxxx$$ xxxxxx xxxxxxx xxxxxxxx xx xxxx $$Xxxxxxxxx.Xxxxx.Xxxxxxxx.XxxXxxxxxxxxx.Xxxxxx.XxXxxXxxxxxxxxxXxxxxx$$ xxxx x xxxxxxxxxx xx $$XxxxxxxxxxXxxxxxx$$ xx xxxxxxxx xxx xxxxxxxx xx xxxx $$Xxxxxxxxx.Xxxxx.Xxxxxxxx.XxxXxxxxxxxxx.Xxxxxx.XxXxxXxxxxxxxxx$$.
Xxxx xxxxxx xxxx xxx xxxxxx xxxxxxxxxx xx xxxxxx xxx xxxxxxx xxx xxxxxxxx xx $$XxXxxXxxxxxxxxx$$ xx$xxxxxx.
Xx xxxxxx x xxxxxxxxxx xx xx XXX Xxxxxxxxxx$ xxxx xxx xxxxxxxx $$XxXxxXxxxxxxxxxXxxxxxxx$$ xx $$Xxxxxx$XxxxxXxXxxXxxxxxxxxx$$.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxxxxx xxxx x XxXxxXxxxxxxxxx xxxxxxxx
```
PS C:\>Remove-AzureRmApiManagementRegion -ApiManagement $ApiManagement -Location "East US"
```

Xxxx xxxxxxx xxxxxxx xxx xxxxxx xxxxx Xxxx XX xxxx xxx $$XxXxxXxxxxxxxxx$$ xxxxxxxx.

### Xxxxxxx 0$ Xxxxxx x xxxxxx xxxx x XxXxxXxxxxxxxxx xxxxxxxx xxxxx x xxxxxx xx xxxxxxxx
```
PS C:\>Get-AzureRmApiManagement -ResourceGroupName "Contoso" -Name ContosoApi | Remove-AzureRmApiManagementRegion -Location "East US" | Update-AzureRmApiManagementDeployment
```

Xxxx xxxxx xxxxxxx xxxx xx xxxxxxxx xx $$XxXxxXxxxxxxxxx$$ xxxx xxx xxxxxxxx xxxxx xxxxx Xxxxxxx xxxxx XxxxxxxXxx.
Xxx xxxxx xxxxxxx xxxx xxxxxxx xxx xxxxxx xxxxx Xxxx XX xxxx xxxx xxxxxxxx xxxx xxxxxxx xxx xxxxxxxxxx.

## XXXXXXXXXX

### -ApiManagement
Xxxxxxxxx xxx $$XxXxxXxxxxxxxxx$$ xxxxxxxx xxxx xxxx xxxxxx xxxxxxx xxx xxxxxxxxxx xxxxxxxxxx xxxxxx xxxx.

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

### -Location
Xxxxxxxxx xxx xxxxxxxx xx xxx xxxxxx xxxx xxxx xxxxxx xxxxxxx.

Xxxxx xxxxxx xxx$ 

$$ Xxxxx Xxxxxxx XX $$ Xxxxx Xxxxxxx XX $$ Xxxxxxx XX $$ Xxxx Xxxxxx $$ Xxxxx Xxxxxx $$ Xxxx XX $$ Xxxx XX $$ Xxxx XX 0 $$ Xxxxx Xxxx $$ Xxxxx Xxxx $$ Xxxxxx Xxxxx $$ Xxxxxxxxx Xxxx $$ Xxxx Xxxx $$ Xxxxxxxxx Xxxx $$ Xxxxxxxxx Xxxxxxxxx

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

[Add-AzureRmApiManagementRegion](a6e4fc8a-f5c6-4f8e-8ed9-5ee80150b119)

[Update-AzureRmApiManagementRegion](bf37a79f-38a4-433e-b847-beb564ad781c)


