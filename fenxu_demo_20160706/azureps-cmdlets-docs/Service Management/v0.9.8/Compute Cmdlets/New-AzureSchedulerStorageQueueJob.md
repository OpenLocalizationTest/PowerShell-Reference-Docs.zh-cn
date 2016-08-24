---
external help file: SMAzure_Compute.xml
online version: 29c40d46-86c3-4f67-94f7-484371fdfba5
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXxxxxxxxxXxxxxxxXxxxxXxx
## XXXXXXXX
Xxxxxxx x xxxxxxxxx xxx xxxx xxx x Xxxxxxx xxxxxx.

## XXXXXX

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureSchedulerStorageQueueJob [-EndTime <DateTime>] [-ErrorActionHeaders <Hashtable>]
 [-ErrorActionMethod <String>] [-ErrorActionQueueMessageBody <String>] [-ErrorActionRequestBody <String>]
 [-ErrorActionSASToken <String>] [-ErrorActionStorageAccount <String>] [-ErrorActionStorageQueue <String>]
 [-ErrorActionURI <Uri>] [-ExecutionCount <Int32>] [-Frequency <String>] [-Interval <Int32>]
 [-JobState <String>] [-StartTime <DateTime>] [-StorageQueueMessage <String>] -JobCollectionName <String>
 -JobName <String> -Location <String> -SASToken <String> -StorageQueueAccount <String>
 -StorageQueueName <String>
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureSchedulerStorageQueueJob [-EndTime <DateTime>] [-ErrorActionHeaders <Hashtable>]
 [-ExecutionCount <Int32>] [-Frequency <String>] [-Interval <Int32>] [-JobState <String>]
 [-StorageQueueMessage <String>]
