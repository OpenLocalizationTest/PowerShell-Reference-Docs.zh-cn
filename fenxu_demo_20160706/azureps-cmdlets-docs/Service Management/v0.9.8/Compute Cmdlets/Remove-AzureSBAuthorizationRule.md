---
external help file: SMAzure_Compute.xml
online version: 07ab8d50-c6de-45f1-8576-99b76f798bca
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Remove-AzureSBAuthorizationRule
## XXXXXXXX
Xxxxxxx xxxxxxxx Xxxxxxx Xxx xxxxxxxxxxxxx xxxx

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Remove-AzureSBAuthorizationRule [-Name] <String> [-Namespace] <String> [-EntityName] <String>
 [-EntityType] <ServiceBusEntityType> [-PassThru]
```

### UNNAMED_PARAMETER_SET_2
```
Remove-AzureSBAuthorizationRule [-Name] <String> [-Namespace] <String> [-PassThru]
```

## XXXXXXXXXXX
Xxxxxxx xxxxxxxx Xxxxxxx Xxx xxxxxxxxxxxxx xxxx

## XXXXXXXX

### $$$$$$$$$$$$$$ Xxxxxx xxxxxxxxxxxxx xxxx xx xxxxxxxxx xxxxx $$$$$$$$$$$$$$
```
C:\PS>Remove-AzureSBAuthorizationRule -Name MyRule -Namespace MyNamespace
```

Xxxxxxx xxxxxxxxxxxxx xxxx XxXxxx xxxx XxXxxxxxxxx

### $$$$$$$$$$$$$$ Xxxxxx xxxxxxxxxxxxx xxxx xxx x Xxxxx $$$$$$$$$$$$$$
```
C:\PS>Remove-AzureSBAuthorizationRule -Name MyRule -Namespace MyNamespace -EntityName MyEntity -EntityType Queue
```

Xxxxxxx xxxxxxxxxxxxx xxxx xxxxxx XxXxxx xxx x XxXxxxxx Xxxxx xx XxXxxxxxxxx

## XXXXXXXXXX

### -EntityName
Xxx xxxxxx xxxx xx xxxxx xxxx xx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: 3
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -EntityType
Xxx xxxxxx xxxx $Xxxxx$ Xxxxx$ Xxxxx$ XxxxxxxxxxxxXxx$.

```yaml
Type: ServiceBusEntityType
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: 4
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Xxx xxxxxx xxxxxxxxxxxxx xxxx xxxx

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Namespace
Xxx xxxxxxxxx xxxx xx xxxxx xxx xxxxxxxxxxxxx xxxx.
Xx xx XxxxxxXxxx xxxxxxxx xxx xxxx xxxx xx xx xxx xxxxxxxxx xxxxx

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PassThru
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxxx xx xxxxxx xxxxxxxxxxxx xxx xxxx xx xxxxx xx xxxxxxxx.
Xx xxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Get-AzureSBAuthorizationRule](07ab8d50-c6de-45f1-8576-99b76f798bca)

[New-AzureSBAuthorizationRule](3e60e1c8-7421-4762-befc-5c8974f684c4)

[Set-AzureSBAuthorizationRule](c199f0d5-8f84-4106-ac4b-afc2192d1218)


