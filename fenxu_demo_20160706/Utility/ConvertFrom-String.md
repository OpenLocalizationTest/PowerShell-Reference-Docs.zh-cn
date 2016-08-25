---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkID=507579
schema: 2.0.0
---

# ConvertFrom-String
## XXXXXXXX
Xxxxxxxx xxx xxxxxx xxxxxxxxxx xxxxxxx xxxx xxxxxx xxxxxxx.

## XXXXXX

### ByDelimiter (Default)
```
ConvertFrom-String [-Delimiter <String>] [-PropertyNames <String[]>] -InputObject <String>
```

### TemplateParsing
```
ConvertFrom-String [-TemplateFile <String[]>] [-TemplateContent <String[]>] [-IncludeExtent] [-UpdateTemplate]
 -InputObject <String>
```

## XXXXXXXXXXX
Xxx xxx xxx xxx XxxxxxxXxxx$Xxxxxx xxxxxx xx xxx xxxxxxxxx xx xxxxxxxxxxxx xxxxxx xxxxxxx.
XxxxxxxXxxx$Xxxxxx xxxxxxxxx xx xxxxxx xx xxxxxxx xxxx xxxx x xxxxxxxxxxx xxxx xxxxxx.
Xxx xxxx xxxxxx xx xxx xxxxxxxx$ xxx xxxxxx xxxxxx xxx xxxxx xx xxxxxx x xxxxxxxxx xx x xxxxx xxxxxxxxxx$ xxx xxxx xxxxxxx xxxxxxxx xxxxx xx xxxx xx xxx xxxxxxxxx xxxxx xxxxxxxx.
Xxx xxx xxxxxxx xxxxx xxxxxxxx xxxxx$ xx xxx xx xxx$ xxxx xxx xxxxxxxxxxxxx xxxxxxxxx xxx xxx.

Xxx xxxxxx$x xxxxxxx xxxxxxxxx xxx$ XxXxxxxxxxx$ xxxxxx xxxxxxx xx xxx xxxxxxx xxxxxxxxxx xxxxxxxxx.
Xx xxxx xxx xxxxxxx xxxxx xxxxxxxx xx xxxxxxxxx xxxxxxxx xx xxx Xxxxxx$Xxx xxxxxx xxxx.

Xxx xxxxxx$x xxxxxxxxx xxxxxxxxx xxx$ XxxxxxxxXxxxxxx$ xxxxxxxxx xxxxxxxx xxxx xxx xxxxxx xxxx xxx xxxxxxxx xx x xxxxxxx xxxxxxxxxx.

Xxxx xxxxxx xxxxxxxx xxx xxxxx$ xxxxx xxxxxxxxx xxxxxxx$ xxx xxxxxxxxxxxxx$xxxxxxxxx$ xxxxxxx$xxxxxx xxxxxxx.

Xxxxxxxxx xxxxxxx$ xx xxxxxxx$ xxxxxx xxx xxxxx xx xxxxx xxxxx$ xxx xxxxxxx xxxxxxxx xxxxx xx xxx xxxxxxxxx xxxxxx.
Xxx xxx xxxxxxxxx xxx xxxxxxxxx xx xxxxxx xxx XxxxxxxXxxx$Xxxxxx xxxxxxx xxxx xxx xx xxx Xxxxxx$$ xxxxxxx$ xx xx xxxxxx xxx Xxxxxxxxx xxxxxxxxx.

Xxx xxxxxx xxxx xxxxxxxx xxxxxxxxxxxxx$xxxxxxxxx$ xxxxxxx$xxxxxx xxxxxxx xxxxx xx xxx XxxxxXxxxxxx xxxxxxxx xxxx xx Xxxxxxxxx Xxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>"Hello World" | ConvertFrom-String
```

Xxx xxxxxxxxx xxxxxxx xxxxxxxxx xx xxxxxx xxxx xxxxxxx xxxxxxxx xxxxx$ X0 xxx X0.
Xxx xxxxxxx xxx $X0$Xxxxx$ xxx $X0$Xxxxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>"Hello World" | ConvertFrom-String -Delimiter "ll"
```

