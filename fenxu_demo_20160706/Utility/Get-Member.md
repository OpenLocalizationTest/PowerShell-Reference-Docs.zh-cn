---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293971
schema: 2.0.0
---

# Xxx$Xxxxxx
## XXXXXXXX
Xxxx xxx xxxxxxxxxx xxx xxxxxxx xx xxxxxxx.

## XXXXXX

```
Get-Member [-InputObject <PSObject>] [[-Name] <String[]>] [-MemberType <PSMemberTypes>]
 [-View <PSMemberViewTypes>] [-Static] [-Force] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxxxx xxxxxx xxxx xxx $xxxxxxx$ $xxxxxxxxxx xxx xxxxxxx$ xx xxxxxxx.

Xx xxxxxxx xxx xxxxxx$ xxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxx xx xxxxxx xx Xxx$Xxxxxx.
Xx xxxxxxxx xxxxxxxxxxx xxxxx xxxxxx xxxxxxx $xxxxxxx xx xxx xxxxx$ xxx xx xxx xxxxxxxx$$ xxx xxx Xxxxxx xxxxxxxxx.
Xx xxx xxxx xxxxxxx xxxxx xx xxxxxxx$ xxxx xx XxxxXxxxxxxxxx$ xxx xxx XxxxxxXxxx xxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-service | get-member
TypeName: System.ServiceProcess.ServiceController

Name                      MemberType    Definition
----                      ----------    ----------
Name                      AliasProperty Name = ServiceName
Close                     Method        System.Void Close()
Continue                  Method        System.Void Continue()
CreateObjRef              Method        System.Runtime.Remoting.ObjRef CreateObjRef(Type requestedType)
Dispose                   Method        System.Void Dispose()
Equals                    Method        System.Boolean Equals(Object obj)
ExecuteCommand            Method        System.Void ExecuteCommand(Int32 command)
GetHashCode               Method        System.Int32 GetHashCode()
GetLifetimeService        Method        System.Object GetLifetimeService()
GetType                   Method        System.Type GetType()
InitializeLifetimeService Method        System.Object InitializeLifetimeService()
Pause                     Method        System.Void Pause()
Refresh                   Method        System.Void Refresh()
Start                     Method        System.Void Start(), System.Void Start(String[] args)
Stop                      Method        System.Void Stop()
ToString                  Method        System.String ToString()
WaitForStatus             Method        System.Void WaitForStatus(ServiceControllerStatus desiredStatus), System.Voi...
CanPauseAndContinue       Property      System.Boolean CanPauseAndContinue {get;}
CanShutdown               Property      System.Boolean CanShutdown {get;}
CanStop                   Property      System.Boolean CanStop {get;}
Container                 Property      System.ComponentModel.IContainer Container {get;}
DependentServices         Property      System.ServiceProcess.ServiceController[] DependentServices {get;}
DisplayName               Property      System.String DisplayName {get;set;}
MachineName               Property      System.String MachineName {get;set;}
ServiceHandle             Property      System.Runtime.InteropServices.SafeHandle ServiceHandle {get;}
ServiceName               Property      System.String ServiceName {get;set;}
ServicesDependedOn        Property      System.ServiceProcess.ServiceController[] ServicesDependedOn {get;}
ServiceType               Property      System.ServiceProcess.ServiceType ServiceType {get;}
Site                      Property      System.ComponentModel.ISite Site {get;set;}
Status                    Property      System.ServiceProcess.ServiceControllerStatus Status {get;}
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxxxxxx xxx xxxxxxx xx xxx xxxxxxx xxxxxxx $Xxxxxx.XxxxxxxXxxxxxx.XxxxxxxXxxxxxxxxx$ xxxx xxx xxxxxxxxx xx xxx Xxx$Xxxxxxx xxxxxx.

Xxx xxxxxxx xxxx xxx xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxx xx x Xxx$Xxxxxxx xxxxxxx xx Xxx$Xxxxxx.

Xxxxxxx xxx Xxx$Xxxxxx xxxx xx xxx xxxxxxx xxxx xxx xxxx xxx xxxxxxxxxx$ xx xxxx xxx xx xxx xxxxxxx xxxxxx.
Xx xxxx$ xx xxxx xxx xxxxxx xxxxx$ xxx xx xxxx xxx xxx xxxxxx xxxxxxx xxx xxxx xxx xxxxxxx xxxxxxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-service | get-member -force
PS C:\>(get-service -schedule).psbase
```

