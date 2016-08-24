---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293943
schema: 2.0.0
---

# Xxx$Xxxx
## XXXXXXXX
Xxxx x Xxxxxxxxx .XXX Xxxxxxxxx xxxx $x xxxxx$ xx x Xxxxxxx XxxxxXxxxx xxxxxxx.

## XXXXXX

### XxxxXxxxxx $Xxxxxxx$
```
Add-Type [-TypeDefinition] <String> [-Language <Language>] [-ReferencedAssemblies <String[]>]
 [-CodeDomProvider <CodeDomProvider>] [-CompilerParameters <CompilerParameters>] [-OutputAssembly <String>]
 [-OutputType <OutputAssemblyType>] [-PassThru] [-IgnoreWarnings] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### XxxxXxxxxx
```
Add-Type [-Name] <String> [-MemberDefinition] <String[]> [-Namespace <String>] [-UsingNamespace <String[]>]
 [-Language <Language>] [-ReferencedAssemblies <String[]>] [-CodeDomProvider <CodeDomProvider>]
 [-CompilerParameters <CompilerParameters>] [-OutputAssembly <String>] [-OutputType <OutputAssemblyType>]
 [-PassThru] [-IgnoreWarnings] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### XxxxXxxx
```
Add-Type [-Path] <String[]> [-ReferencedAssemblies <String[]>] [-CompilerParameters <CompilerParameters>]
 [-OutputAssembly <String>] [-OutputType <OutputAssemblyType>] [-PassThru] [-IgnoreWarnings]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### XxxxXxxxxxxXxxx
```
Add-Type -LiteralPath <String[]> [-ReferencedAssemblies <String[]>] [-CompilerParameters <CompilerParameters>]
 [-OutputAssembly <String>] [-OutputType <OutputAssemblyType>] [-PassThru] [-IgnoreWarnings]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### XxxxXxxxxxxxXxxx
```
Add-Type -AssemblyName <String[]> [-PassThru] [-IgnoreWarnings] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxx xxxxxx xxxx xxx xxxxxx x .XXX Xxxxxxxxx xxxxx xx xxxx Xxxxxxx XxxxxXxxxx xxxxxxx.
Xxx xxx xxxx xxxxxxxxxxx xxxxxxx $xx xxxxx xxx Xxx$Xxxxxx xxxxxx$ xxx xxx xxx xxxxxxx$ xxxx xx xxx xxxxx xxx xxx .XXX Xxxxxxxxx xxxxxx.
Xx xxx xxx xx Xxx$Xxxx xxxxxxx xx xxxx Xxxxxxx XxxxxXxxxx xxxxxxx$ xxx xxxxx xx xxxxxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxx.

Xxx xxx xxxxxxx xxx xxxx xx xxxxxxxxxx xx xxxxxxxx xxxxxxxx xx xxxxxx xxxx xxxxx$ xx xxx xxx xxxxxxx xxx xxxxxx xxxx xxxxxx xx xxxxx xx x xxxxxxxx.
Xxx xxx xxxx xxxxxxx xxxx x xxxxxx xxx Xxx$Xxxx xxxx xxxxxx xxx xxxxxxxx xxx xxxxx.
Xxx xxx xxx xxxx xxxxxxx xx xxxx Xxxxxxxx Xxxxxx $X$Xxxxxx$ xxxxx xx xxxxxxxxx xxxxxxxxx xx Xxxxxxx XxxxxXxxxx.
Xx xxx xxxxxxx xxxxxx xxxx$ Xxx$Xxxx xxxxxxxx xxx xxxxxxxxx xxxxxx xxxx xxx xxxxxxxxx xx xx$xxxxxx xxxxxxxx xxxx xxxxxxxx xxx xxx .XXX Xxxxxxxxx xxxxx.

Xxx xxx xxx xxx xxxxxxxxxx xx Xxx$Xxxx xx xxxxxxx xx xxxxxxxxx xxxxxxxx xxx xxxxxxxx $XXxxxx xx xxx xxxxxxx$$ xxxxxxxx xxxxxxx$ xxxxxxxx xxxxxxxxxxxx$ xxx xxxxx xxxxxxxxx$ xxx xxxxx xx xxx xxxx$ xxx xxx xxxxxxxxx xxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$source = @"
public class BasicTest
{
  public static int Add(int a, int b)
    {
        return (a + b);
    }
  public int Multiply(int a, int b)
    {
    return (a * b);
    }
}
"@

PS C:\>Add-Type -TypeDefinition $source
PS C:\>[BasicTest]::Add(4, 3)
PS C:\>$basicTestObject = New-Object BasicTest
PS C:\>$basicTestObject.Multiply(5, 2)
```

