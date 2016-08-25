---
external help file: SMAzure_Compute.xml
online version: aaed4c39-d209-4663-b058-b480553ee6a9
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Get-AzureSchedulerJobHistory
## XXXXXXXX
Xxxx xxxxxxx xxx x xxxxxxxxx xxx.

## XXXXXX

```
Get-AzureSchedulerJobHistory [-Location] <String> [-JobCollectionName] <String> [-JobName] <String>
 [[-JobStatus] <String>] [-First] [-Skip] [-IncludeTotalCount]
```

## XXXXXXXXXXX
Xxxx xxxxx xxxxxxxxx xxx xxxxxx xx xxx 0.0.00 xxxxxxx xx xxx Xxxxxxxxx Xxxxx XxxxxXxxxx xxxxxx.
Xx xxx xxx xxxxxxx xx xxx xxxxxx xxx$xx xxxxx$ xx xxx Xxxxx XxxxxXxxxx xxxxxxx$ xxxx $Xxx$Xxxxxx $Xxxx Xxxxx$.Xxxxxxx.

Xxx Xxx$XxxxxXxxxxxxxxXxxXxxxxxx xxxxxx xxxx xxx xxxxxxx xxx x xxxxxxxxx xxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx xxxxxxx xxx x xxx xx xxxxx xxx xxxx
```
PS C:\>Get-AzureSchedulerJobHistory -Location "North Central US" -JobCollectionName "JobCollection01" -JobName "Job01"
```

Xxxx xxxxxxx xxxx xxx xxxxxxx xx xxx xxx xxxxx Xxx00.
Xxxx xxx xxxxxxx xx xxx xxx xxxxxxxxxx xxxxx XxxXxxxxxxxxx00 xx xxx xxxxxxxxx xxxxxxxx.

### Xxxxxxx 0$ Xxx xxxxxxx xxx x xxxxxx xxx xx xxxxx xxx xxxx
```
PS C:\>Get-AzureSchedulerJobHistory -Location "North Central US" -JobCollectionName "JobCollection01" -JobName "Job12" -JobStatus "Failed"
```

Xxxx xxxxxxx xxxx xxx xxxxxxx xx xxx xxx xxxxx Xxx00 xxxx xxx x xxxxxx xx Xxxxxx.
Xxxx xxx xxxxxxx xx xxx xxx xxxxxxxxxx xxxxx XxxXxxxxxxxxx00 xx xxx xxxxxxxxx xxxxxxxx.

## XXXXXXXXXX

### -JobCollectionName
Xxxxxxxxx xxx xxxx xx x xxxxxxxxx xxx xxxxxxxxxx.
Xxxx xxxxxx xxxx xxx xxxxxxx xxx x xxx xxxx xxxxxxx xx xxx xxxxxxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

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

### -JobName
Xxxxxxxxx xxx xxxx xx x xxxxxxxxx xxx xxx xxxxx xx xxx xxx xxxxxxx.

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

### -JobStatus
Xxxxxxxxx xxx xxxxxx xx xxxxxxxxx xxx xxx xxxxx xx xxx xxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 4
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Location
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxx xxxx xxxxx xxx xxxxx xxxxxxx.
Xxxxx xxxxxx xxx$ 

$$ Xxxxxxxx Xxxx $$ Xxxxxxxx Xxxxxx $$ Xxxxxxxx XX $$ Xxxx Xxxx $$ Xxxx XX $$ Xxxxx Xxxxxxx XX $$ Xxxxx Xxxxxx $$ Xxxxx Xxxxxxx XX $$ Xxxxxxxxx Xxxx $$ Xxxx Xxxxxx $$ Xxxx XX

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

### -First
Xxxx xxxx xxx xxxxxxxxx xxxxxx xx xxxxxxx.
Xxxxx xxx xxxxxx xx xxxxxxx xx xxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Skip
Xxxxxxx xxx xxxxxxxxx xxxxxx xx xxxxxxx xxx xxxx xxxx xxx xxxxxxxxx xxxxxxx.
Xxxxx xxx xxxxxx xx xxxxxxx xx xxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IncludeTotalCount
Xxxxxxx xxx xxxxx xxxxxx xx xxxxxxx xx xxx xxxx xxx $xx xxxxxxx$ xxxxxxxx xx xxx xxxxxxxx xxxxxxx.
Xx xxx xxxxxx xxxxxx xxxxxxxxx xxx xxxxx xxxxx$ xx xxxxxxxx $Xxxxxxx xxxxx xxxxx.$ Xxx xxxxxxx xxx xx Xxxxxxxx xxxxxxxx xxxx xxxxxxxxx xxx xxxxxxxxxxx xx xxx xxxxx xxxxx xxxxx.
Xxx xxxxx xx Xxxxxxxx xxxxxx xxxx 0.0 xx 0.0 xxxxx 0.0 xxxxx xxxx xxx xxxxxx xxxxx xxx xxxxx xxx xxxxxxx$ 0.0 xxxxx xxxx xxx xxxxx xx xxxxx$ xxx x xxxxx xxxxxxx 0.0 xxx 0.0 xxxxxxxxx xx xxxxxxxxxxxx xxxxxxxx xxxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Get-AzureSchedulerJob](aaed4c39-d209-4663-b058-b480553ee6a9)

[Get-AzureSchedulerJobCollection](1f6e64a2-021e-4ad7-93a4-9e1138607f01)