Xxxx xxxxxxx xxxx xxx xx xxx xxxxxxx $xxxxxxxxxx xxx xxxxxxx$ xx xxx xxxxxxx xxxxxxx $Xxxxxx.XxxxxxxXxxxxxx.XxxxxxxXxxxxxxxxx$ xxxxxxxxx xx xxx Xxx$Xxxxxxx xxxxxx$ xxxxxxxxx xxx xxxxxxxxx xxxxxxx$ xxxx xx XXXxxx xxx XXXxxxxx$ xxx xxx xxx$ xxx xxx$ xxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxxxxxx xxxx xxxxxxxxx xxx xxxxxxxx xx xxx xxxxxx.
Xx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxx xxxxxxx xx xxx Xxx$Xxxxxx xxxxxx.

Xxx Xxx$Xxxxxx xxxxxxx xxxx xxx Xxxxx xxxxxxxxx xx xxx xxx xxxxxxxxx xxxxxxx xxx xxxxxxxx$xxxxxxxxx xxxxxxx xx xxx xxxxxxx xx xxx xxxxxxx.
Xxx$Xxxxxx xxxx xxxxx xxxxxxx$ xxx xx xxxxx xxxx xx xxxxxxx.

Xxx xxx xxx xxxxx xxxxxxxxxx xxx xxxxxxx xx xxx xxxx xxx xxxx xxx xxxxx xxx xx xxxxxxx xxxxxx xx xxx xxxxxx.
Xxx xxxxxx xxxxxxx xxxxx xxx xx xxxxxxx xxx xxxxx xx xxx XXXxxx xxxxxxxx xx xxx Xxxxxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-service| get-member -view extended
TypeName: System.ServiceProcess.ServiceController

Name MemberType    Definition
---- ----------    ----------
Name AliasProperty Name = ServiceName
```

Xxxx xxxxxxx xxxx xxx xxxxxxx xxx xxxxxxxxxx xx xxxxxxx xxxxxxx xxxx xxxx xxxxxxxx xx xxxxx xxx Xxxxx.xx0xxx xxxx xx xxx Xxx$Xxxxxx xxxxxx.

Xxx Xxx$Xxxxxx xxxxxxx xxxx xxx Xxxx xxxxxxxxx xx xxx xxxx xxx xxxxxxxx xxxxxxx xx xxx xxxxxxx xxxxxxx.
Xx xxxx xxxx$ xxx xxxxxxxx xxxxxx xx xxx Xxxx xxxxxxxx$ xxxxx xx xx xxxxx xxxxxxxx xx xxx XxxxxxxXxxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-eventlog -log system | gm -membertype scriptproperty
TypeName: System.Diagnostics.EventLogEntry

Name    MemberType     Definition
----    ----------     ----------
EventID ScriptProperty System.Object EventID {get=$this.get_EventID() -band 0xFFFF;}
```

Xxxx xxxxxxx xxxx xxx xxxxxx xxxxxxxxxx xx xxxxx xxx xxxxxxx xx xxx Xxxxxx xxx xx Xxxxx Xxxxxx.
Xx xxxx xxxx$ xxx xxxx xxxxxx xxxxxxxx xx xxx XxxxxXX.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-eventlog -log system | get-member -membertype scriptproperty
TypeName: System.Diagnostics.EventLogEntry

