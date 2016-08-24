---
external help file: SMAzure_Compute.xml
online version: 
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXxxXxxxxxxXxxxXxxxxx
## XXXXXXXX
Xxxx xxxxxxx xxx Xxxxx xxxxxxx xxxxxxx xxxxx.

## XXXXXX

```
Get-AzureWebHostingPlanMetric [[-WebSpaceName] <String>] [[-Name] <String>] [[-MetricNames] <String[]>]
 [[-StartDate] <DateTime>] [[-EndDate] <DateTime>] [[-TimeGrain] <String>] [-InstanceDetails]
```

## XXXXXXXXXXX
Xxxx xxxxx xxxxxxxxx xxx xxxxxx xx xxx 0.0.00 xxxxxxx xx xxx Xxxxxxxxx Xxxxx XxxxxXxxxx xxxxxx.
Xx xxx xxx xxxxxxx xx xxx xxxxxx xxx$xx xxxxx$ xx xxx Xxxxx XxxxxXxxxx xxxxxxx$ xxxx $Xxx$Xxxxxx $Xxxx Xxxxx$.Xxxxxxx.

Xxx Xxx$XxxxxXxxXxxxxxxXxxxXxxxxx xxxxxx xxxx xxxxxxx xxx Xxxxx xxx xxxxxxx xxxxx xx x xxxxxxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx xxxxxxx xxx xxx xxxx xxxxx xxxxx xx x xxx$xxxxxxxx xxxxx
```
PS C:\>Get-AzureWebHostingPlanMetric -WebSpaceName "eastuswebspace" -StartDate (get-date).AddHours(-3) -InstanceDetails $Metrics[1].Data 
Name : CpuPercentage 
Unit : Percent 
StartTime : 8/11/2014 7:00:00 AM 
EndTime : 8/11/2014 5:00:23 PM 
TimeGrain : PT1H 
PrimaryAggregationType : Instance 
Values : {Time:8/11/2014 7:00:00 AM, Total:2, Min:9, Max:0, Time:8/11/2014 8:00:00 AM, Total:2, Min:9, Max:0, 
Time:8/11/2014 9:00:00 AM, Total:2, Min:9, Max:0, Time:8/11/2014 10:00:00 AM, Total:2, Min:8, Max:0...} $metrics[1].Data.Values | ft 
TimeCreated Total Minimum Maximum Count InstanceName
 ----------- ----- ------- ------- ----- ------------ 
8/11/2014 7:00:00 AM 2 9 0 1 RD00155DC24599 
8/11/2014 8:00:00 AM 2 9 0 1 RD00155DC24599 
8/11/2014 9:00:00 AM 2 9 0 1 RD00155DC24579 
8/11/2014 10:00:00 AM 2 8 0 1 RD00155DC24599 
8/11/2014 11:00:00 AM 2 9 0 1 RD00155DC24599 
8/11/2014 12:00:00 PM 2 6 0 1 RD00155DC24599 
8/11/2014 1:00:00 PM 2 15 0 1 RD00155DC24599 
8/11/2014 2:00:00 PM 3 21 0 1 RD00155DC24599 
8/11/2014 3:00:00 PM 2 13 0 1 RD00155DC24599 
8/11/2014 4:00:00 PM 2 14 0 1 RD00155DC24599
```

Xxxx xxxxxxx xxxx xxx xxxxxxx xxxx xxxxxxx xxx xxxx xxxxx xxxxx xx xxx$xxxxxxxx xxxxx.

## XXXXXXXXXX

### $XxxXxxx
Xxxxxxxxx xxx xxx xxxx$ xx x XxxxXxxx xxxxxx$ xxxx xxxxx xx xxxxxx xxxxxxx.
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
Xx xxx xxxxxxx xxxxxxx xxxx xxxx xx xxx xx xxxx xxxxxxxx$ xxxx xxxxxx xxxxxxx xxxxxxx xxxxxxx xxx xxxx xxxxxxx.

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
Xxxxxxx xx xxxxx xx xxxxxxx xx xxx.
Xx xxx xx xxx xxxxxxx x xxxxx xxx xxxx xxxxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxx.

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
Xxxxxxxxx xxx xxxx xx x xxxx xx xxx xxxxxxxxxxxx.
Xx xxxxxxx$ Xxx$XxxxxXxxXxxxxxxXxxxXxxxxx xxxx xxx xxxxxxxx xx xxx xxxxxxx xxxxxxxxxxxx.
Xxxx xxxxxxxxx xxxx xxx xxxxxxx xxxxxxxx xxxxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxXxxx
Xxxxxxxxx xxx xxxxx xxxx$ xx x XxxxXxxx xxxxxx$ xxx xxxxx xx xxx xxxxxxx.

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
Xxxxxxxxx xxx xxxx xxxx xxx xxxxx xx xxx xxxxxxx.
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

### $XxxXxxxxXxxx
Xxxxxxxxx xxx xxxx xx x xxxxxxxx xx xxx xxxxxxxxxxxx.
Xx xxxxxxx$ Xxx$XxxxxXxxXxxxxxxXxxxXxxxxx xxxx xxx xxxxx xx xxx xxxxxxx xxxxxxxxxxxx.
Xxxx xxxxxxxxx xxxx xxx xxxxxxx xxxxxxxx xxxxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: WebSpace

Required: False
Position: 1
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

### 
Xxx xxx xxxx xxxxx xx xxxx xxxxxx xx xxxxxxxx xxxx$ xxx xxx xx xxxxx.

## XXXXXXX

### 
Xxxxxxxxx.XxxxxxxXxxxx.Xxxxxxxx.Xxxxxxxxx.Xxxxxxxx.Xxxxxxxx.XxxXxxxxxxx.XxxxxxXxxxxxxx

Xx xxxxxxx$ Xxx$XxxxxXxxXxxxxxxXxxxXxxxxx xxxxxxx xx xxxxx xx XxxxxxXxxxxxxx xxxxxxx.

## XXXXX

## XXXXXXX XXXXX

[Xxx$XxxxxXxxXxxxxxxXxxx](8e660e09-5cdc-4324-b7da-608008b057ca)