Xxx xxxxxxxxx xxxxxxx xxxxxxxxx xx xxxxxx xxxx $X0$Xx$ xxx $X0$x Xxxxx$$ xx xxxxxxxxxx xxx $xx$ xx $Xxxxx $ xx xxx xxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>"Phoebe Cat" | ConvertFrom-String -TemplateContent {PersonInfo*:{Name:Phoebe Cat}} PS C:\>$template = {PersonInfo*:{Name:Phoebe Cat}}
"Phoebe Cat" | ConvertFrom-String -TemplateContent $template
```

Xxx xxxxxxxxx xxxxxxx xxxx xx xxxxxxxxxx xx xxx xxxxx xx xxx XxxxxxxxXxxxxxx xxxxxxxxx xx xxxxxxxx Xxxxxxx XxxxxXxxxx xxxx xxx xxxxxx xxx$xx xxxxxx xx XxxxxxxXxxx$Xxxxxx xxx x xxxxxxxx xx Xxxx.

Xxx xxx xxxx xxxx xxx xxxxxxxxxx xx x xxxxxxxx$ xxxx xxx xxx xxxxxxxx xx xxx xxxxx xx xxx XxxxxxxxXxxxxxx xxxxxxxxx$ xx xxxxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>"Hello World" | ConvertFrom-String -PropertyNames FirstWord,SecondWord
```

Xxx xxxxxxxxx xxxxxxx xxxxxxxxx xx xxxxxx xxxx xxxxxxxx xxx xxxxxxxxxx$ XxxxxXxxx xxx XxxxxxXxxx.
Xxx xxxxxxx xxx $XxxxxXxxx$Xxxxx$ xxx $XxxxxxXxxx$Xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>"123 456" | ConvertFrom-String -PropertyNames String,Int
```

Xxx xxxxxxxxx xxxxxxx xxxxxxxxx xx xxxxxx xxxx xxxxxxx xxxxxxxx xxxxx X0 xxx X0$ xxx xxxxxxxx xxxxx Xxxxxx xxx Xxx $xxx Xxxxxxx$ xxx xxxxxxxxxx.
Xxx xxxxxxx xxx $X0$000$ xxx $X0$000$.
Xxx xxxxxx xxxxxxxx xx xx xxxxxxx$ xxx x xxxxxx.

## XXXXXXXXXX

### -Delimiter
X xxxxxxx xxxxxxxxxx xxxx xxxxxxxxxx xxx xxxxxxxx xxxxxxx xxxxxxxx.
Xxxxxxxx xxxx xxx xxxxxxx xx xxx xxxxx xxxxxx xxxxxxxxxx xx xxx xxxxxxxxx xxxxxx.
Xxx xxxxxxxxx xx xxxxxxxxxx xxxx xx x xxxx xx Xxxxxx.Xxxx.XxxxxxxXxxxxxxxxxx.XxxxxxxXxxxxxxxxx.Xxxxx$$.

```yaml
Type: String
Parameter Sets: ByDelimiter
Aliases: DEL

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IncludeExtent
Xxxxxxxx xxxxxx xxxx xxxxxxxx xxxx xx xxxxxxx xx xxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: TemplateParsing
Aliases: IE

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Xxxxxxxxx xxxxxxx xxxxxxxx xxxx xxx xxxxxxxx$ xx x xxxxxxxx xxxx xxxxxxxx x xxxxxx xxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PropertyNames
Xxx xx xxxx xxxxxxxx xxxxx xx xxxxx xx xxxxxx xxxxx xxxxxx xx xxx xxxxxxxxx xxxxxx.
Xxxxx xxxx xx xxxx xxxx xxx xxxxx xx xxxxx xxxxxxxxx xxxxxxxx xxxx xxxxxxxxx xxxxxxxx xxxxxx.
Xx xxx xxxxxxx xx xxx xxxxxx xx x xxxxxxx xxxxx$ xxx xxxx xxxxxxx xxxxx xx xxxxx $xxx xxxxxxx$ $$$$xxxx$$$ xx $$$xxxx$$ $$ xxxx xxx xxxx xx xxxx xxxxxxx xxxxx xx xxxxxxxx xx xxx xxxxxxxx.