Xxxxx xxxxxxxx xxx xxx XxxxxXxxx xxxxx xx xxx xxxxxxx xx xxxxxxxxxx xxxxxx xxxx xxxx xx xxxxxx xx x xxxxxxxx.
Xxx xxxx xxx x xxxxxx xxxxxx xxxxxx Xxx xxx x xxx$xxxxxx xxxxxx xxxxxx Xxxxxxxx.

Xxx xxxxx xxxxxxx xxxxxx xxx xxxxxx xxxx xxx xxx xxxxx xx xxx $xxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxx$Xxxx xxxxxx xx xxx xxx xxxxx xx xxx xxxxxxx.
Xxxxxxx xx xx xxxxx xxxxxx xxxxxx xxxx$ xxx xxxxxxx xxxx xxx XxxxXxxxxxxxxx xxxxxxxxx xx xxxxxxx xxx xxxx xx xxx $xxxxxx xxxxxxxx.

Xxx xxxxxxxxx xxxxxxxx xxx xxx xxx xxxxx.

Xxx xxxxx xxxxxxx xxxxx xxx Xxx xxxxxx xxxxxx xx xxx XxxxxXxxx xxxxx.
Xx xxxx xxx xxxxxx$xxxxx xxxxxxxxxx $$$$ xx xxxxxxx x xxxxxx xxxxxx xx xxx xxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxx$Xxxxxx xxxxxx xx xxxxxxxxxxx xx xxxxxxxx xx xxx XxxxxXxxx xxxxx.
Xx xxxxx xxx xxx xxxxxx xx xxx $xxxxxXxxxXxxxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxxxxxxx xxxxxx xx $xxxxxXxxxXxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>[BasicTest] | Get-Member
PS C:\>[BasicTest] | Get-Member -Static
PS C:\>$basicTestObject | Get-Member
PS C:\>[BasicTest] | Get-Member

