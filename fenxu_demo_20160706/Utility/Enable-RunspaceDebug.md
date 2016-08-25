---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: 
schema: 2.0.0
---

# Enable-RunspaceDebug
## XXXXXXXX
Xxxxxxx xxxxxxxxx xx xxxxxxxxx xxxxx xxx xxxxxxxxxx xx xxxxxxxxx xxxxx x xxxxxxxx xx xxxxxxxx.

## XXXXXX

### RunspaceNameParameterSet (Default)
```
Enable-RunspaceDebug [-BreakAll] [[-RunspaceName] <String[]>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### RunspaceIdParameterSet
```
Enable-RunspaceDebug [-BreakAll] [-RunspaceId] <Int32[]> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### RunspaceParameterSet
```
Enable-RunspaceDebug [-BreakAll] [-Runspace] <Runspace[]> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### RunspaceInstanceIdParameterSet
```
Enable-RunspaceDebug [-RunspaceInstanceId] <Guid[]> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### ProcessNameParameterSet
```
Enable-RunspaceDebug [[-ProcessName] <String>] [[-AppDomainName] <String[]>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxxx xxxxxxx xx xxxxxx xx x xxxxxx xxxxxxx.

## XXXXXXXX

### 0$
```
PS C:\>
```

### 0$
```
PS C:\>
```

## XXXXXXXXXX

### -AppDomainName
$$Xxxx$$

```yaml
Type: String[]
Parameter Sets: ProcessNameParameterSet
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BreakAll
$$Xxxx$$

```yaml
Type: SwitchParameter
Parameter Sets: RunspaceNameParameterSet, RunspaceIdParameterSet, RunspaceParameterSet
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationAction
$$Xxxx$$

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa
Accepted values: SilentlyContinue, Stop, Continue, Inquire, Ignore, Suspend

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
$$Xxxx$$

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProcessName
$$Xxxx$$

```yaml
Type: String
Parameter Sets: ProcessNameParameterSet
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Runspace
$$Xxxx$$

```yaml
Type: Runspace[]
Parameter Sets: RunspaceParameterSet
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -RunspaceId
$$Xxxx$$

```yaml
Type: Int32[]
Parameter Sets: RunspaceIdParameterSet
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RunspaceInstanceId
$$Xxxx$$

```yaml
Type: Guid[]
Parameter Sets: RunspaceInstanceIdParameterSet
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RunspaceName
$$Xxxx$$

```yaml
Type: String[]
Parameter Sets: RunspaceNameParameterSet
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

