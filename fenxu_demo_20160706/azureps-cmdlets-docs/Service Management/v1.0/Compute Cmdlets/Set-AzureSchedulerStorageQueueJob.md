---
external help file: SMAzure_Compute.xml
online version: bb736406-8b48-4bdf-b67b-0c928e674c7d
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Set-AzureSchedulerStorageQueueJob
## XXXXXXXX
Xxxxxxx x xxxxxxxxx xxx xxxx xxx x xxxxxxx xxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Set-AzureSchedulerStorageQueueJob [-Location] <String> [[-Interval] <Int32>] [[-Frequency] <String>]
 [[-EndTime] <DateTime>] [[-ExecutionCount] <Int32>] [[-JobState] <String>] [[-ErrorActionMethod] <String>]
 [[-ErrorActionURI] <Uri>] [[-ErrorActionRequestBody] <String>] [[-ErrorActionHeaders] <Hashtable>]
 [[-ErrorActionStorageAccount] <String>] [-JobCollectionName] <String> [[-ErrorActionStorageQueue] <String>]
 [[-ErrorActionSASToken] <String>] [[-ErrorActionQueueMessageBody] <String>] [-JobName] <String>
 [[-StorageQueueAccount] <String>] [[-StorageQueueName] <String>] [[-SASToken] <String>]
 [[-StorageQueueMessage] <String>] [[-StartTime] <DateTime>] [-PassThru]
```

### UNNAMED_PARAMETER_SET_2
```
Set-AzureSchedulerStorageQueueJob [[-Interval] <Int32>] [[-Frequency] <String>] [[-EndTime] <DateTime>]
 [[-ExecutionCount] <Int32>] [[-JobState] <String>] [[-ErrorActionHeaders] <Hashtable>] [-PassThru]
```

## XXXXXXXXXXX
Xxxx xxxxx xxxxxxxxx xxx xxxxxx xx xxx 0.0.00 xxxxxxx xx xxx Xxxxxxxxx Xxxxx XxxxxXxxxx xxxxxx.
Xx xxx xxx xxxxxxx xx xxx xxxxxx xxx$xx xxxxx$ xx xxx Xxxxx XxxxxXxxxx xxxxxxx$ xxxx $Xxx$Xxxxxx $Xxxx Xxxxx$.Xxxxxxx.

Xxx Xxx$XxxxxXxxxxxxxxXxxxxxxXxxxxXxx xxxxxx xxxxxxx x xxxxxxxxx xxx xxxx xxx xx Xxxxx Xxxxxxx xxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x Xxxxxxx xxxxx xxxxxxx
```
PS C:\>Set-AzureSchedulerStorageQueueJob -Location "North Central US" -JobCollectionName "JobCollection01 -JobName "Job12" -StorageQueueMessage "Updated message"
```

Xxxx xxxxxxx xxxxxxx xxx xxxxx xxxxxxx xxx xxx Xxxxxxx xxx xxxxx Xxx00.
Xxx xxxxxxx xxxxxxxxx xxx xxx xxxxxxxxxx xxxx xxx xxx xxxxxxxx.

### Xxxxxxx 0$ Xxxxxx x Xxxxxxx xxxxx xxx
```
PS C:\>Set-AzureSchedulerStorageQueueJob -Location "North Central US" -JobCollectionName "JobCollection02" -JobName "Job16" -JobState "Enabled"
```

Xxxx xxxxxxx xxxxxxx xxx xxx xxxxx Xxx00.
Xxx xxxxxxx xxxxxxx xxx xxxxx xx xxx xxx xx Xxxxxxx xx xxxxxxxxxx xxxx xxxxx xxx xxx XxxXxxxx xxxxxxxxx.

## XXXXXXXXXX

### -EndTime
Xxxxxxxxx x xxxx$ xx x XxxxXxxx xxxxxx$ xxx xxx xxxxxxxxx xx xxxx xxxxxxxxxx xxx xxx.
Xx xxxxxx x XxxxXxxx xxxxxx$ xxx xxx Xxx$Xxxx xxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxxx Xxx$Xxxx Xxx$Xxxx.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases: 

Required: False
Position: 12
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -ErrorActionHeaders
Xxxxxxxxx xxxxxxx xx x xxxx xxxxx.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases: 

Required: False
Position: 18
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ErrorActionMethod
Xxxxxxxxx xxx xxxxxx xxx XXXX xxx XXXXX xxxxxx xxxxx.
Xxxxx xxxxxx xxx$ 

$$ XXX $$ XXX $$ XXXX $$ XXXX $$ XXXXXX

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: 15
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -ErrorActionQueueMessageBody
Xxxxxxxxx xxx xxxx xxx Xxxxxxx xxx xxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: 22
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -ErrorActionRequestBody
Xxxxxxxxx xxx xxxx xxx XXX xxx XXXX xxx xxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: 17
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -ErrorActionSASToken
Xxxxxxxxx xxx Xxxxxx Xxxxxx Xxxxxxxxx $XXX$ xxxxx xxx xxx Xxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: 21
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ErrorActionStorageAccount
Xxxxxxxxx xxx xxxx xx xxx Xxxxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: 19
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ErrorActionStorageQueue
Xxxxxxxxx xxx xxxx xx xxx Xxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: 20
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ErrorActionURI
Xxxxxxxxx xxx XXX xxx xxx xxxxx xxx xxxxxx.

```yaml
Type: Uri
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: 16
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExecutionCount
Xxxxxxxxx xxx xxxxxx xxxxxxxxxxx xx x xxx xxxx xxx.
Xx xxxxxxx$ x xxx xxxxxx xxxxxxxxxxxx.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: 13
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -Frequency
Xxxxxxxxx xxx xxxxxxx xxxxxxxxx xxx xxxx xxxxxxxxx xxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 11
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -Interval
Xxxxxxxxx xxx xxxxxxxx xx xxxxxxxxxx xx xxx xxxxxxxxx xxxxxxxxx xx xxxxx xxx Xxxxxxxxx xxxxxxxxx.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: 10
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -JobCollectionName
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxxxx xx xxxxxxx xxx xxxxxxxxx xxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: 2
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -JobName
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxxx xxx xx xxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: 3
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -JobState
Xxxxxxxxx xxx xxxxx xxx xxx xxxxxxxxx xxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 14
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
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: 1
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxxx xx xxxxxx xxxxxxxxxxxx xxx xxxx xx xxxxx xx xxxxxxxx.
Xx xxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

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

### -SASToken
Xxxxxxxxx xxx XXX xxxxx xxx xxx Xxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: 6
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -StartTime
Xxxxxxxxx x xxxx$ xx x XxxxXxxx xxxxxx$ xxx xxx xxx xx xxxxx.

```yaml
Type: DateTime
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: 9
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -StorageQueueAccount
Xxxxxxxxx xxx Xxxxxxx xxxxxxx xxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: 4
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -StorageQueueMessage
Xxxxxxxxx xxx xxxxx xxxxxxx xxx xxx Xxxxxxx xxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: 7
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -StorageQueueName
Xxxxxxxxx xxx xxxx xx xxx Xxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: 5
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[New-AzureSchedulerStorageQueueJob](bb736406-8b48-4bdf-b67b-0c928e674c7d)


