---
external help file: SMAzure_Compute.xml
online version: 07ab8d50-c6de-45f1-8576-99b76f798bca
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXXXxxxxxxxxxxxxXxxx
## XXXXXXXX
Xxxxxxx xxx Xxxxxxx Xxx xxxxxxxxxxxxx xxxx

## XXXXXX

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureSBAuthorizationRule [-Name] <String> [-Permission] [-Namespace] <String> [-EntityName] <String>
 [-EntityType] <ServiceBusEntityType> [[-PrimaryKey] <String>] [[-SecondaryKey] <String>]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureSBAuthorizationRule [-Name] <String> [-Permission] [-Namespace] <String> [[-PrimaryKey] <String>]
 [[-SecondaryKey] <String>]
```

## XXXXXXXXXXX
Xxxxxxx xxx Xxxxxxx Xxx xxxxxxxxxxxxx xxxx

## XXXXXXXX

### $$$$$$$$$$$$$$ Xxxxxxx xxx xxxxxxxxxxxxx xxxx xxxx xxxxxxxxx xxxxxxx xxx $$$$$$$$$$$$$$
```
C:\PS>New-AzureSBAuthorizationRule -Name MyRule -Namespace MyNamespace -Permission $("Send")
```

Xxxxxxx xxx xxxxxxxxxxxxx xxxx xx xxxxxxxxx xxxxx xxxx Xxxx xxxxxxxxxx

### $$$$$$$$$$$$$$ Xxxxxxx xxx xxxxxxxxxxxxx xxxx xxxxxxxxx xxxxxxx xxx $$$$$$$$$$$$$$
```
C:\PS>New-AzureSBAuthorizationRule -Name MyRule -Namespace MyNamespace -Permission $("Manage", "Listen", "Send") -EntityName MyEntity -EntityType Queue -PrimaryKey P+lL/Mnd2Z9sj5hwMrRyAxQDdX8RHfbdqU2eIAqs1rc=
```

Xxxxxxx xxx xxxxxxxxxxxxx xxxx xx XxXxxxxx Xxxxx xxxxx xxxx xxx xxxxxxxxxxx

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
Accept pipeline input: False
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
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxx
Xxx xxxxxx xxxxxxxxxxxxx xxxx xxxx

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: 
Accept pipeline input: False
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
Xxx xxxxxxxxxxxxx xxxxxxxxxxx $Xxxx$ Xxxxxx$ Xxxxxx$

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Accepted values: Manage, Send, Listen

Required: False
Position: 2
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxXxx
Xxx Xxxxxx Xxxxxx Xxxxxxxxx xxxxxxx xxx.
Xxxx xx xxxxxxxxx xx xxx xxxxxxxx

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 6
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxxXxx
Xxx Xxxxxx Xxxxxx Xxxxxxxxx xxxxxxxxx xxx

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 7
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Xxx$XxxxxXXXxxxxxxxxxxxxXxxx](07ab8d50-c6de-45f1-8576-99b76f798bca)

[Xxxxxx$XxxxxXXXxxxxxxxxxxxxXxxx](7d4951b1-15ff-4fa4-9122-36538eee9cbe)

[Xxx$XxxxxXXXxxxxxxxxxxxxXxxx](c199f0d5-8f84-4106-ac4b-afc2192d1218)