Xx xxx xxxxxxx xxx xxxxxxxx xx xxx XxxxxxxxXxxx xxxxx$ xxxxx xxxxx xxx xxxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxx xxxx xxxxx.

Xx xxx xxxxxxx xxxx xxxxxxxx xxxxx xxxx xxxxx xxx xxxxxx$ Xxxxxxx XxxxxXxxxx xxxxxxx xxx xxxxx xxxxxxxx xxxxx.
Xx xxx xx xxx xxxxxxx xxxxxx xxxxxxxx xxxxx xx xxxx xxx xxxxxx$ Xxxxxxx XxxxxXxxxx xxxxxxxxxxxxx xxxxxxx xxxxxxxxx xxxxxxxx xxxxx xx xxx xxxxxxxxxx xxxx xxx xxx xxxxx$ X0$ X0$ xxx.

```yaml
Type: String[]
Parameter Sets: ByDelimiter
Aliases: PN

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TemplateContent
Xxxxxxxxx xx xxxxxxxxxx $xx xx xxxxxxxxxx xxxxx xx x xxxxxxxx$ xxxx xxxxxxxxx xxx xxxxxxxxxx xx xxxxx xxx xxxx xx xxxxxx xxxxxxx.
Xxx xxxxxx xx x xxxxxxxx xxxxx xxxxxxxxxxxxx xx xxx xxxxxxxxx$ $$$xxxxxxxx$xxxxxxxx$$xxxx$xxxxxxxx$xxxx$ xxx xxxxxxx $$$xxxxxxx$xxxxx$. Xx xxxxxxx xx $XxxxxxXxxx$$$Xxxx$Xxxxxxxx XxXxxxx$.

```yaml
Type: String[]
Parameter Sets: TemplateParsing
Aliases: TC

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TemplateFile
Xxxxxxxxx x xxxx xxxx xxxxxxxx x xxxxxxxx xxx xxx xxxxxxx xxxxxxx xx xxx xxxxxx.
Xx xxx xxxxxxxx xxxx$ xxxxxxxxxx xxx xxxxx xxxxxx xxx xxxxxxxx xx xxxxxxxx$ xx xxxxx xx xxx xxxxxxxxx xxxxxxx.
Xx x xxxxxxxx $xxxx xx xxx Xxxx xxxxxxxx xx xxxx xxxxxxx$ $xxx xxx xxxxxxxxxx xxxxx xxxxxxxxxx$ xxx xxxxxx xxxxxxxx xxxxx$ xxx xx xxxxxxxx $$$ xx xxxxxxxx xxxx xxxx xxxxxxx xx xxxxxxxx xxxxxxx $xxxxxx xxxx xxxxxxxxxx xxxxxxxx xxxxxxxxxx xxxx x xxxxxx xxxxxx.

$Xxxx$$Xxx Xxxxxxxx$

$Xxxx$Xxxxxxx$$ $Xxxxx$XX$

$Xxxx$$Xxxxxxx Xxxxxx$

$Xxxx$Xxxxxx$$ $Xxxxx$XX$

```yaml
Type: String[]
Parameter Sets: TemplateParsing
Aliases: TF

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UpdateTemplate
Xxxxx xxx xxxxxxx xx x xxxxxxxx xxxxxxxxx xxxx x xxxxxxx xx xxx xxxxxxxx xxxx.
Xxxx xxxxx xxx xxxxxxxxx xxxxxxxx xxxxxxx xxxxxx.
Xx xxx XxxxxxXxxxxxxx$ xxx xxxx xxxx xxxxxxx x xxxxxxxx xxxx xxxx xxx XxxxxxxxXxxx xxxxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: TemplateParsing
Aliases: UT

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### System.String

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[ConvertFrom-String: Example-based text parsing]()

[ConvertFrom-StringData]()

[ConvertFrom-Csv]()

[ConvertTo-Xml]()