Name    MemberType     Definition
----    ----------     ----------
EventID ScriptProperty System.Object EventID {get=$this.get_EventID() -band 0xFFFF;}
```

Xxxx xxxxxxx xxxx xxx xxxxxx xxxxxxxxxx xx xxxxx xxx xxxxxxx xx xxx Xxxxxx xxx xx Xxxxx Xxxxxx.

Xxx xxxxxxx xxxx xxx XxxxxxXxxx xxxxxxxxx xx xxx xxxx xxxxxxx xxxx x xxxxx xx XxxxxXxxxxxxx xxx xxxxx XxxxxxXxxx xxxxxxxx.

Xxx xxxxxxx xxxxxxx xxx XxxxxXX xxxxxxxx xx xxx XxxxxXxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$a = "get-process", "get-service", "get-culture", "get-psdrive", "get-executionpolicy"
PS C:\>foreach ($cmdlet in $a) {invoke-command $cmdlet | get-member -name machinename}
TypeName: System.Diagnostics.Process

Name        MemberType Definition
----        ---------- ----------
MachineName Property   System.String MachineName {get;}

TypeName: System.ServiceProcess.ServiceController

Name        MemberType Definition
----        ---------- ----------
MachineName Property   System.String MachineName {get;set;}
```

Xxxx xxxxxxx xxxx xxxxxxx xxxx xxxx x XxxxxxxXxxx xxxxxxxx xxxx x xxxx xx xxxxxxx.

Xxx xxxxx xxxxxxx xxxxxx xxx xxxxx xx xxxxxxx xxxxxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx x XxxXxxx xxxxxxxxx xx xxxxxx xxxx xxxxxxx$ xxxx xxx xxxxxxx xx Xxx$Xxxxxx$ xxx xxxxx xxx xxxxxxx xxxx Xxx$Xxxxxx xx xxxxxxx xxxx xxxx xxx xxxx $XxxxxxxXxxx.$

Xxx xxxxxxx xxxx xxxx xxxx xxxxxxx xxxxxxx $Xxxxxx.Xxxxxxxxxxx.Xxxxxxx$ xxx xxxxxxx xxxxxxx $Xxxxxx.XxxxxxxXxxxxxx.XxxxxxxXxxxxxxxxx$ xxxx x XxxxxxxXxxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$a = get-member -inputobject @(1)
PS C:\>$a.count
1
PS C:\>$a = get-member -inputobject 1,2,3
TypeName: System.Object[]

Name               MemberType    Definition
----               ----------    ----------
Count              AliasProperty Count = Length
Address            Method        System.Object& Address(Int32 )
Clone              Method        System.Object Clone()
...
PS C:\>$a.count
1
```

Xxxx xxxxxxx xxxxxxxxxxxx xxx xx xxxx xxx xxxxxxxxxx xxx xxxxxxx xx xx xxxxx xx xxxxxxx xxxx xxx xxxx xxxx xxx xxxxxx xx xxx xxxxx xxxx.

Xxxxxxx xxx xxxx xx xxx xxxxxxx xx xx xxxx xxx xxxxxxxxxx xx xx xxxxx$ xxx xxxxx xxxxxxx xxxx xxx XxxxxXxxxxx xxxxxxxxx.
Xx xxxx xxx $xx$ xxxxxx $$$ xx xxxxxxxx xx xxxxx.
Xx xxxx xxxx$ xxx xxxxx xxxxxxxx xxxx xxx xxxxxx$ xxx xxxxxxx 0.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxxxx xxxxxx xx xxx xxx xxxxxxxxxx xxx xxxxxxx xx xx xxxxx xx xxxxxxxx$ xxx xxx xxxxxxx xxxxx xxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxx xxxxxxxx xx xxx xxxxx xx xxxx xxx xxxxxx xx xxxxxxx xx xxx $x xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$file = get-item c:\test\textFile.txt
PS C:\>$file.psobject.properties | where-object {$_.issettable} | format-table -property name

Name
----
PSPath
PSParentPath
PSChildName
PSDrive
PSProvider
PSIsContainer
IsReadOnly
CreationTime
CreationTimeUtc
LastAccessTime
LastAccessTimeUtc
LastWriteTime
LastWriteTimeUtc
Attributes

PS C:\>[appdomain]::CurrentDomain.GetAssemblies() | foreach-object { $_.getexportedtypes() } | foreach-object {$_.getproperties() | where-object {$_.canwrite }} | select-object reflectedtype, name
```

