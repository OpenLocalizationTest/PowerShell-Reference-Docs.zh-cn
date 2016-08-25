---
external help file: SMAzure_Compute.xml
online version: 0c2a5092-db45-4ce7-b39b-d1e499b4a867
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Get-AzureWebsiteJobHistory
## XXXXXXXX
Xxxx x xxx xxx xxxxxxx

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Get-AzureWebsiteJobHistory [[-Name] <String>] [-Slot <String>] -JobName <String> [-Latest]
```

### UNNAMED_PARAMETER_SET_2
```
Get-AzureWebsiteJobHistory [[-Name] <String>] [-Slot <String>] -JobName <String>
```

### UNNAMED_PARAMETER_SET_3
```
Get-AzureWebsiteJobHistory [[-Name] <String>] [-Slot <String>] -JobName <String> -RunId <String>
```

## XXXXXXXXXXX
Xxxx x xxx xxx xxxxxxx

## XXXXXXXX

### $$$$$$$$$$$$$$  Xxx xxxxxxxx xxxxxxx xxx x xxx xxx $$$$$$$$$$$$$$
```
C:\PS>Get-AzureWebsiteJobHistory -Name MyWebsite -JobName MyWebJob
```

Xxxx xxxxxxxx xxxxxxx xxx XxXxxXxx

### $$$$$$$$$$$$$$  Xxx xxxxxx xxx xxx x xxx xxx $$$$$$$$$$$$$$
```
C:\PS>Get-AzureWebsiteJobHistory -Name MyWebsite -JobName MyWebJob -Latest
```

Xxxx xxxxxx xxx xxxx xxx XxXxxXxx

### $$$$$$$$$$$$$$  Xxx xxxxxxxx xxx xxx x xxx xxx $$$$$$$$$$$$$$
```
C:\PS>Get-AzureWebsiteJobHistory -Name MyWebsite -JobName MyWebJob -RunId 10
```

Xxxx xxx xxxx xxxxx xxx xxxx xx 00 xxx XxXxxXxx

## XXXXXXXXXX

### -JobName
Xxx xxx xxx xxxx

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Latest
Xx xxxxxxxxx$ xxxxxx xxx xxxxxx xxx xxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Xxx xxxx xx xxx Xxxxx xxxxxxx

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

### -RunId
Xxx xx xx xxx xxx xxxxxxx xxx xxxx xx xxx

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Slot
Xxx xxxx xxxx xx xxx Xxxxx xxxxxxx

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Get-AzureWebsite](0c2a5092-db45-4ce7-b39b-d1e499b4a867)

[New-AzureWebsite](498c1abd-298b-43e9-ac53-bc57054a5387)

[Get-AzureWebsiteJob](5ef76b84-385f-419e-8aba-228d53ce2232)

[New-AzureWebsiteJob](89c77daa-24fd-4b27-b624-3486fe642722)

[Remove-AzureWebsiteJob](e25091a2-2472-4674-978c-ec1522631bc1)


