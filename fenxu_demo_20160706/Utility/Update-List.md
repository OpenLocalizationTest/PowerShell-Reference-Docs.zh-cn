---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294024
schema: 2.0.0
---

# Update-List
## XXXXXXXX
Xxxx xxxxx xx xxx xxxxxxx xxxxx xxxx x xxxxxxxx xxxxx xxxx xxxxxxxx x xxxxxxxxxx xx xxxxxxx.

## XXXXXX

### AddRemoveSet (Default)
```
Update-List [-Add <Object[]>] [-Remove <Object[]>] [-InputObject <PSObject>] [[-Property] <String>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### ReplaceSet
```
Update-List -Replace <Object[]> [-InputObject <PSObject>] [[-Property] <String>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxx$Xxxx xxxxxx xxxx xxxxx xx xxx xxxxxxx xxxxx xxxx x xxxxxxxx xxxxx xx xx xxxxxx$ xxx xxxx xx xxxxxxx xxx xxxxxxx xxxxxx.
Xxxx xxxxxx xx xxxxxxxx xxx xxxxxxxxxx xxxx xxxxxxx xxxxxxxxxxx xx xxxxxxx.

Xxx Xxx xxx Xxxxxx xxxxxxxxxx xxx xxxxxxxxxx xxxxx xx xxx xxxxxx xxxx xxxx xxx xxxxxxxxxx.
Xxx Xxxxxxx xxxxxxxxx xxxxxxxx xxx xxxxxx xxxxxxxxxx.

Xx xxx xx xxx xxxxxxx x xxxxxxxx xx xxx xxxxxxx$ Xxxxxx$Xxxx xxxxxxx xx xxxxxx xxxx xxxxxxxxx xxx xxxxxx xxxxxxx xx xxxxxxxx xxx xxxxxx.
Xxx xxx xxxxxx xxx xxxxxx xxxxxx xx xxxxxxx xxxx xxxxxx xxxxxxx$ xxxx xx Xxx$$ xxxxxxx.

Xxxx xxxxxx xxxxx xxxx xxxx xxx xxxxxxxx xxxx xx xxxxx xxxxxxx xxxxxxxx xxx XXxxx xxxxxxxxx xxxx Xxxxxx$Xxxx xxxx.
Xxxx$ xxx Xxx$$ xxxxxxx xxxx xxxxxx xx xxxxxx xxxx xxxxxxx xxx XXxxx xxxxxxxxx.
Xxx xxxx xxxxxxx xxxx xxx xxxxxxxxx xxxx Xxxxxxx XxxxxXxxxx xx xxx xxxxxxx xxxx xxxxxxxxx.
Xx xxxxxxxxx xxxxxxx x xxxxxx xxxxxxxx Xxxxxx$Xxxx$ xxx xxx xxxxxx Xxxx xxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-mailbox | update-list -Property aliases -Add "A","B" -Remove "X","Y" | set-mailbox
```

Xxxx xxxxxxx xxxx X xxx X xxx xxxxxxx X xxx X xxxx xxx Xxxxxxx xxxxxxxx xx x xxxxxxx.

Xxx xxxxxxx xxxx xxx Xxx$XxxxXxx xxxxxx xxxx Xxxxxxxxx Xxxxxxxx Xxxxxx xx xxx xxx xxxxxxx.
X xxxxxxxx xxxxxxxx xxxxx xxx xxxxxxx xxxxxx xx xxx Xxxxxx$Xxxx xxxxxx.

Xxx Xxxxxx$Xxxx xxxxxxx xxxx xxx Xxxxxxxx xxxxxxxxx xx xxxxxxxx xxxx xxx Xxxxxxx xxxxxxxx xx xxx xxxxxxx xx xxxxx xxxxxxx$ xxx xx xxxx xxx Xxx xxx Xxxxxx xxxxxxxxxx xx xxxxxxx xxx xxxxx xxxx xxx xxxxx xxxxx xxx xxxxxxx xxxx xxx xxxxxxxxxx.
Xxx Xxxxxxx xxxxxxxx xxxxxxxx xxx xxxxxxxxxx xx Xxxxxx$Xxxx$ xxxxxxx xx xxxxxx x xxxxxxxxxx xx Xxxxxxxxx .XXX Xxxxxxxxx xxxxxxx xxxx xxxx Xxx xxx Xxxxxx xxxxxxx.

Xxx Xxxxxx$Xxxx xxxxxx xxxxxxx xxx xxxxxxx xxxxxxx$ xxxxx xx xxxxx xx xxx Xxx$XxxxXxx xxxxxx$ xxxxx xxxxxxx xxx xxxxxxx.

Xxx xxxx xxxxxxxxxxx xxxxx Xxx$Xxxxxxx$ xxx xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXx$000000.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$m = get-mailbox
PS C:\>update-list -InputObject $m -Property aliases -Add "A","B" -Remove "X", "Y" | set-mailbox
```

Xxxx xxxxxxx xxxx X xxx X xx xxx xxxxx xx xxx Xxxxxxx xxxxxxxx xx x xxxxxxx xxx xxxxxxx X xxx X. Xxxx xxxxxxx xxx xxx xxxx xxxxxx xx xxx xxxxxxxx xxxxxxx$ xxxxxxxx xx xxx x xxxxxxxx xxxxxxxxx xxxxxx.

Xxx xxxxxxx xxxx xxx Xxx$XxxxXxx xxxxxx xx xxx xxx xxxxxxx$ xxx xx xxxxx xxx xxxxxxx xx xxx $x xxxxxxxx.
Xxxx xxxxxxx xxxx xxx XxxxxXxxxxx xxxxxxxxx xx Xxxxxx$Xxxx xx xxxxxxx xxx xxxxxxx.
Xxx xxxxx xx XxxxxXxxxxx xx xxx xxxxxxx xx xxx $x xxxxxxxx.
Xx xxxx xxx Xxxxxxxx xxxxxxxxx xx xxxxxxx xxx Xxxxxxx xxxxxxxx xxx xxx Xxx xxx Xxxxxx xxxxxxxxxx xx xxxxxxx xxx xxxxx xxxxx xxxxx xx xxx xxxxxxx xxxx xxx xxxxx xx Xxxxxxx.

Xxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxx xxxxxxx xxxxxx xx xxx Xxx$Xxxxxxx xxxxxx$ xxxxx xxxxxxx xxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-mailbox | set-mailbox -alias (update-list -Add "A", "B" -Remove "X","Y")
```

Xxxx xxxxxxx xxxx X xxx X xx xxx xxxxx xx xxx Xxxxxxx xxxxxxxx xx x xxxxxxx xxx xxxxxxx X xxx X. Xxxx xxxxxxx xxx xxx xxxx xxxxxx xx xxx xxx xxxxxxxx xxxxxxxx$ xxx xx xxxx x xxxxxxxxx xxxxxxxxx xx xxxxxxx xxx xxxx.

Xxxxxxx xx xxxxxxxx xxx Xxxxxxx xxxxxxxx xx xxx xxxxxxx xxxxxx xxxxxxx xx xx Xxx$Xxxxxxx$ xxxx xxxxxxx xxxx Xxxxxx$Xxxx xx xxxxxx xx xxxxxx xxxx xxxxxxxxxx xxx xxxxxx.
Xxxx xx xxxxxxx xxx xxxxxx xx xxx Xxxxx xxxxxxxxx xx Xxx$Xxxxxxx.

Xxx xxxxxxx xxxx xxx Xxx$XxxxXxx xxxxxx xx xxx xxx xxxxxxx.
X xxxxxxxx xxxxxxxx xxxxx xxx xxxxxxx xxxxxx xx xxx Xxx$Xxxxxxx xxxxxx$ xxxxx xxxxxxx xxxxxxxxx.

Xxx xxxxxxx xxxx xxx Xxxxx xxxxxxxxx xx Xxx$Xxxxxxx xx xxxxxx xxx Xxxxxxx xxxxxxxx xx xxx xxxxxxx xxxxxx.
Xxx xxxxx xx xxx Xxxxx xxxxxxxxx xx xx Xxxxxx$Xxxx xxxxxxx xxxx xxxxxxx xx xxxxxx xxxx xxxxxxxxxx xxx xxxxxx.
Xxx Xxxxxx$Xxxx xxxxxxx xx xxxxxxxx xx xxxxxxxxxxx xx xxxxxx xxxx xx xxxx xxxxxx xxx xxxxx xx xxx Xxxxx xxxxxxxxx xx xxxxxxxxx.
Xxxx xxx Xxx$Xxxxxxx xxxxxxx xxxxxxxxx$ xxx xxxxxxx xx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>update-list -InputObject $a -Property aliases -replace "A", "B" | set-mailbox
```

Xxxx xxxxxxx xxxx xxx Xxxxxxx xxxxxxxx xx Xxxxxx$Xxxx xx xxxxxxx xxx xxxxxxxxxx xx xxx Xxxxxxx xxxxxxxx xx xxx xxxxxx xx $x xxxx x xxx xxxxxxxxxx.

Xxxx xxxxxxx xxxx xxx XxxxxXxxxxx xxxxxxxxx xxxxx$ xx xxxx xxxx$ xx xxxxxxxxxx xx xxxxx x xxxxxxxx xxxxxxxx xx xxxx $x xx Xxxxxx$Xxxx.

## XXXXXXXXXX

### -Add
Xxxxxxxxx xxx xxxxxxxx xxxxxx xx xx xxxxx xx xxx xxxxxxxxxx.
Xxxxx xxx xxxxxx xx xxx xxxxx xxxx xxxx xxxxxx xxxxxx xx xxx xxxxxxxxxx.

```yaml
Type: Object[]
Parameter Sets: AddRemoveSet
Aliases: 

Required: False
Position: Named
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

### -InputObject
Xxxxxxxxx xxx xxxxxxx xx xx xxxxxxx.
Xxx xxx xxxx xxxx xxx xxxxxx xx xx xxxxxxx xx Xxxxxx$Xxxx.

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Property
Xxxxxxxxxx xxx xxxxxxxx xxxx xxxxxxxx xxx xxxxxxxxxx xxxx xx xxxxx xxxxxxx.
Xx xxx xxxx xxxx xxxxxxxxx$ Xxxxxx$Xxxx xxxxxxx xx xxxxxx xxxx xxxxxxxxxx xxx xxxxxx xxxxxxx xx xxxxxxxx xxx xxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Remove
Xxxxxxxxx xxx xxxxxxxx xxxxxx xx xx xxxxxxx xxxx xxx xxxxxxxxxx.

```yaml
Type: Object[]
Parameter Sets: AddRemoveSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Replace
Xxxxxxxxx x xxx xxxxxxxxxx.
Xxxx xxxxxxxxx xxxxxxxx xxx xxxxx xx xxx xxxxxxxx xxxxxxxxxx xxxx xxx xxxxx xxxxxxxxx xx xxxx xxxxxxxxx.

```yaml
Type: Object[]
Parameter Sets: ReplaceSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### System.Management.Automation.PSObject
Xxx xxx xxxx xxx xxxxxxx xx xx xxxxxxx xx Xxxxxx$Xxxx.

## XXXXXXX

### Objects or System.Management.Automation.PSListModifier
Xxxxxx$Xxxx xxxxxxx xxx xxxxxxx xxxxxx$ xx xx xxxxxxx xx xxxxxx xxxx xxxxxxxxxx xxx xxxxxx xxxxxx.

## XXXXX

## XXXXXXX XXXXX

[Select-Object]()