TypeName: System.RuntimeType
Name                           MemberType Definition
----                           ---------- ----------
Clone                          Method     System.ObjectClone(
Equals                         Method     System.BooleanEquals
FindInterfaces                 Method     System.Type[] FindInt...

PS C:\>[BasicTest] | Get-Member -static

TypeName: BasicTest
Name            MemberType Definition
----            ---------- ----------
Add             Method     static System.Int32 Add(Int32 a, Int32 b)
Equals          Method     static System.Boolean Equals(Object objA,
ReferenceEquals Method     static System.Boolean ReferenceEquals(Obj

PS C:\>$basicTestObject | Get-Member

TypeName: BasicTest
Name        MemberType Definition
----        ---------- ----------
Equals      Method     System.Boolean Equals(Object obj)
GetHashCode Method     System.Int32 GetHashCode()
GetType     Method     System.Type GetType()
Multiply    Method     System.Int32 Multiply(Int32 a, Int32 b)
ToString    Method     System.String ToString()
```

Xxxxx xxxxxxxx xxx xxx Xxx$Xxxxxx xxxxxx xx xxxxxxx xxx xxxxxxx xxxx xxx Xxx$Xxxx xxx Xxx$Xxxxxx xxxxxxx xxxxxxx xx xxx xxxxxxxx xxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxxxx xxxxxx xx xxx xxx xxxx xxx xxxxxxx xx xxx XxxxxXxxx xxxxx xxxx Xxx$Xxxx xxxxx xx xxx xxxxxxx.
Xxx Xxx$Xxxxxx xxxxxxx xxxxxxx xxxx xx xx x Xxxxxx.XxxxxxxXxxx xxxxxx$ xxxxx xx xxxxxxx xxxx xxx Xxxxxx.Xxxxxx xxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxx xxxxxxxxx xx xxx Xxx$Xxxxxx xxxxxx xx xxx xxx xxxxxx xxxxxxxxxx xxx xxxxxxx xx xxx XxxxxXxxx xxxxx.
Xxx xxxxxx xxxxx xxxx xxx Xxx xxxxxx xx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxxxx xxxxxx xx xxx xxx xxxxxxx xx xxx xxxxxx xxxxxx xx xxx $XxxxxXxxxXxxxxx xxxxxxxx.
Xxxx xxx xxx xxxxxx xxxxxxxx xxxx xxx xxxxxxx xx xxxxx xxx Xxx$Xxxxxx xxxxxx xxxx xxx $XxxxxXxxx xxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx xxxxx xx xxx $XxxxxXxxxXxxxxx xxxxxxxx xx xx xxxxxxxx xx xxx XxxxxXxxx xxxxx xxx xxxx xx xxxxxxxx x xxxxxx xxxxxx Xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$accType = Add-Type -AssemblyName accessib* -PassThru
```

Xxxx xxxxxxx xxxx xxx xxxxxxx xxxx xxx Xxxxxxxxxxxxx xxxxxxxx xx xxx xxxxxxx xxxxxxx.
Xxx xxxxxxx xxxx xxx XxxxxxxxXxxx xxxxxxxxx xx xxxxxxx xxx xxxx xx xxx xxxxxxxx.
Xxx xxxxxxxx xxxxxxxxx xxxxxx xxx xx xxx xxx xxxxxxx xxxxxxxx xxxx xxxx xxx xxx xxx xxxx xx xxx xxxx xx xxx xxxxxxxx.

Xxx xxxxxxx xxxx xxx XxxxXxxx xxxxxxxxx xx xxxxxxxx xxxxxxx xxxx xxxxxxxxx xxx xxxxxxx xxxx xxx xxxxx xx xxx xxxxxxx$ xxx xx xxxxx xxx xxxxxxx xx xxx $xxxXxxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Add-Type -Path c:\ps-test\Hello.vb[VBFromFile]::SayHello(", World")

# From Hello.vb

Public Class VBFromFilePublic Shared Function SayHello(sourceName As String) As StringDim myValue As String = "Hello"return myValue + sourceNameEnd FunctionEnd Class
PS C:\>[VBFromFile]::SayHello(", World")Hello, World
```

Xxxx xxxxxxx xxxx xxx Xxx$Xxxx xxxxxx xx xxx xxx XXXxxxXxxx xxxxx xxxx xx xxxxxxx xx xxx Xxxxx.xx xxxx xx xxx xxxxxxx xxxxxxx.
Xxx xxxx xx xxx Xxxxx.xx xxxx xx xxxxx xx xxx xxxxxxx xxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxx xxxxxx xx xxx xxx xxxx xxxxxxx xx xxx Xxxxx.xx xxxx xx xxx xxxxxxx xxxxxxx.
Xxx xxxxxxx xxxx xxx Xxxx xxxxxxxxx xx xxxxxxx xxx xxxxxx xxxx.

Xxx xxxxxx xxxxxxx xxxxx xxx XxxXxxxx xxxxxxxx xx x xxxxxx xxxxxx xx xxx XXXxxxXxxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$signature = @"
[DllImport("user32.dll")]public static extern bool ShowWindowAsync(IntPtr hWnd, int nCmdShow);
"@
$showWindowAsync = Add-Type -MemberDefinition $signature -Name "Win32ShowWindowAsync" -Namespace Win32Functions -PassThru 

# Minimize the Windows PowerShell console

$showWindowAsync::ShowWindowAsync((Get-Process -Id $pid).MainWindowHandle, 2)

# Restore it

$showWindowAsync::ShowWindowAsync((Get-Process -Id $pid).MainWindowHandle, 4)
```

Xxx xxxxxxxx xx xxxx xxxxxxx xxxxxxxxxxx xxx xx xxxx xxxxxx Xxxxxxx XXXx xx Xxxxxxx XxxxxXxxxx.
Xxx$Xxxx xxxx xxx Xxxxxxxx Xxxxxx $X$Xxxxxx$ xxxxxxxxx xx xxxx x xxxxxxxx xx Xxxx00.xxx xxxx Xxxxxxx XxxxxXxxxx.

Xxx xxxxx xxxxxxx xxxxxx xxx X$ xxxxxxxxx xx xxx XxxxXxxxxxXxxxx xxxxxxxx xx xxx $xxxxxxxxx xxxxxxxx.
$Xxx xxxx xxxxxxxxxxx$ xxx $XxxxXxxxxxXxxxx Xxxxxxxx$ xx xxx XXXX xxxxxxx xx xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXx$000000.$ Xx xxxxxx xxxx xxx xxxxxxxxx xxxxxx xxxx xx xxxxxxx xx x Xxxxxxx XxxxxXxxxx xxxxxxx$ xxx $xxxxxx$ xxxxxxx xxx xxxx xxxxx xx xxx xxxxxxxx xxxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxx$Xxxx xxxxxx xx xxx xxx XxxxXxxxxxXxxxx xxxxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxx xx x xxxxxx xxxxxx xx x xxxxx xxxx Xxx$Xxxx xxxxxxx.
Xxx xxxxxxx xxxx xxx XxxxxxXxxxxxxxxx xxxxxxxxx xx xxxxxxx xxx xxxxxx xxxxxxxxxx xxxxx xx xxx $xxxxxxxxx xxxxxxxx.

Xxx xxxxxxx xxxx xxx Xxxx xxx Xxxxxxxxx xxxxxxxxxx xx xxxxxxx x xxxx xxx xxxxxxxxx xxx xxx xxxxx.
Xx xxxx xxx XxxxXxxx xxxxxxxxx xx xxxxxxxx xx xxxxxx xxxx xxxxxxxxxx xxx xxxxx$ xxx xx xxxxx xxx xxxxxx xx xxx $xxxxXxxxxxXxxxx xxxxxxxx.

Xxx xxxxx xxx xxxxxx xxxxxxxx xxx xxx xxx XxxxXxxxxxXxxxx xxxxxx xxxxxx.
Xxx xxxxxx xxxxx xxx xxxxxxxxxx$ xxx xxxxxx xxxxxx$ xxx xx xxxxxxx xxxxxxxxx xxx xxx xxxxxx xx xx xx xxxxx.

Xxx xxxxx xxxxxxx xxxxx XxxxXxxxxxXxxxx.
Xx xxxx xxx Xxx$Xxxxxxx xxxxxx xxxx xxx $xxx xxxxxxxxx xxxxxxxx xx xxx xxx xxxxxxx xxxx xx xxxxxxx xxx xxxxxxx Xxxxxxx XxxxxXxxxx xxxxxxx.
Xxxx xx xxxx xxx XxxxXxxxxxXxxxxx xxxxxxxx xx xxx xxxxxxx xxxxxxx xxx x xxxxx xx $0$$ xxxxx xxxxxxxxxx xxx XX$XXXXXXXX xxxxx.

Xx xxxxxxx xxx xxxxxx$ xxx xxxxxx xxxxxxx xxx x xxxxx xx $0$ xxx xxx xxxxxx xxxxxxxx$ xxxxx xxxxxxxxxx xxx XX$XXXXXXX xxxxx.
$XX$XXXXXXXX xx 0.$

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Add-Type -MemberDefinition $jsMethod -Name "PrintInfo" -Language JScript
```

Xxxx xxxxxxx xxxx xxx Xxx$Xxxx xxxxxx xx xxx x xxxxxx xxxx xxxxxx XXxxxxx xxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxx.
Xx xxxx xxx XxxxxxXxxxxxxxxx xxxxxxxxx xx xxxxxx xxxxxx xxxx xxxxxx xx xxx $xxXxxxxx xxxxxxxx.
Xx xxxx xxx Xxxx xxxxxxxxx xx xxxxxxx x xxxx xxx xxx xxxxx xxxx Xxx$Xxxx xxxxxxx xxx xxx xxxxxx xxx xxx Xxxxxxxx xxxxxxxxx xx xxxxxxx xxx XXxxxxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Add-Type -Path FSharp.Compiler.CodeDom.dll
PS C:\>Add-Type -Path FSharp.Compiler.CodeDom.dll
PS C:\>$Provider = New-Object Microsoft.FSharp.Compiler.CodeDom.FSharpCodeProvider
PS C:\>$fSharpCode = @"
let rec loop n =if n <= 0 then () else beginprint_endline (string_of_int n);loop (n-1)end
"@
PS C:\>$fsharpType = Add-Type -TypeDefinition $fSharpCode -CodeDomProvider $Provider -PassThru | where { $_.IsPublic }
PS C:\>$fsharpType::loop(4)4321
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxx Xxx$Xxxx xxxxxx xx xxx xx XXxxxx xxxx xxxxxxxx xx xxxx Xxxxxxx XxxxxXxxxx xxxxxxx.
Xx xxx xxxx xxxxxxx xx Xxxxxxx XxxxxXxxxx$ xxx xxxx xxxx xxx XXxxxx.Xxxxxxxx.XxxxXxx.xxx xxxx xx xxxxxxxxx xxxx xxx XXxxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xx xxx xxxxxxx xxxx xxx Xxx$Xxxx xxxxxx xxxx xxx Xxxx xxxxxxxxx xx xxxxxxx xx xxxxxxxx.
Xxx$Xxxx xxxx xxx xxxxx xx xxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxx$Xxxxxx xxxxxx xx xxxxxx xx xxxxxxxx xx xxx XXxxxx xxxx xxxxxxxx xxx xxxxx xxx xxxxxx xx xxx $Xxxxxxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxxx xxx XXxxxx xxxx xxxx xxxxxxx xxx Xxxx xxxxxx xx xxx $XXxxxxXxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxx$Xxxx xxxxxx xx xxxx xxx xxxxxx xxxxx xxxxxxx xx $xXxxxxXxxx xx xxx $xXxxxxXxxx xxxxxxxx.
Xxx XxxxXxxxxxxxxx xxxxxxxxx xxxxxxxxx xxx xxxxxx xxxx xxxx xxxxxxx xxx xxxxx.
Xxx XxxxXxxXxxxxxxx xxxxxxxxx xxxxxxxxx xxx xxxxxx xxxx xxxxxxxx.

Xxx XxxxXxxx xxxxxxxxx xxxxxxx Xxx$Xxxx xx xxxxxx x Xxxxxxx xxxxxx xxxx xxxxxxxxxx xxx xxxxx xxx x xxxxxxxx xxxxxxxx $$$ xxxxx xxx Xxxxxxx xxxxxx xx xxx Xxxxx$Xxxxxx xxxxxx$ xxxxx xxxxxxx xxxx xxx xxxxxx xxxxx.
Xxx Xxxxx$Xxxxxx xxxxxx xx xxxx xxxxxxx xxx XXxxxx xxxxxxxx xxxxxxxxx xxx$xxxxxx xxxxx xx xxxxxxx xxx xxxxxxxxx xxxxxx xxxx.

Xxx xxxxx xxxxxxx xxxxx xxx Xxxx xxxxxx xx x xxxxxx xxxxxx xx xxx xxxx xxxxxx xx xxx $xXxxxxXxxx xxxxxxxx.

## XXXXXXXXXX

### $XxxxxxxxXxxx
Xxxxxxxxx xxx xxxx xx xx xxxxxxxx xxxx xxxxxxxx xxx xxxxx.
Xxx$Xxxx xxxxx xxx xxxxx xxxx xxx xxxxxxxxx xxxxxxxx.
Xxxx xxxxxxxxx xx xxxxxxxx xxxx xxx xxx xxxxxxxx xxxxx xxxxx xx xx xxxxxxxx xxxx.

Xxxxx xxx xxxx xx xxxxxx xxxx $xxxx xxxxx xx xxx $xxxxxxx xxxx$$ xx xx xxxxxxxx.
Xxxxxxxx xxxxxxxxxx xxx xxxxxxxxx xx xxx xxxxxxxx xxxx.
Xx xxx xxxxx x xxxxxx xx xxxxxxx xxxx$ Xxx$Xxxx xxxxxxxx xx xx xxx xxxx xxxx$ xxx xxxx xxxx xxx xxxx xxxx xx xxxx xxx xxxxxxxx.

Xxxx xxxxxxxxx xxxx xxx xxxxxx x xxxx xx xxxx xxxx.
Xx xxxxx xxx xxxx xx xxx xxxxxxxx xxxxxxx$xxxx xxxxxxx $XXX$ xxxx$ xxx xxx Xxxx xxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: FromAssemblyName
Aliases: AN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxXxxxxxxx
Xxxxxxxxx x xxxx xxxxxxxxx xx xxxxxxxx.
Xxx$Xxxx xxxx xxx xxxxxxxxx xxxxxxxx xx xxxxxxx xxx xxxxxx xxxx.
Xxx xxxxxxx xx xxx XXxxxx xxxxxxxx. Xxx xxxx xxxxxxxxx xx xxx xxx xxxxx x xxxxxxxx xxxx xxxxxx xx xxxxxxxxx xx xxxxx xxx Xxxxxxxx xxxxxxxxx.
Xxx XxxxXxxXxxxxxxx xxxx xxx xxxxxxx xxxx xx xxxx xx xxxxxxxx xxxxxxxxxx xxxx xxxxxx xxxx.

```yaml
Type: CodeDomProvider
Parameter Sets: FromSource, FromMember
Aliases: Provider

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxXxxxxxxxxx
Xxxxxxxxx xxx xxxxxxx xxx xxx xxxxxx xxxx xxxxxxxx.
Xxxxx xxxxxxx xxx xxxx xx xxx xxxxxxxx xxxxxxx xxxxxxxx.

Xxxx xxxxxxxxx xxxxxx xxx xx xxxxxx xxx xxxxxxxx xx xxxxxxxx xx xxxxxxxxxx xxxx$ xxxxx xxxxxxxxx$ xx xxx xxxxxxx$xxxx xxxxxxx$ xxxx xx xxx $$xxxxxx$ xxxxxx.
Xxxx xxxxxxxxx xxxxxxxxxx xxx XxxxxxxxXxxxxxxxxx xxxxx $Xxxxxx.XxxxXxx.Xxxxxxxx.XxxxxxxxXxxxxxxxxx$.

Xxx xxxxxx xxx xxx XxxxxxxxXxxxxxxxxx xxx XxxxxxxxxxXxxxxxxxxx xxxxxxxxxx xx xxx xxxx xxxxxxx.

```yaml
Type: CompilerParameters
Parameter Sets: FromSource, FromMember, FromPath, FromLiteralPath
Aliases: CP

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxXxxxxxxx
Xxxxxxx xxxxxxxx xxxxxxxx.
Xxx xxxx xxxxxxxxx xx xxxxxxx Xxx$Xxxx xxxx xxxxxxxx xxxxxxxx xxxxxxxx xx xxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxxxxXxxxxx
Xxxxx xxx xxxx xx xxxxxx xxxx $xxxx xxxxx xx xxx $xxxxxxx xxxx$$ xx xx xxxxxxxx.
Xxxxxxxx xxxxxxxxxx xxx xxxxxxxxx xx xxx xxxxxxxx xxxx.
Xx xxx xxxxx x xxxxxx xx xxxxxxx xxxx$ Xxx$Xxxx xxxxxxxx xx xx xxx xxxx xxxx$ xxx xxxx xxxx xxx xxxx xxxx xx xxxx xxx xxxxxxxx.

Xxxx xxxxxxxxx xxxx xxx xxxxxx x xxxx xx xxxx xxxx.
Xx xxxxx xxx xxxx xx xxx xxxxxxxx xxxxxxx$xxxx xxxxxxx $XXX$ xxxx$ xxx xxx Xxxx xxxxxxxxx.

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
Xxxxx xxx xxxx xx xxxxxx xxxx $xxxx xxxxx xx xxx $xxxxxxx xxxx$$ xx xx xxxxxxxx.
Xxxxxxxx xxxxxxxxxx xxx xxxxxxxxx xx xxx xxxxxxxx xxxx.
Xx xxx xxxxx x xxxxxx xx xxxxxxx xxxx$ Xxx$Xxxx xxxxxxxx xx xx xxx xxxx xxxx$ xxx xxxx xxxx xxx xxxx xxxx xx xxxx xxx xxxxxxxx.

Xxxx xxxxxxxxx xxxx xxx xxxxxx x xxxx xx xxxx xxxx.
Xx xxxxx xxx xxxx xx xxx xxxxxxxx xxxxxxx$xxxx xxxxxxx $XXX$ xxxx$ xxx xxx Xxxx xxxxxxxxx.

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

### $Xxxxxxxx
Xxxxxxxxx xxx xxxxxxxx xxxx xx xxxx xx xxx xxxxxx xxxx.
Xxx Xxx$Xxxx xxxxxx xxxx xxx xxxxx xx xxxx xxxxxxxxx xx xxxxxx xxx xxxxxxxxxxx XxxxXxxXxxxxxxx.
Xxxxx xxxxxx xxx $XXxxxx$$ $XXxxxxXxxxxxx0$$ $XxxxxxXxxxx$$ xxx $XXxxxxx$.
$XXxxxx$ xx xxx xxxxxxx xxxxx.

```yaml
Type: Language
Parameter Sets: FromSource, FromMember
Aliases: 
Accepted values: CSharp, CSharpVersion2, CSharpVersion3, JScript, VisualBasic

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxxxxx xxxx xxxxx xx xxxxxxxx XXX xxxxx xxxx xxxxxxx xxx xxxxx.
Xxxxxx Xxxx$ xxx xxxxx xx xxx XxxxxxxXxxx xxxxxxxxx xx xxxx xxxxxxx xx xx xx xxxxx.
Xx xxxxxxxxxx xxx xxxxxxxxxxx xx xxxxxxxxx.
Xx xxx xxxx xxxxxxxx xxxxxx xxxxxxxxxx$ xxxxxxx xx xx xxxxxx xxxxxxxxx xxxxx.
Xxxxxx xxxxxxxxx xxxxx xxxx Xxxxxxx XxxxxXxxxx xxx xx xxxxxxxxx xxx xxxxxxxxxx xx xxxxxx xxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: FromLiteralPath
Aliases: PSPath

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxXxxxxxxxxx
Xxxxxxxxx xxx xxxxxxxxxx xx xxxxxxx xxx xxx xxxxx.
Xxx$Xxxx xxxxxxxxx xxx xxxxxxxx xxxx xxxx xx xxxxxxxx xx xxxxxxx xxx xxxxxxxxxx xx xxxxxxx.

Xxx xxx xxx xxxx xxxxxxx xx xxxx Xxxxxxxx Xxxxxx $X$Xxxxxx$ xxxxx xx xxxxxxxxx xxxxxxxxx xx Xxxxxxx XxxxxXxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxx xxxxxxxx.

```yaml
Type: String[]
Parameter Sets: FromMember
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxx xx xxxxxx.
Xxxx xxxxxxxxx xx xxxxxxxx xxxx xxxxxxxxxx x xxxx xxxx x xxxxxx xxxxxxxxxx.

Xxx xxxx xxxx xxx xxxxxxxxx xxxx xx xxxxxx xxxxxx x xxxxxxx.
Xxx xxxxxx xxxxxx x xxxx xx xxxxxx xx.
Xx xxx xxxx xx xxxxxx xxx xxxx xxx x xxxx$ xxx xxxx xxxxxx xxx xxxx xx xxxxx x xxx Xxxxxxx XxxxxXxxxx xxxxxxx.
Xxxxxxxxx$ xxx xxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: FromMember
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxxxx
Xxxxxxxxx x xxxxxxxxx xxx xxx xxxx.

Xx xxxx xxxxxxxxx xx xxx xxxxxxxx xx xxx xxxxxxx$ xxx xxxx xx xxxxxxx xx xxx Xxxxxxxxx.XxxxxXxxxx.Xxxxxxxx.XxxXxxx.XxxxXxxxxxxxxXxxxx xxxxxxxxx.
Xx xxx xxxxxxxxx xx xxxxxxxx xx xxx xxxxxxx xxxx xx xxxxx xxxxxx xxxxx xx x xxxxx xx $xxxx$ xxx xxxx xx xxxxxxxxx xx xxx xxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: FromMember
Aliases: NS

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxXxxxxxxx
Xxxxxxxxx x XXX xxxx xxx xxx xxxxxxxx xxxx xxx xxxxxxxxx xxxx xx xxx xxxxxxxx.
Xxxxx x xxxx $xxxxxxxx$ xxx xxxx xxxx.
Xxxxxxxx xxxxxxxxxx xxx xxxxxxxxx.
Xx xxxxxxx$ Xxx$Xxxx xxxxxxxxx xxx xxxxxxxx xxxx xx xxxxxx.

```yaml
Type: String
Parameter Sets: FromSource, FromMember, FromPath, FromLiteralPath
Aliases: OA

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxXxxx
Xxxxxxxxx xxx xxxxxx xxxx xx xxx xxxxxx xxxxxxxx.
Xxxxx xxxxxx xxx Xxxxxxx$ XxxxxxxXxxxxxxxxxx$ xxx XxxxxxxXxxxxxxxxxx.
Xxx xxxx xxxxxxxxxxx xxxxx xxx xxxxxx$ xxx $XxxxxxXxxxxxxxXxxx Xxxxxxxxxxx$ xx XXXX.

Xx xxxxxxx$ xx xxxxxx xxxx xx xxxxxxxxx.

Xxxx xxxxxxxxx xx xxxxx xxxx xxxx xx xxxxxx xxxxxxxx xx xxxxxxxxx xx xxx xxxxxxx.

```yaml
Type: OutputAssemblyType
Parameter Sets: FromSource, FromMember, FromPath, FromLiteralPath
Aliases: OT
Accepted values: ConsoleApplication, Library, WindowsApplication

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxx
Xxxxxxx x Xxxxxx.Xxxxxxx xxxxxx xxxx xxxxxxxxxx xxx xxxxx xxxx xxxx xxxxx.
Xx xxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxx
Xxxxxxxxx xxx xxxx xx xxxxxx xxxx xxxxx xx xxxxxxxx XXX xxxxx xxxx xxxxxxx xxx xxxxx.

Xx xxx xxxxxx xxxxxx xxxx xxxxx$ Xxx$Xxxx xxxxxxxx xxx xxxx xx xxx xxxxx xxx xxxxxxx xx xx$xxxxxx xxxxxxxx xx xxx xxxxx.
Xxx xxxx xxxx xxxxxxxxx xxxxxxxxx xx xxx xxxxx xx Xxxx xxxxxxxxxx xxx xxxxxxxx xxxx Xxx$Xxxx xxxx.

Xx xxx xxxxxx xx xxxxxxxx xxxx$ Xxx$Xxxx xxxxx xxx xxxxx xxxx xxx xxxxxxxx.
Xx xxxxxxx xx xx$xxxxxx xxxxxxxx xx xxx xxxxxx xxxxxxxx xxxxx$ xxx xxx XxxxxxxxXxxx xxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: FromPath
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxxxXxxxxxxxxx
Xxxxxxxxx xxx xxxxxxxxxx xxxx xxxxx xxx xxxx xxxxxxx.
Xx xxxxxxx$ Xxx$Xxxx xxxxxxxxxx Xxxxxx.xxx xxx Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.xxx.
Xxx xxxxxxxxxx xxxx xxx xxxxxxx xx xxxxx xxxx xxxxxxxxx xxx xxxxxxxxxx xx xxxxxxxx xx xxx xxxxxxx xxxxxxxxxx.

Xxx xxxxxx xxx xxx XxxxxxxxXxxxxxxxxx xxx XxxxxxxxxxXxxxxxxxxx xxxxxxxxxx xx xxx xxxx xxxxxxx.

```yaml
Type: String[]
Parameter Sets: FromSource, FromMember, FromPath, FromLiteralPath
Aliases: RA

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxxxxxxxx
Xxxxxxxxx xxx xxxxxx xxxx xxxx xxxxxxxx xxx xxxx xxxxxxxxxxx.
Xxxxx xxx xxxxxx xxxx xx x xxxxxx xx xxxx$xxxxxx$ xx xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxx xxxx.
Xxx xxxx xxxxxxxxxxx xxxxx xxxx$xxxxxxx$ xxx xxxxx$Xxxxxxx$Xxxxx $xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXX$000000$.

Xxxxxxx x xxxxxxxxx xxxxxxxxxxx xx xxxx xxxx xxxxxxxxxx.
Xx xxx xxxx xxx xxxxxxxxx xxxxxxxxxxx$ xxxx xxxx xxxxx xxxx xxx xxxx xxxx xx xxxxxxx xxxx xx xxx xxxxxxxx xxx xxxxxxx xxxx$ xxxxxxx xx xxxxxxxxxxxxx xxxxxxxxx.
Xxx xxxxxxx$ xx xxx xxxxxx x xxxx xxxxxx $Xxxxxxxxx$$ xxxxxxx xxxx xxx $Xxxxxxxxx$ xx xxx xxxxxxxx xxx Xxxxxx.Xxxxxxxxx xxxx xxxx.

```yaml
Type: String
Parameter Sets: FromSource
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxXxxxxxxxx
Xxxxxxxxx xxxxx xxxxxxxxxx xxxx xxx xxxxxxxx xxx xxx xxxxx.
Xxxx xx xxxx xxxx xxx Xxxxx xxxxxxx xx X$.

Xx xxxxxxx$ Xxx$Xxxx xxxxxxxxxx xxx Xxxxxx xxxxxxxxx.
Xxxx xxx XxxxxxXxxxxxxxxx xxxxxxxxx xx xxxx$ Xxx$Xxxx xxxx xxxxxxxxxx xxx Xxxxxx.Xxxxxxx.XxxxxxxXxxxxxxx xxxxxxxxx xx xxxxxxx.
Xxx xxxxxxxxxx xxxx xxx xxx xx xxxxx xxx XxxxxXxxxxxxxx xxxxxxxxx xxx xxxxxxxxxx xx xxxxxxxx xx xxx xxxxxxx xxxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: FromMember
Aliases: Using

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### Xxxx
Xxx xxxxxx xxxx xxxxxxx xx Xxx$Xxxx.

## XXXXXXX

### Xxxx xx Xxxxxx.Xxxx
Xxxx xxx xxx xxx XxxxXxxx xxxxxxxxx$ Xxx$Xxxx xxxxxxx x Xxxxxx.Xxxx xxxxxx xxxx xxxxxxxxxx xxx xxx xxxx.
Xxxxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX
Xxx xxxxx xxxx xxx xxx xxxxx xxxx xx xxx xxxxxxx xxxxxxx. Xx xxx xxx xxxxx xx xxx xxxxxxxx$ xxx xxxx xx xxxx Xxxxxxx XxxxxXxxxx xxxxxxx.
Xxx xxxx xxxxxxxxxxx xxxxx xxx xxxxxxx$ xxx xxxxx$Xxxxxxxx $xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXX$000000$.

Xxxx xxxxx $xxx xxxxxxxxxx$ xxxx xx xxxxxx xxxxxx x xxxxxxx. Xxx xxxxxx xxxxxx x xxxx xx xxxxxx xx.
Xx xxx xxxx xx xxxxxx xxx xxxx xxx x xxxx$ xxx xxxx xxxxxx xxx xxxx xx xxxxx x xxx Xxxxxxx XxxxxXxxxx xxxxxxx.
Xxxxxxxxx$ xxx xxxxxxx xxxxx.

Xxx XxxxXxxXxxxxxxx xxxxx xxx xxxx xxxxxxxxx$ xxxx xx XxxxXxxxxx xxx XXxxxx$ xxxx xxx xxxxxxxx xxxxxx.
Xx x xxxxxx$ xxxxx xxxxxxx xx xxxxx xxxxxxxxx xxxxxx xx xxxx xxxx Xxx$Xxxx.

Xxxx xxxxxx xx xxxxx xx xxx XxxxXxxXxxxxxxx xxxxx.
Xxx xxxx xxxxxxxxxxx xxxxx xxxx xxxxx$ xxx xxx Xxxxxxxxx .XXX Xxxxxxxxx XXX.

## XXXXXXX XXXXX

[Xxx$Xxxxxx]()

[Xxx$Xxxxxx]()

