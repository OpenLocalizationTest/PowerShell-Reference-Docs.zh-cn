---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294009
schema: 2.0.0
---

# Xxxxxx$Xxx
## XXXXXXXX
Xxxxx xxxx xx xx XXX xxxxxx xx xxxxxxxx.

## XXXXXX

### Xxx $Xxxxxxx$
```
Select-Xml [-Xml] <XmlNode[]> [-XPath] <String> [-Namespace <Hashtable>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### Xxxx
```
Select-Xml [-Path] <String[]> [-XPath] <String> [-Namespace <Hashtable>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### XxxxxxxXxxx
```
Select-Xml -LiteralPath <String[]> [-XPath] <String> [-Namespace <Hashtable>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### Xxxxxxx
```
Select-Xml -Content <String[]> [-XPath] <String> [-Namespace <Hashtable>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxx$Xxx xxxxxx xxxx xxx xxx XXxxx xxxxxxx xx xxxxxx xxx xxxx xx XXX xxxxxxx xxx xxxxxxxxx.
Xxxxx xx XXxxx xxxxx$ xxx xxx xxx Xxxxxxx$ Xxxx$ xx Xxx xxxxxxxxx xx xxxxxxx xxx XXX xx xx xxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\> $Path = "$pshome\Types.ps1xml"
PS C:\>$XPath = "/Types/Type/Members/AliasProperty"
PS C:\>Select-Xml -Path $path -XPath $xpath | Select-Object -ExpandProperty Node
Name                 ReferencedMemberName
----                 --------------------
Count                Length
Name                 Key
Name                 ServiceName
RequiredServices     ServicesDependedOn
ProcessName          Name
Handles              Handlecount
VM                   VirtualSize
WS                   WorkingSetSize
Name                 ProcessName
Handles              Handlecount
VM                   VirtualMemorySize
WS                   WorkingSet
PM                   PagedMemorySize
NPM                  NonpagedSystemMemorySize
Name                 __Class
Namespace            ModuleName
```

Xxxx xxxxxxx xxxx xxx xxxxx xxxxxxxxxx xx xxx Xxxxx.xx0xxx.
$Xxx xxxxxxxxxxx xxxxx xxxx xxxx$ xxx xxxxx$Xxxxx.xx0xxx.$

Xxx xxxxx xxxxxxx xxxxx xxx xxxx xx xxx Xxxxx.xx0xxx xxxx xx xxx $Xxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxx xxx XXX xxxx xx xxx XxxxxXxxxxxxx xxxx xx xxx $XXxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxxxxx$Xxx xxxxxx xx xxx xxx XxxxxXxxxxxxx xxxxx xxxx xxx xxxxxxxxxx xx xxx XXxxx xxxxxxxxx xxxx xxx Xxxxx.xx0xxx xxxx.
Xxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx xx xxxx xxx XxxxxXxxxxxxx xxxxx xx xxx Xxxxxx$Xxxxxx xxxxxx.
Xxx XxxxxxXxxxxxxx xxxxxxxxx xxxxxxx xxx Xxxx xxxxxx xxx xxxxxxx xxx Xxxx xxx XxxxxxxxxxXxxxxxXxxx xxxxxxxxxx.

Xxx xxxxxx xxxxx xxx Xxxx xxx XxxxxxxxxxXxxxxxXxxx xx xxxx xxxxx xxxxxxxx xx xxx Xxxxx.xx0xxx xxxx.
Xxx xxxxxxx$ xxxxx xx x Xxxxx xxxxxxxx xxxx xx xx xxxxx xx xxx Xxxxxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>[xml]$Types = Get-Content $pshome\Types.ps1xml
PS C:\>Select-Xml -Xml $Types -XPath "//MethodName"
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxx XXX xxxxxxxxx xx xxxxxxx xx XXX xxxxxxxx xx xxx Xxxxxx$Xxx xxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxx xxxxxxx xx xxx Xxxxx.xx0xxx xxxx xxx xxxx xx xx xxx $Xxxxx xxxxxxxx.
Xxx $$$xxx$$$ xxxxx xxx xxxxxxxx xx xx XXX xxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxx$Xxx xxxxxx xx xxx xxx XxxxxxXxxx xxxxx xx xxx Xxxxx.xx0xxx xxxx.
Xxx xxxxxxx xxxx xxx Xxx xxxxxxxxx xx xxxxxxx xxx XXX xxxxxxx xx xxx $Xxxxx xxxxxxxx xxx xxx XXxxx xxxxxxxxx xx xxxxxxx xxx xxxx xx xxx XxxxxxXxxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
The first command creates a hash table that represents the XML namespace that is used for the help files and saves it in the $Namespace variable.
PS C:\>$Namespace = @{command="http://schemas.microsoft.com/maml/dev/command/2004/10"; maml="http://schemas.microsoft.com/maml/2004/10"; dev="http://schemas.microsoft.com/maml/dev/2004/10"}

The second command saves the path to the help files in the $Path variable.If there are no help files in this path on your computer, use the Update-Help cmdlet to download the help files. For more information about Updatable Help, see about_Updatable_Help ( http://go.microsoft.com/fwlink/?LinkId=235801).
PS C:\>$Path = "$pshome\en-us\*dll-Help.xml"

The third command uses the Select-Xml cmdlet to search the XML for cmdlet names by finding Command:Name element anywhere in the files. It saves the results in the $xml variable.Select-Xml returns a SelectXmlInfo object that has a Node property, which is a System.Xml.XmlElement object. The Node property has an InnerXML property, which contains the actual XML that is retrieved.
PS C:\>$Xml = Select-Xml -Path $Path -Namespace $Namespace -XPath "//command:name"

The fourth command sends the XML in the $Xml variable to the Format-Table cmdlet. The Format-Table command uses a calculated property to get the Node.InnerXML property of each object in the $Xml variable, trim the white space before and after the text, and display it in the table, along with the path to the source file.
PS C:\>$Xml | Format-Table @{Label="Name"; Expression= {($_.node.innerxml).trim()}}, Path -AutoSize

Name                    Path
----                    ----
Export-Counter          C:\Windows\system32\WindowsPowerShell\v1.0\en-us\Microsoft.PowerShell.Commands.Diagnostics.dll-Help.xml
Get-Counter             C:\Windows\system32\WindowsPowerShell\v1.0\en-us\Microsoft.PowerShell.Commands.Diagnostics.dll-Help.xml
Get-WinEvent            C:\Windows\system32\WindowsPowerShell\v1.0\en-us\Microsoft.PowerShell.Commands.Diagnostics.dll-Help.xml
Import-Counter          C:\Windows\system32\WindowsPowerShell\v1.0\en-us\Microsoft.PowerShell.Commands.Diagnostics.dll-Help.xml
Add-Computer            C:\Windows\system32\WindowsPowerShell\v1.0\en-us\Microsoft.PowerShell.Commands.Management.dll-Help.xml
Add-Content             C:\Windows\system32\WindowsPowerShell\v1.0\en-us\Microsoft.PowerShell.Commands.Management.dll-Help.xml
Checkpoint-Computer     C:\Windows\system32\WindowsPowerShell\v1.0\en-us\Microsoft.PowerShell.Commands.Management.dll-Help.xml
...
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxx Xxxxxx$Xxx xxxxxx xx xxxxxx xxx Xxxxxxx XxxxxXxxxx XXX$xxxxx xxxxxx xxxx xxxxx.
Xx xxxx xxxxxxx$ xx$xx xxxxxx xxx xxx xxxxxx xxxx xxxx xxxxxx xx x xxxxx xxx xxxx xxxx xxxx xxx xxx xxxx xx xxx xxxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
The first command saves a here-string that contains XML in the $xml variable. (For more information about here-strings, see about_Quoting_Rules.)
PS C:\>$xml = @"
<?xml version="1.0" encoding="utf-8"?>
<Book>
  <projects>
    <project name="Book1" date="2009-01-20">
      <editions>
        <edition language="English">En.Book1.com</edition>
        <edition language="German">Ge.Book1.Com</edition>
        <edition language="French">Fr.Book1.com</edition>
        <edition language="Polish">Pl.Book1.com</edition>
      </editions>
    </project>
  </projects>
</Book>
"@

The second command uses the Content parameter  of Select-Xml to specify the XML in the $xml variable.
PS C:\>Select-Xml -Content $xml -XPath "//edition" | foreach {$_.node.InnerXML}

En.Book1.com
Ge.Book1.Com
Fr.Book1.com
Pl.Book1.com

The third command is equivalent to the second. It uses a pipeline operator (|) to send the XML in the $xml variable to the Select-Xml cmdlet.
PS C:\>$xml | Select-Xml -XPath "//edition" | foreach {$_.node.InnerXML}

En.Book1.com
Ge.Book1.Com
Fr.Book1.com
Pl.Book1.com
```

Xxxx xxxxxxx xxxxx xxx xxxxxxxxx xxxx xx xxxx XXX xx xxx Xxxxxx$Xxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
The first command creates a hash table for the default namespace the that snippet XML files use and assigns it to the $SnippetNamespace variable. The hash table value is the XMLNS schema URI in the snippet XML. The hash table key name, "snip," is arbitrary. You can use any name that is not reserved, but you cannot use "xmlns."
PS C:\>$SnippetNamespace = @{snip="http://schemas.microsoft.com/PowerShell/Snippets"}

The second command uses the Select-Xml cmdlet to get the content of the Title element of each snippet. It uses the Path parameter to specify the Snippets directory and the Namespace parameter to specify the namespace in the $SnippetNamespace variable. The value of  the XPath parameter is the "snip" namespace key, a colon (:), and the name of the Title element.The command uses a pipeline operator (|) to send each Node property that Select-Xml returns to the ForEach-Object cmdlet, which gets the title in the value of the InnerXml property of the node.
PS C:\>Select-Xml -Path $home\Documents\WindowsPowerShell\Snippets -Namespace $SnippetNamespace -XPath "//snip:Title" | foreach {$_.Node.Innerxml}
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxx Xxxxxx$Xxx xxxxxx xxxx XXX xxxxxxxxx xxxx xxx xxx xxxxxxx $xxxxx$ xxxxxxxxx.
Xxx xxxxxxx xxxx xxx xxxxxx xx Xxxxxxx XxxxxXxxxx XXX xxxx$xxxxxxx xxxxxxx xxxxx.
Xxx xxxxxxxxxxx xxxxx xxxxxxxx$ xxx Xxx$XxxXxxxxxx.

## XXXXXXXXXX

### $Xxxxxxx
Xxxxxxxxx x xxxxxx xxxx xxxxxxxx xxx XXX xx xxxxxx.
Xxx xxx xxxx xxxx xxxxxxx xx Xxxxxx$Xxx.

```yaml
Type: String[]
Parameter Sets: Content
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### $XxxxxxxxxxxXxxxxx
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

### $XxxxxxxxxxxXxxxxxxx
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

### $Xxxxxxxxx
Xxxxxxxxx x xxxx xxxxx xx xxx xxxxxxxxxx xxxx xx xxx XXX.
Xxx xxx xxxxxx $$$$xxxxxxxxxXxxx$$ $ $$xxxxxxxxxXxxxx$$$.

Xxxx xxx XXX xxxx xxx xxxxxxx xxxxxxxxx$ xxxxx xxxxxx xxxx $xxxxx$$ xxx xx xxxxxxxxx xxx xxx xxx xxxxxxxxx xxxx.
Xxx xxxxxx xxx $xxxxx$.
Xx xxx XXxxx xxxxxxxxx$ xxxxxx xxxx xxxx xxxx xxxx xxx xxxxxxxxx xxxx xxx x xxxxx$ xxxx xx $$$xxxxxxxxxXxxx$Xxxx$.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxx
Xxxxxxxxx xxx xxxx xxx xxxx xxxxx xx xxx XXX xxxxx xx xxxxxx.
Xxxxxxxx xxxxxxxxxx xxx xxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: Path
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XXxxx
Xxxxxxxxx xx XXxxx xxxxxx xxxxx.
Xxx xxxxx xxxxxxxx xx xxxx$xxxxxxxxx.
Xxxx xxxxxxxxx xx xxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxx
Xxxxxxxxx xxx xx xxxx XXX xxxxx.

Xx XXX xxxxxxxx xxxx xx xxxxxxxxx xx x xxxxxxxxxx xx XXX xxxxx.
Xx xxx xxxx xx XXX xxxxxxxx xx Xxxxxx$Xxx$ xxxx xxxxxxxx xxxx xxxx xx xxxxxxxx xxxxxxxxxx xx xx xxxxx xxxxxxx xxx xxxxxxxx.

```yaml
Type: XmlNode[]
Parameter Sets: Xml
Aliases: Node

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### $XxxxxxxXxxx
Xxxxxxxxx xxx xxxxx xxx xxxx xxxxx xx xxx XXX xxxxx xx xxxxxx.
Xxxxxx Xxxx$ xxx xxxxx xx xxx XxxxxxxXxxx xxxxxxxxx xx xxxx xxxxxxx xx xx xx xxxxx.
Xx xxxxxxxxxx xxx xxxxxxxxxxx xx xxxxxxxxx.
Xx xxx xxxx xxxxxxxx xxxxxx xxxxxxxxxx$ xxxxxxx xx xx xxxxxx xxxxxxxxx xxxxx.
Xxxxxx xxxxxxxxx xxxxx xxxx Xxxxxxx XxxxxXxxxx xxx xx xxxxxxxxx xxx xxxxxxxxxx xx xxxxxx xxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: LiteralPath
Aliases: PSPath

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

### Xxxxxx.Xxxxxx xx Xxxxxx.Xxx.XxxXxxx
Xxx xxx xxxx x xxxx xx XXX xxxx xx Xxxxxx$Xxx.

## XXXXXXX

### Xxxxxxxxx.XxxxxXxxxx.Xxxxxxxx.XxxxxxXxxXxxx

## XXXXX
XXxxx xx x xxxxxxxx xxxxxxxx xxxx xx xxxxxxxx xx xxxxxxxx xxxxx xx xx XXX xxxxxxxx.
Xxx xxxx xxxxxxxxxxx xxxxx xxx XXxxx xxxxxxxx$ xxx xxx $Xxxxxxxxx Xxxxxxx$ xxxxxxx xx xxx $Xxxxx Xxxxxxxxx$ xxxxx xx xxx XXXX $Xxxxxxxxx Xxxxxxxxx Xxxxxxx$ xxxxxxx xx xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXx$000000.
Xxx$ xxx $XXxxx Xxxxxxxxx$ xx xxx XXXX xxxxxxx xx xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXx$000000.

## XXXXXXX XXXXX

[XxxxxxxXx$Xxx]()

