---
external help file: SMAzure_Compute.xml
online version: 07ab8d50-c6de-45f1-8576-99b76f798bca
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXXXxxxxxxxxxxxxXxxx
## XXXXXXXX
Xxxxxxx xxxxxxxx Xxxxxxx Xxx xxxxxxxxxxxxx xxxx

## XXXXXX

### XXXXXXX$XXXXXXXXX$XXX$0
```
Set-AzureSBAuthorizationRule [-Name] <String> [-Permission] [-Namespace] <String> [-EntityName] <String>
 [-EntityType] <ServiceBusEntityType> [[-PrimaryKey] <String>] [[-SecondaryKey] <String>]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Set-AzureSBAuthorizationRule [-Name] <String> [-Permission] [-Namespace] <String> [[-PrimaryKey] <String>]
 [[-SecondaryKey] <String>]
```

## XXXXXXXXXXX
Xxxxxxx xxxxxxxx Xxxxxxx Xxx xxxxxxxxxxxxx xxxx

## XXXXXXXX

### $$$$$$$$$$$$$$ Xxxxx xxxxxxx xxx xxx xxxxxxxxxxxxx xxxx xx xxxxxxxxx xxxxx $$$$$$$$$$$$$$
```
C:\PS>Set-AzureSBAuthorizationRule -Name MyRule -Namespace MyNamespace -Permission $("Send")
```

Xxx xxxxxxx xxx xx xxxxxxx

### $$$$$$$$$$$$$$ Xxxxxx xxxxxxxxxxxxx xxxx xxxxxxxxxx $$$$$$$$$$$$$$
```
C:\PS>Set-AzureSBAuthorizationRule -Name MyRule -Namespace MyNamespace -Permission $("Listen", "Send") -EntityName MyEntity -EntityType Queue
```

Xxxxxxx xxx xxxxxxxxxxx

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

Required: True
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

[Xxx$XxxxxXXXxxxxxxxxxxxxXxxx](3e60e1c8-7421-4762-befc-5c8974f684c4)

[Xxxxxx$XxxxxXXXxxxxxxxxxxxxXxxx](7d4951b1-15ff-4fa4-9122-36538eee9cbe)


