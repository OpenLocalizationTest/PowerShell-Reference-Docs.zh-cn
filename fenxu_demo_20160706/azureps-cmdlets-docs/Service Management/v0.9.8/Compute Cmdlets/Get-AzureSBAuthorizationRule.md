---
external help file: SMAzure_Compute.xml
online version: 3e60e1c8-7421-4762-befc-5c8974f684c4
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXXXxxxxxxxxxxxxXxxx
## XXXXXXXX
Xxxx Xxxxxxx xxx xxxxxxxxxxxxx xxxxx

## XXXXXX

### XXXXXXX$XXXXXXXXX$XXX$0
```
Get-AzureSBAuthorizationRule [[-Name] <String>] [-Permission] [-Namespace] <String> [-EntityName] <String>
 [-EntityType] <ServiceBusEntityType>
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Get-AzureSBAuthorizationRule [[-Name] <String>] [-Permission] [-Namespace] <String>
```

## XXXXXXXXXXX
Xxxx Xxxxxxx xxx xxxxxxxxxxxxx xxxxx

## XXXXXXXX

### $$$$$$$$$$$$$$ Xxx xxxxxxxxxxxxx xxxx xx xxxxxxxxx xxxxx $$$$$$$$$$$$$$
```
C:\PS>Get-AzureSBAuthorizationRule -Namespace MyNamespace
```

Xxxx xxx xxxxxxxxx xxxxxxxxxxxxx xxxxx xx XxXxxxxxxxx

### $$$$$$$$$$$$$$ Xxx xxxxxxxxxxxxx xxxx xxx x Xxxxx $$$$$$$$$$$$$$
```
C:\PS>Get-AzureSBAuthorizationRule -Namespace MyNamespace -EntityName MyEntity -EntityType Queue
```

Xxxx xxx xxxxxxxxx xxxxxxxxxxxxx xxxxx x XxXxxxxx Xxxxx xx XxXxxxxxxxx

### $$$$$$$$$$$$$$ Xxx xxxxxxxxxxxxx xxxx xx xxxx $$$$$$$$$$$$$$
```
C:\PS>Get-AzureSBAuthorizationRule -Name MyRule -Namespace MyNamespace
```

Xxxx xx xxxxxxxxxxxxx xxxx xxxxxx XxXxxx xx XxXxxxxxxxx xxxxx

### $$$$$$$$$$$$$$ Xxx xxxxxxxxxxxxx xxxx xx xxxxxxxxxxx $$$$$$$$$$$$$$
```
C:\PS>Get-AzureSBAuthorizationRule -Namespace MyNamespace -Permission $("Send")
```

Xxxx xxx xxxxxxxxxxxxx xxxxx xxxx xxxx xxxx xxxxxxxxxx xx xxxxxxxxx xxxxx

## XXXXXXXXXX

### $XxxxxxXxxx
Xxx xxxxxx xxxx xx xxxxx xxxx xx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: 4
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxxXxxx
Xxx xxxxxx xxxx $Xxxxx$ Xxxxx$ Xxxxx$ XxxxxxxxxxxxXxx$.

```yaml
Type: ServiceBusEntityType
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: 5
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $Xxxx
Xxx xxxxxx xxxxxxxxxxxxx xxxx xxxx

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $Xxxxxxxxx
Xxx xxxxxxxxx xxxx xx xxxxx xxx xxxxxxxxxxxxx xxxx.
Xx xx XxxxxxXxxx xxxxxxxx xxx xxxx xxxx xx xx xxx xxxxxxxxx xxxxx

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $Xxxxxxxxxx
Xxx xxxxxxxxxxxxx xxxxxxxxxxx xx xxxxxx $Xxxx$ Xxxxxx$ Xxxxxx$.
Xxxx xxxx xxxxx xxxxx

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Accepted values: Manage, Send, Listen

Required: False
Position: 2
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Xxx$XxxxxXXXxxxxxxxxxxxxXxxx](3e60e1c8-7421-4762-befc-5c8974f684c4)

[Xxxxxx$XxxxxXXXxxxxxxxxxxxxXxxx](7d4951b1-15ff-4fa4-9122-36538eee9cbe)

[Xxx$XxxxxXXXxxxxxxxxxxxxXxxx](c199f0d5-8f84-4106-ac4b-afc2192d1218)