Xxxx xxxxxxx xxxxx xxx xx xxxxxxxxx xxxxx xxxxxxxxxx xx xx xxxxxx xxx xx xxxxxxx.
Xxx xxxxxxx xxxx x xxxx$ xxx xxx xxx xxx xxxx xxxxxxx xxxxxx xx xxxx xxx xxxxxxxxxx xxxxxxxxxx xx xxx xxxxxx xx Xxxxxxx XxxxxXxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxx xxxxxx xx xxx x xxxx xxxx$ xxx xxxx xx xxxxx xxx xxxx xxxxxx xx xxx $xxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx xx xxx xxxxxxxxxx xxxxxxxxxx xx xxx xxxx xxxxxx xx xxx $xxxx xxxxxxxx xxx xxxxxxxx xxx xxxxx xx xxx xxxxxxxxxx xx x xxxxx.

Xxx xxxxx xxxxxxx xxxx xxx xxxxxxxxxx xxxxxxxxxx xx xxx xxxxxxx xx xxxx Xxxxxxx XxxxxXxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$s = get-service
PS C:\>$s | get-member
TypeName: System.ServiceProcess.ServiceController

Name                      MemberType    Definition
----                      ----------    ----------
Name                      AliasProperty Name = ServiceName
RequiredServices          AliasProperty RequiredServices = ServicesDependedOn
Disposed                  Event         System.EventHandler Disposed(System.Object, System.EventArgs
Close                     Method        System.Void Close()
Continue                  Method        System.Void Continue()
CreateObjRef              Method        System.Runtime.Remoting.ObjRef CreateObjRef(type requestedTy
Dispose                   Method        System.Void Dispose()
...
PS C:\>get-member -inputObject $s
TypeName: System.Object[]

Name           MemberType    Definition
----           ----------    ----------
Count          AliasProperty Count = Length
Address        Method        System.Object&, mscorlib, Version=2.0.0.0, Cultu
Clone          Method        System.Object Clone()
CopyTo         Method        System.Void CopyTo(array array, int index), Syst
Equals         Method        bool Equals(System.Object obj)
Get            Method        System.Object Get(int )
GetEnumerator  Method        System.Collections.IEnumerator GetEnumerator()
GetHashCode    Method        int GetHashCode()
...
```

Xxxx xxxxxxx xxxxx xxx xxx XxxxxXxxxxx xxxxxxxxx xxxxx xx xxx Xxx$Xxxxxx xxxxxx.
Xxxx xxx xxx xxx XxxxxXxxxxx xxxxxxxxx xx xxx xxx xxxxxxx xx x xxxxxxxxxx$ Xxx$Xxxxxx xxxx xxx xxxxxxx xx xxx xxxxxxxxxx.
Xxxx xxx xxxx x xxxxxxxxxx xx xxxxxxx xx Xxx$Xxxxxx$ Xxx$Xxxxxx xxxx xxx xxxxxxx xx xxxx xxxx xx xxx xxxxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx xxxxxxxx xx xxx xxxxx xxxxxxxx xxx xxxxx xxx xxxxxxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxx xxx $x xxxxxxxx xx xxx Xxx$Xxxxxx xxxxxx.
Xxx$Xxxxxx xxxx xxx xxxxx xx xxxx xxxxxx xx $x xxx xxx xxxxxxx xx xxxx xxxx.
Xx xxxx xxxx$ xx xxxx XxxxxxxXxxxxxxxxx xxxxxxx xxx xxxxx xxx xxxxxxx$ xxxx xx XxxxxxxxXxxxxxxx xxx Xxxxx.

Xxx xxxxx xxxxxxx xxxx xxx XxxxxXxxxxx xxxxxxxxx xx Xxx$Xxxxxx xx xxxxxx xxx $x xxxxxxxx.
Xxx$Xxxxxx xxxx xxx xxxx $Xxxxxx.Xxxxxx$$$$$ xxx xxx xxxxxxx xx xxx xxxxxxxxxx $xx $xxxxx$$ xx XxxxxxxXxxxxxxxxx xxxxxxx$ xxxx xx Xxxxx xxx Xxxxx.

## XXXXXXXXXX

### $Xxxxx
Xxxx xxx xxxxxxxxx xxxxxxx $XXXxxx$ XXXxxxxxx$ XXXxxxxx$ XXXxxxXxxxx$ xxx xxx xxxxxxxx$xxxxxxxxx xxx$ xxx xxx$ xxxxxxx xx xxx xxxxxxx.
Xx xxxxxxx$ Xxx$Xxxxxx xxxx xxxxx xxxxxxxxxx xx xxx xxxxx xxxxx xxxx $Xxxx$ xxx $Xxxxxxx$$ xxx xx xxxx xxx xxxxxxx xxxx.

Xxx xxxxxxxxx xxxx xxxxxxxxx xxx xxxxxxxxxx xxxx xxx xxxxx xxxx xxx xxx xxx Xxxxx xxxxxxxxx$

$$ XXXxxx$  Xxx xxxxxxxx xxxxxxxxxx xx xxx .XXX Xxxxxxxxx xxxxxx xxxxxxx xxxxxxxxx xx xxxxxxxxxx. Xxxxx xxx xxx xxxxxxxxxx xxxxxxx xxx xxx xxxxxx xxxxx xxx xxxxxx xx XXXX.
$$ XXXxxxxxx$ Xxx xxxxxxxxxx xxx xxxxxxx xxxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxx xxxx xxxxxx.
$$ XXXxxxxxxx$ Xxx xxxxxxxxxx xxx xxxxxxx xxxx xxxx xxxxx xx xxx Xxxxx.xx0xxx xxxxx xx xx xxxxx xxx Xxx$Xxxxxx xxxxxx.
$$ XXXxxxxx$ Xxx xxxxxxx xxxx xxxxxxxx xxx xxxx xxxxxx xx x Xxxxxxx XxxxxXxxxx XXXxxxxx xxxxxx.
$$ XXXxxxXxxxx$ X xxxx xx xxxxxx xxxxx xxxx xxxxxxxx xxx xxxxxx$ xx xxxxx xx xxxxxxxxxxx. Xxxx xxxxxxxxxx xxx xxxxxx$ Xxxxxxx XxxxxXxxxx xxxxxxxx xxx xxx xxxxx xx xxx Xxxxxx.xx0xxx xxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxxxxxx xxxxxxxxx $$xxxxxx$. Xx xxxx xxx xxxxxxxxxx xxxxxxxxxx xxx xxx xxxxx xxxx xxxx xx xxxxx.

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
Xxx xxxxxxxxx xxxx xxxxxxxxx xxx xxxxxxxxxx xxxx xxx xxxxx xxxx xxx xxx xxx Xxxxx xxxxxxxxx$

$$ XXXxxx$  Xxx xxxxxxxx xxxxxxxxxx xx xxx .XXX Xxxxxxxxx xxxxxx xxxxxxx xxxxxxxxx xx xxxxxxxxxx. Xxxxx xxx xxx xxxxxxxxxx xxxxxxx xxx xxx xxxxxx xxxxx xxx xxxxxx xx XXXX.
$$ XXXxxxxxx$ Xxx xxxxxxxxxx xxx xxxxxxx xxxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxx xxxx xxxxxx.
$$ XXXxxxxxxx$ Xxx xxxxxxxxxx xxx xxxxxxx xxxx xxxx xxxxx xx xxx Xxxxx.xx0xxx xxxxx xx xx xxxxx xxx Xxx$Xxxxxx xxxxxx.
$$ XXXxxxxx$ Xxx xxxxxxx xxxx xxxxxxxx xxx xxxx xxxxxx xx x Xxxxxxx XxxxxXxxxx XXXxxxxx xxxxxx.
$$ XXXxxxXxxxx$ X xxxx xx xxxxxx xxxxx xxxx xxxxxxxx xxx xxxxxx$ xx xxxxx xx xxxxxxxxxxx. Xxxx xxxxxxxxxx xxx xxxxxx$ Xxxxxxx XxxxxXxxxx xxxxxxxx xxx xxx xxxxx xx xxx Xxxxxx.xx0xxx xxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxxxxxx xxxxxxxxx $$xxxxxx$. Xx xxxx xxx xxxxxxxxxx xxxxxxxxxx xxx xxx xxxxx xxxx xxxx xx xxxxx.

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
Xxx xxxxxxxxx xxxx xxxxxxxxx xxx xxxxxxxxxx xxxx xxx xxxxx xxxx xxx xxx xxx Xxxxx xxxxxxxxx$

$$ XXXxxx$  Xxx xxxxxxxx xxxxxxxxxx xx xxx .XXX Xxxxxxxxx xxxxxx xxxxxxx xxxxxxxxx xx xxxxxxxxxx. Xxxxx xxx xxx xxxxxxxxxx xxxxxxx xxx xxx xxxxxx xxxxx xxx xxxxxx xx XXXX.
$$ XXXxxxxxx$ Xxx xxxxxxxxxx xxx xxxxxxx xxxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxx xxxx xxxxxx.
$$ XXXxxxxxxx$ Xxx xxxxxxxxxx xxx xxxxxxx xxxx xxxx xxxxx xx xxx Xxxxx.xx0xxx xxxxx xx xx xxxxx xxx Xxx$Xxxxxx xxxxxx.
$$ XXXxxxxx$ Xxx xxxxxxx xxxx xxxxxxxx xxx xxxx xxxxxx xx x Xxxxxxx XxxxxXxxxx XXXxxxxx xxxxxx.
$$ XXXxxxXxxxx$ X xxxx xx xxxxxx xxxxx xxxx xxxxxxxx xxx xxxxxx$ xx xxxxx xx xxxxxxxxxxx. Xxxx xxxxxxxxxx xxx xxxxxx$ Xxxxxxx XxxxxXxxxx xxxxxxxx xxx xxx xxxxx xx xxx Xxxxxx.xx0xxx xxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxxxxxx xxxxxxxxx $$xxxxxx$. Xx xxxx xxx xxxxxxxxxx xxxxxxxxxx xxx xxx xxxxx xxxx xxxx xx xxxxx.

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

### $XxxxxXxxxxx
Xxxxxxxxx xxx xxxxxx xxxxx xxxxxxx xxx xxxxxxxxx.

Xxxxx xxx XxxxxXxxxxx xxxxxxxxx xx xxx xxx xxxx xx xxxxxx xx xxxxxx xx Xxx$Xxxxxx.
Xxx xxxxxxxxxxx xxx xx xxxxxxx$

$$ Xxxx xxx xxxx x xxxxxxxxxx xx xxxxxxx xx Xxx$Xxxxxx$ Xxx$Xxxxxx xxxx xxx xxxxxxx xx xxx xxxxxxxxxx xxxxxxx xx xxx xxxxxxxxxx$ xxxx xx xxx xxxxxxxxxx xx xxxx xxxxxx xx xx xxxxx xx xxxxxxx.
$$ Xxxx xxx xxx XxxxxXxxxxx xx xxxxxx x xxxxxxxxxx xx xxxxxxx$ Xxx$Xxxxxx xxxx xxx xxxxxxx xx xxx xxxxxxxxxx$ xxxx xx xxx xxxxxxxxxx xx xxx xxxxx xx xx xxxxx xx xxxxxxx.

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

### $XxxxxxXxxx
Xxxx xxxx xxxxxxx xxxx xxx xxxxxxxxx xxxxxx xxxx.
Xxx xxxxxxx xx Xxx.

Xxx xxxxx xxxxxx xxx xxxx xxxxxxxxx xxx$ XxxxxXxxxxxxx$ Xxx$ XxxxXxxxxx$ XxxxXxxxxxxx$ Xxxxx$ XxxxxxXxx$ Xxxxxx$ Xxxxxxx$ Xxxxxxxxxxxx$ XxxxxxxxxxxxxXxxxxxxx$ Xxxxxxxxxx$ Xxxxxxxx$ XxxxxxxxXxx$ XxxxxxXxxxxx$ xxx XxxxxxXxxxxxxx.

Xxx xxxxxxxxxxx xxxxx xxxxx xxxxxx$ xxx $XXXxxxxxXxxxx Xxxxxxxxxxx$ xx XXXX xx xxxx$$$xxxx.xxxxxxxxx.xxx$xx$xx$xxxxxxx$xxxxxxx$xxxxxxx$xxxxxx.xxxxxxxxxx.xxxxxxxxxx.xxxxxxxxxxxxx$x$xx.00$.xxxx.

Xxx xxx xxxxxxx xxxx xxxxx xxxx xx xxxxxx.
Xx xxx xxxxxxx x xxxxxx xxxx xxxx xxx xxxxxx xxxx xxx xxxx$ Xxxxxxx XxxxxXxxxx xxxxxxx x xxxx xxxxx.

Xx xxx xxxxxxx xxxxx xx xxxxxxx$ xxxx xx xxx xxxxxxxx xxxxxxx$ xxx xxx Xxxx xxxxxxxxx.
Xx xxx xxx xxx XxxxxxXxxx xxxxxxxxx xxxx xxx Xxxxxx xx Xxxx xxxxxxxxxx$ Xxx$Xxxxxx xxxx xxx xxxxxxx xxxx xxxxxx xx xxxx xxxx.

```yaml
Type: PSMemberTypes
Parameter Sets: (All)
Aliases: Type
Accepted values: AliasProperty, CodeProperty, Property, NoteProperty, ScriptProperty, Properties, PropertySet, Method, CodeMethod, ScriptMethod, Methods, ParameterizedProperty, MemberSet, Event, Dynamic, All

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxx
Xxxxxxxxx xxx xxxxx xx xxx xx xxxx xxxxxxxxxx xx xxxxxxx xx xxx xxxxxx.
Xxx$Xxxxxx xxxx xxxx xxx xxxxxxxxx xxxxxxxxxx xxx xxxxxxx.

Xx xxx xxx xxx Xxxx xxxxxxxxx xxxx xxx XxxxxxXxxx$ Xxxx$ xx Xxxxxx xxxxxxxxxx$ Xxx$Xxxxxx xxxx xxxx xxx xxxxxxx xxxx xxxxxxx xxx xxxxxxxx xx xxx xxxxxxxxxx.

Xx xxx x xxxxxx xxxxxx xx xxxx$ xxx xxx Xxxxxx xxxxxxxxx xxxx xxx Xxxx xxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxx
Xxxx xxxx xxx xxxxxx xxxxxxxxxx xxx xxxxxxx xx xxx xxxxxx.

Xxxxxx xxxxxxxxxx xxx xxxxxxx xxx xxxxxxx xx xxx xxxxx xx xxxxxxx$ xxx xx xxx xxxxxxxxxx xxxxxxxx xx xxx xxxxx.

Xx xxx xxx xxx Xxxxxx xxxxxxxxx xxxx xxx Xxxx xxxxxxxxx$ xxx Xxxx xxxxxxxxx xx xxxxxxx.
Xx xxx xxx xxx Xxxxxx xxxxxxxxx xxxx xxx XxxxxxXxxx xxxxxxxxx$ Xxx$Xxxxxx xxxx xxxx xxx xxxxxxx xxxx xxxxxx xx xxxx xxxx.

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
Xxxx xxxx xxxxxxxxxx xxxxx xx xxxxxxx $xxxxxxxxxx xxx xxxxxxx$.
Xxxxxxx xxx xx xxxx xx xxx xxxxxx.
Xxx xxxxxxx xx $Xxxxxxx$ Xxxxxxxx$.

Xxxxx xxxxxx xxx$

$$ Xxxx$  Xxxx xxxx xxx xxxxxxxx xxxxxxxxxx xxx xxxxxxx xx xxx .XXX Xxxxxxxxx xxxxxx $xxxxxxx xxxxxxxxx xx xxxxxxxxxx$.
$$ Xxxxxxx$  Xxxx xxxx xxx xxxxxxxxxx xxx xxxxxxx xxxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxx xxxx xxxxxx.
$$ Xxxxxxxx$ Xxxx xxxx xxx xxxxxxxxxx xxx xxxxxxx xxxx xxxx xxxxx xx xxx Xxxxx.xx0xxx xxxxx xx xx xxxxx xxx Xxx$Xxxxxx xxxxxx.
$$ Xxx$ Xxxx xxx xxxxxxx xx xxx Xxxx$ Xxxxxxx$ xxx Xxxxxxxx xxxxx.

Xxx Xxxx xxxxxxxxx xxxxxxxxxx xxx xxxxxxx xxxxxxxxx$ xxx xxxx xxx xxxxxxx xx xxxxx xxxxxxx.

Xx xxx xxxxxxxxxx xxxxxx xxxxx$ xxxx xx xxxxxx xxxxxxxxxx$ xxx xxx XxxxxxXxxx xxxxxxxxx.
Xx xxx xxx xxx XxxxxxXxxx xxx Xxxx xxxxxxxxxx xx xxx xxxx xxxxxxx$ Xxx$Xxxxxx xxxx xxx xxxxxxx xxxx xxxxxx xx xxxx xxxx.
Xx xxx xxx xxx Xxxxxx xxx Xxxx xxxxxxxxxx xx xxx xxxx xxxxxxx$ xxx Xxxx xxxxxxxxx xx xxxxxxx.

```yaml
Type: PSMemberViewTypes
Parameter Sets: (All)
Aliases: 
Accepted values: Extended, Adapted, Base, All

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxx
Xxx xxx xxxx xxx xxxxxx xx Xxx$Xxxxxx

## XXXXXXX

### Xxxxxxxxx.XxxxxXxxxx.Xxxxxxxx.XxxxxxXxxxxxxxxx
Xxx$Xxxxxx xxxxxxx xx xxxxxx xxx xxxx xxxxxxxx xx xxxxxx xxxx xxx xxxx.

## XXXXX
Xxx xxx xxx xxxxxxxxxxx xxxxx x xxxxxxxxxx xxxxxx xxxxxx xx xxxxx xxx XxxxxXxxxxx xxxxxxxxx xx xx xxxxxx xxx xxxxxx$ xxxxxxxx xx x xxxxx$ xx Xxx$Xxxxxx.

Xxx xxx xxx xxx $xxxx xxxxxxxxx xxxxxxxx xx xxxxxx xxxxxx xxxx xxxxxx xxx xxxxxx xx xxx xxxxxxxxxx xxx xxxxxxx.
Xxx $xxxx xxxxxxxx xxxxxx xx xxx xxxxxxxx xx xxx xxxxxx xx xxxxx xxx xxxxxxxxxx xxx xxxxxxx xxx xxxxx xxxxx.
Xxx xxxx xxxxxxxxxxx xxxxx xxx $xxxx xxxxxxxx$ xxx xxxxx$Xxxxxxxxx$Xxxxxxxxx.

## XXXXXXX XXXXX

[Xxx$Xxxxxx]()

[Xxx$Xxxxxxx]()

[Xxx$Xxxx]()

[Xxx$XXXxxxx]()

[xxxxx$Xxxxxxxxx$Xxxxxxxxx]()

[xxxxx$Xxxxxxxxxx]()

[xxxxx$Xxxxxxx]()

[xxxxx$Xxxxxxx]()

