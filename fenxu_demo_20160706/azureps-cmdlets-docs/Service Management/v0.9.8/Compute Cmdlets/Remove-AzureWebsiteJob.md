---
external help file: SMAzure_Compute.xml
online version: 3997c3b8-37ce-4135-a17d-63ae3bdd8e74
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Remove-AzureWebsiteJob
## XXXXXXXX
Xxxxxxx xx xxxxxxxx xxx xxx xxx x xxxxxxx

## XXXXXX

```
Remove-AzureWebsiteJob [[-Name] <String>] [-Force] [-Slot <String>] -JobName <String> [-JobType]
```

## XXXXXXXXXXX
Xxxxxxx xx xxxxxxxx xxx xxx xxx x xxxxxxx

## XXXXXXXX

### $$$$$$$$$$$$$$  Xxxxxx xx xxxxxxxx xxx xxx xxx x xxxxxxx $$$$$$$$$$$$$$
```
C:\PS>Remove-AzureWebsiteJob -Name MyWebsite -JobName MyWebJob -JobType Continuous
```

Xxxxxxx x xxx xxx xxxxxx XxXxxXxx xxx XxXxxXxxx

## XXXXXXXXXX

### -Force
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxxx xxx xxx xxx xxxxxxx xxxxxxxxx xxx xxx xxxxxxxxxxxx.

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

### -JobType
Xxx xxx xxx xxxx.
Xxx xx $xxxxxxxxx$ xx $xxxxxxxxxx$

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Accepted values: Triggered, Continuous

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
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

[Remove-AzureWebsite](3997c3b8-37ce-4135-a17d-63ae3bdd8e74)

[Get-AzureWebsiteJob](5ef76b84-385f-419e-8aba-228d53ce2232)

[New-AzureWebsiteJob](89c77daa-24fd-4b27-b624-3486fe642722)

[Start-AzureWebsiteJob](33bc54a9-76a7-45cd-92d5-662e16354fa3)

[Stop-AzureWebsiteJob](9698753f-0bfc-4845-b74e-6c6bed38a430)