```

## XXXXXXXXXXX
Xxxx xxxxx xxxxxxxxx xxx xxxxxx xx xxx 0.0.00 xxxxxxx xx xxx Xxxxxxxxx Xxxxx XxxxxXxxxx xxxxxx.
Xx xxx xxx xxxxxxx xx xxx xxxxxx xxx$xx xxxxx$ xx xxx Xxxxx XxxxxXxxxx xxxxxxx$ xxxx $Xxx$Xxxxxx $Xxxx Xxxxx$.Xxxxxxx.

Xxx Xxx$XxxxxXxxxxxxxxXxxxxxxXxxxxXxx xxxxxx xxxxxxx x xxxxxxxxx xxx xxxx xxx xx Xxxxx Xxxxxxx xxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x Xxxxxxx xxx xxxx xxxx xxxx
```
PS C:\>New-AzureSchedulerStorageQueueJob -JobCollectionName "JobCollection01" -JobName "Job01" -Location "North Central US" -StorageQueueAccount "ContosoStorageAccount" -StorageQueueName "ContosoStorageQueue" -SASToken "?sv=2012-02-12&si=samplePolicy%2F30%2F2014%206%3A37%3A36%20PM&sig=vLQEbSfZbTFh7q3YrzlxBeL%2BjiYKp0gE6lMJ0a5Nb4M%3D"
```

Xxxx xxxxxxx xxxxxxx x xxxxxxxxx Xxxxxxx xxx xx xxxx xx xxx xxxxxxxxxx xxxxx XxxXxxxxxxxxx00.
Xxx xxxxxxx xxxxxxxxx xxx Xxxxxxx xxxxxxx$ xxxxx xxxx$ xxx XXX xxxxx.
Xxx xxx xxxx xxxx$ xxxxxxxxxxx.

### Xxxxxxx 0$ Xxxxxx x Xxxxxxx xxx xxxx xxxx x xxxxxxxxx xxxxxx xx xxxxx
```
PS C:\>New-AzureSchedulerStorageQueueJob -JobCollectionName "JobCollection01" -JobName "Job12" -Location "North Central US"-StorageQueueAccount "ContosoStorageAccount" -StorageQueueName "ContosoStorageQueue" -SASToken "?sv=2012-02-12&si=samplePolicy%2F30%2F2014%206%3A37%3A36%20PM&sig=vLQEbSfZbTFh7q3YrzlxBeL%2BjiYKp0gE6lMJ0a5Nb4M%3D" -ExecutionCount 20 -Frequency "Hour" -Interval 2
```

Xxxx xxxxxxx xxxxxxx x xxxxxxxxx Xxxxxxx xxx xx xxxx xx xxx xxxxxxxxxx xxxxx XxxXxxxxxxxxx00.
Xxx xxxxxxx xxxxxxxxx xxx Xxxxxxx xxxxxxx$ xxxxx xxxx$ xxx XXX xxxxx.
Xxx xxx xxxx 00 xxxxx xx xxxxx$ xxxxx xxxxx xxxx.

## XXXXXXXXXX

### $XxxXxxx
Xxxxxxxxx x xxxx$ xx x XxxxXxxx xxxxxx$ xxx xxx xxxxxxxxx xx xxxx xxxxxxxxxx xxx xxx.
Xx xxxxxx x XxxxXxxx xxxxxx$ xxx xxx Xxx$Xxxx xxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxxx Xxx$Xxxx Xxx$Xxxx.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxXxxxxxXxxxxxx
Xxxxxxxxx xxxxxxx xx x xxxx xxxxx.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxXxxxxxXxxxxx
Xxxxxxxxx xxx xxxxxx xxx XXXX xxx XXXXX xxxxxx xxxxx.
Xxxxx xxxxxx xxx$ 

$$ XXX $$ XXX $$ XXXX $$ XXXX $$ XXXXXX

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxXxxxxxXxxxxXxxxxxxXxxx
Xxxxxxxxx xxx xxxx xxx Xxxxxxx xxx xxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxXxxxxxXxxxxxxXxxx
Xxxxxxxxx xxx xxxx xxx XXX xxx XXXX xxx xxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxXxxxxxXXXXxxxx
Xxxxxxxxx xxx Xxxxxx Xxxxxx Xxxxxxxxx $XXX$ xxxxx xxx xxx Xxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxXxxxxxXxxxxxxXxxxxxx
Xxxxxxxxx xxx xxxx xx xxx Xxxxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxXxxxxxXxxxxxxXxxxx
Xxxxxxxxx xxx xxxx xx xxx Xxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxXxxxxxXXX
Xxxxxxxxx xxx XXX xxx xxx xxxxx xxx xxxxxx.

```yaml
Type: Uri
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxxXxxxx
Xxxxxxxxx xxx xxxxxx xxxxxxxxxxx xx x xxx xxxx xxx.
Xx xxxxxxx$ x xxx xxxxxx xxxxxxxxxxxx.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxxxx
Xxxxxxxxx xxx xxxxxxx xxxxxxxxx xxx xxxx xxxxxxxxx xxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxxx
Xxxxxxxxx xxx xxxxxxxx xx xxxxxxxxxx xx xxx xxxxxxxxx xxxxxxxxx xx xxxxx xxx Xxxxxxxxx xxxxxxxxx.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxXxxxxxxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxxxx xx xxxxxxx xxx xxxxxxxxx xxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxXxxx
Xxxxxxxxx xxx xxxx xxx xxx xxxxxxxxx xxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxXxxxx
Xxxxxxxxx xxx xxxxx xxx xxx xxxxxxxxx xxx.

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

### $Xxxxxxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxx xxxx xxxxx xxx xxxxx xxxxxxx.
Xxxxx xxxxxx xxx$ 

$$ Xxxxxxxx Xxxx $$ Xxxxxxxx Xxxxxx $$ Xxxxxxxx XX $$ Xxxx Xxxx $$ Xxxx XX $$ Xxxxx Xxxxxxx XX $$ Xxxxx Xxxxxx $$ Xxxxx Xxxxxxx XX $$ Xxxxxxxxx Xxxx $$ Xxxx Xxxxxx $$ Xxxx XX

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XXXXxxxx
Xxxxxxxxx xxx XXX xxxxx xxx xxx Xxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxXxxx
Xxxxxxxxx x xxxx$ xx x XxxxXxxx xxxxxx$ xxx xxx xxx xx xxxxx.

```yaml
Type: DateTime
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxXxxxxXxxxxxx
Xxxxxxxxx xxx Xxxxxxx xxxxxxx xxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxxxXxxxxXxxxxxx
Xxxxxxxxx xxx xxxxx xxxxxxx xxx Xxxxxxx xxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxXxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxx Xxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Xxx$XxxxxXxxxxxxxxXxxxxxxXxxxxXxx](29c40d46-86c3-4f67-94f7-484371fdfba5)


