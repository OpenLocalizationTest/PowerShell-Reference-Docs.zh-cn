---
external help file: SMAzure_Compute.xml
online version: 0c2a5092-db45-4ce7-b39b-d1e499b4a867
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Get-AzureWebsiteJob
## XXXXXXXX
Xxxx xxx xxx xxxx xxxxxxxxxx xxxx x xxxxxxx

## XXXXXX

```
Get-AzureWebsiteJob [[-Name] <String>] [-JobName <String>] [-JobType <String>] [-Slot <String>]
```

## XXXXXXXXXXX
Xxxx xxx xxx xxxx xxxxxxxxxx xxxx x xxxxxxx

## XXXXXXXX

### $$$$$$$$$$$$$$  Xxx xxxxxxxx xxx xxx xxxx $$$$$$$$$$$$$$
```
C:\PS>Get-AzureWebsiteJob -Name MyWebsite -JobName MyWebJob
```

Xxxx x xxx xxx xxxxxx XxXxxXxx xxxx XxXxxxxxx xxxxxxxxxx xxxx

### $$$$$$$$$$$$$$  Xxx xxx xxx xxxx xxx x xxxxxxx $$$$$$$$$$$$$$
```
C:\PS>Get-AzureWebsiteJob -Name MyWebsite
```

Xxxx xxx xxx xxxx xxxxxxxxxx xxxx XxXxxxxxx xxxxxxxxxx xxxx

### $$$$$$$$$$$$$$  Xxx xxx xxxxxxxxx xxx xxxx $$$$$$$$$$$$$$
```
C:\PS>Get-AzureWebsiteJob -Name MyWebsite -Slot staging -Type Triggered
```

Xxxx xxx xxxxxxxxx xxx xxxx xxxx xxxxxxx xxxx xx XxXxxxxxx

## XXXXXXXXXX

### -JobName
Xxx xxx xxx xxxx

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

### -JobType
Xxx xxx xxx xxxx.
Xxx xx $xxxxxxxxx$ xx $xxxxxxxxxx$

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

[Get-AzureWebsite](0c2a5092-db45-4ce7-b39b-d1e499b4a867)

[New-AzureWebsiteJob](89c77daa-24fd-4b27-b624-3486fe642722)

[Remove-AzureWebsiteJob](e25091a2-2472-4674-978c-ec1522631bc1)

[Start-AzureWebsiteJob](33bc54a9-76a7-45cd-92d5-662e16354fa3)

[Stop-AzureWebsiteJob](9698753f-0bfc-4845-b74e-6c6bed38a430)


