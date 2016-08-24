---
external help file: SMAzure_Compute.xml
online version: 
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXxxxxxxXxxxxx
## XXXXXXXX
Xxxx xxxxxxx xxx xxx Xxxxx xxxxxxx xx xxx xxxxxxx xxxxxxxxxxxx.

## XXXXXX

```
Get-AzureWebsiteMetric [[-Name] <String>] [[-MetricNames] <String[]>] [[-StartDate] <DateTime>]
 [[-EndDate] <DateTime>] [[-TimeGrain] <String>] [-InstanceDetails] [-SlotView] [-Slot <String>]
```

## XXXXXXXXXXX
Xxxx xxxxx xxxxxxxxx xxx xxxxxx xx xxx 0.0.00 xxxxxxx xx xxx Xxxxxxxxx Xxxxx XxxxxXxxxx xxxxxx.
Xx xxx xxx xxxxxxx xx xxx xxxxxx xxx$xx xxxxx$ xx xxx Xxxxx XxxxxXxxxx xxxxxxx$ xxxx $Xxx$Xxxxxx $Xxxx Xxxxx$.Xxxxxxx.

Xxx Xxx$XxxxxXxxxxxxXxxxxx xxxxxx xxxx xxxxxxx xxx xxx Xxxxx xxxxxxx xx xxx xxxxxxx xxxxxxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx xxxxxxx xxx xxx xxxx xxxxx xxxxx xx x xxx$xxxxxxxx xxxxx xxx x xxxxxxx
```
PS C:\>Get-AzureWebsiteMetric -Name "ContosoWebSite" -StartDate (get-date).AddHours(-3) -MetricNames "Requests" -InstanceDetails -SlotView -TimeGrain "PT1M" 
$metrics[1].Data Name : Requests 

Unit : Count 

StartTime : 8/11/2014 7:05:00 AM 

EndTime : 8/11/2014 5:06:01 PM 

TimeGrain : PT1M 
PrimaryAggregationType : Instance 
Values : {Time:8/11/2014 7:05:00 AM, Total:4, Min:, Max:, Time:8/11/2014 7:06:00 AM, Total:3, Min:, Max:, 
Time:8/11/2014 7:07:00 AM, Total:3, Min:, Max:, Time:8/11/2014 7:08:00 AM, Total:12, Min:, Max:...} 
$metrics[1].Data.Values | ft 
TimeCreated Total Minimum Maximum Count InstanceName 
----------- ----- ------- ------- ----- ------------ 
8/11/2014 7:05:00 AM 4 1 RD00155DC24599 
8/11/2014 7:06:00 AM 3 1 RD00155DC24599 
8/11/2014 7:07:00 AM 3 1 RD00155DC24589 
8/11/2014 7:08:00 AM 12 1 RD00155DC24599
8/11/2014 7:09:00 AM 37 1 RD00155DC24599 
8/11/2014 7:10:00 AM 9 1 RD00155DC24599
```

Xxxx xxxxxxx xxxx xxxxxxx xxx xxx xxxx xxxxx xxxxx xx x xxx$xxxxxxxx xxxxx xxx x xxxxxxx.

## XXXXXXXXXX

### $XxxXxxx
Xxxxxxxxx xxx xxxx$ xx x XxxxXxxx xxxxxx$ xx xxxx xxxxxxx xxxxxxx.
Xx xxxxxx x XxxxXxxx xxxxxx$ xxx xxx Xxx$Xxxx xxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxxx Xxx$Xxxx Xxx$Xxxx.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases: 

Required: False
Position: 5
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxxxxXxxxxxx
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxxxx xxxxxxx xx x xxx$xxxxxxxx xxxxx.
Xx xxx xxx xxxxxxx xxxx xxxx xx xxx xx xxxx xxxxxxxxx$ xxxx xxxxxx xxxxxxx xxxxxxx xxx xxxx xxxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: 7
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxxXxxxx
Xxxxxxxxx xx xxxxx xx xxxxxxx xx xxx.
Xx xxx xx xxx xxxxxxx xxxx xxxxxxxxx$ xxx xxxxxx xxxx xxx xxxxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $Xxxx
Xxxxxxxxx xxx xxxx xx x xxxxxxx xx xxx xxxxxxxxxxxx.
Xxxx xxxxxxxxx xxxx xxx xxxxxxx xxxxxxxx xxxxxxxxxx.

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

### $Xxxx
Xxxxxxxxx xxx xxxxxxxxxxx xx x xxxxx xxxxxxx xxxxxxxxxx.
Xxxxx xxxxxx xxx$ Xxxxxxxxxx xxx Xxxxxxx.

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

### $XxxxXxxx
Xxxxxxxxx xxxx xxxx xxxxxx xxxx xxxxxxx xxx xxx xxxx xxxxx xxxx xxxxxxx xxxxxxx xx xxx xxxxxxx xxxx.
Xx x xxxx xxxxxx xxxxxx xxx xxxx xxxxxx$ xxx xxxxxxx xxx xxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: 8
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxXxxx
Xxxxxxxxx xxx xxxx$ xx x XxxxXxxx xxxxxx$ xx xxxxx xxxxxxx xxxxxxx.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases: 

Required: False
Position: 4
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxxXxxxx
Xxxxxxxxx xxx xxxx xxxx xxx xxxxxxx.
Xxxxx xxxxxx xxx$ 

$$ XX0X $Xxxxxx$ $$ XX0X $Xxxx$ $$ X0X $Xxx$

Xxx xxxxxxx xxxxx xx XX0X.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 6
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

### 
Xxx xxx xxxx xxxxx xx xxxx xxxxxx xx xxxxxxxx xxxx$ xxx xxx xx xxxxx.

## XXXXXXX

### Xxxxxxxxx.XxxxxxxXxxxx.Xxxxxxxx.Xxxxxxxxx.Xxxxxxxx.Xxxxxxxx.XxxXxxxxxxx.XxxxxxXxxxxxxx
Xx xxxxxxx$ Xxx$XxxxxXxxxxxxXxxxxx xxxxxxx xx xxxxx xx XxxxxxXxxxxxxx xxxxxxx.

## XXXXX

## XXXXXXX XXXXX

[Xxx$XxxxxXxxxxxx](0c2a5092-db45-4ce7-b39b-d1e499b4a867)


