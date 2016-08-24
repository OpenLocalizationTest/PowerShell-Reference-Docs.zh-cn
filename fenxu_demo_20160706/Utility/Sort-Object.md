---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294017
schema: 2.0.0
---

# Xxxx$Xxxxxx
## XXXXXXXX
Xxxxx xxxxxxx xx xxxxxxxx xxxxxx.

## XXXXXX

```
Sort-Object [-Descending] [-Unique] [-InputObject <PSObject>] [[-Property] <Object[]>] [-Culture <String>]
 [-CaseSensitive] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxx$Xxxxxx xxxxxx xxxxx xxxxxxx xx xxxxxxxxx xx xxxxxxxxxx xxxxx xxxxx xx xxx xxxxxx xx xxxxxxxxxx xx xxx xxxxxx.

Xxx xxx xxxxxxx x xxxxxx xxxxxxxx xx xxxxxxxx xxxxxxxxxx $xxx x xxxxx$xxx xxxx$$ xxx xxx xxx xxxxxx x xxxx$xxxxxxxxx xx xxxx$xxxxxxxxxxx xxxx.
Xxx xxx xxxx xxxxxx Xxxx$Xxxxxx xx xxxxxxx xxxx xxx xxxxxxx xxxx x xxxxxx xxxxx xxx x xxxxxxxxxx xxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-childitem | sort-object

Mode                LastWriteTime     Length Name
----                -------------     ------ ----
-a---         9/13/2005   4:24 PM          0 0
-a---          9/6/2005   4:19 PM         12 a.csv
-a---         9/21/2005   3:49 PM        529 a.Ps
-a---         8/22/2005   4:14 PM         22 a.pl
-a---         9/27/2005  10:33 AM         24 a.txt
-a---         9/15/2005  10:31 AM        398 a.vbs
-a---         7/21/2005  12:39 PM      37066 a.xml
-a---         8/28/2005  11:30 PM       5412 a.xslt
-a---        10/25/2005   1:59 PM        125 AdamTravel.txt
-a---         7/21/2005   9:49 AM         59 add2Num.Ps
-a---         8/29/2005   5:42 PM       7111 add-content.xml
-a---         9/21/2005  12:46 PM       8771 aliens.Ps
-a---         8/10/2005   2:10 PM        798 array.xml
-a---          8/4/2004   5:00 AM        110 AUTORUN.INF
-a---          9/6/2005   4:20 PM        245 b.csv
...
```

Xxxx xxxxxxx xxxxx xxx xxxxxxxxxxxxxx xxx xxxxx xx xxx xxxxxxx xxxxxxxxx.
Xxxxxxx xx xxxxxxxxxx xxx xxxxxxxxx$ xxx xxxxx xxx xxxxxxxxxxx xxx xxxxxx xx xxxxxxxxx xxxxxxxxxxxx xxxxx xx xxxxx xxxxxxx xxxx xxxxxxxx$ Xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-childitem | sort-object -property length

Mode                LastWriteTime     Length Name
----                -------------     ------ ----
-a---         12/3/2006   5:35 PM          2 pref.txt
-a---          9/6/2006   3:33 PM         15 count.txt
-a---         7/26/2006  10:01 AM         30 filenoext
-a---         8/18/2006   9:02 AM         52 temp.ps1
-a---         8/18/2006   9:02 AM         52 temp.msh
-a---          9/6/2006   3:33 PM         56 fivewords.txt
-a---         7/26/2006   9:28 AM         80 date.csv
-a---         7/29/2006   7:15 PM         84 test2.txt
-a---         7/29/2006   7:15 PM         84 test.ps1
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxx xx xxx xxxxxxx xxxxxxxxx xx xxxxxxxxx xxxxx xx xxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process | sort-object -property WS | select-object -last 5

Handles  NPM(K)    PM(K)      WS(K) VM(M)   CPU(s)     Id ProcessName
-------  ------    -----      ----- -----   ------     -- -----------
1105      25    44236      18932   197    93.81      2032 iexplore
2526      66    37668      36836   221   393.27       868 svchost
974       19    22844      45928   371    88.39      3952 WINWORD
1371      22    42192      61872   323    75.75      1584 INFOPATH
2145      58    93088      70680   619   396.69      3908 OUTLOOK
```

Xxxx xxxxxxx xxxxxxxx xxx xxxx xxxxxxxxx xx xxx xxxxxxxx xxxx xxx xxxxxxxx xxxxxx xxx xxxxx xx xxx xxxx xx xxxxx xxxxxxx xxxx.

Xxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx x xxxx xx xxxxxxxxx.
Xx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxx xx xxx Xxxx$Xxxxxx xxxxxx$ xxxxx xxxxx xxx xxxxxxx xx xxxxxxx$xxx xxxxx.

Xxxxxxx xxxxxxxx xxxxxxxx xxxxx xxx xxxxxxx xx xxx Xxxxxx$Xxxxxx$ xxxxx xxxxxxxx xxxx xxx xxxx xxxx xxxxx xx xxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-history | sort-object -descending

Id CommandLine
-- -----------
51 get-history | sort -descending
50 get-history | sort -descending
49 get-history | sort -descending
48 get-history | sort -descending
47 get-history | sort -descending
46 get-history | sort -descending
45 get-history | sort -descending
44 cd $pshome
43 get-childitem | sort-object
42 gci *.txt
```

Xxxx xxxxxxx xxxxx XxxxxxxXxxx xxxxxxx xxxxx xxx Xx xxxxxxxx xx xxx xxxxxxx xxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-service | sort-object -property @{Expression="Status";Descending=$true}, @{Expression="DisplayName";Descending=$false}

Status   Name               DisplayName
------   ----               -----------
Running  ALG                Application Layer Gateway Service
Running  Ati HotKey Poller  Ati HotKey Poller
Running  wuauserv           Automatic Updates
Running  BITS               Background Intelligent Transfer Ser...
Running  Client for NFS     Client for NFS
...
Stopped  clr_optimizatio... .NET Runtime Optimization Service v...
Stopped  Alerter            Alerter
Stopped  AppMgmt            Application Management
Stopped  aspnet_state       ASP.NET State Service
Stopped  ATI Smart          ATI Smart
Stopped  ClipSrv            ClipBook
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxxxx xx xxx xxxxxxxx xx xxxxxxxxxx Xxxxxx xxxxx xxx xxxxxxxxx XxxxxxxXxxx xxxxx.

Xxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxx xxxxxxxx xx xxx xxxxxxxx.
Xx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxxxxxxx xx xxx Xxxx$Xxxxxx xxxxxx.

Xx xxxx xxx xxxxxxxx xx xxxxxxxxx xxxxx xxx xxxxxxx xxxxxxxx xx xxxxxxxxxx xxxxx$ xxx xxxxxxx xxxx x xxxx xxxxx xxx xxx xxxxx xx xxx Xxxxxxxx xxxxxxxxx.
Xxx xxxx xxxxx xxxx xx Xxxxxxxxxx xxx xx xxxxxxx xxx xxxxxxxx xxxx xxx xx Xxxxxxxxx xx Xxxxxxxxxx xxx xx xxxxxxx xxx xxxx xxxxx.

Xxx xxxxxxxxx xxxxxxx$ xxxxx xxxxx xxx Xxxxxx xxxxxx xx xxxxxxxxxx xxxxx$ xxxxx xxxxxxxxxx xxxx x Xxxxxx xxxxx xx $Xxxxxxx$ xxxxxx xxxxx xxxx x Xxxxxx xxxxx xx $Xxxxxxx$.
Xxxx xxxxxx xx xxxxxxxxx xxxxx$ $Xxxxxxx$ xxxxxxx xxxxxx $Xxxxxxx$$ xxxxxxx Xxxxxx xx xx xxxxxxxxxx xxxxxxxx xx xxxxx xxx xxxxx xx $Xxxxxxx$ $0$ xx xxxx xxxx xxx xxxxx xx $Xxxxxxx$ $0$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-childitem *.txt | sort-object -property @{Expression={$_.LastWriteTime - $_.CreationTime}; Ascending=$false} | Format-Table LastWriteTime, CreationTime

LastWriteTime                           CreationTime
-------------                           ------------
2/21/2006 10:22:20 AM                   10/3/2005 4:19:40 PM
2/27/2006 8:14:24 AM                    2/23/2006 10:41:08 PM
2/24/2006 1:26:19 PM                    2/23/2006 11:23:36 PM
1/5/2006 12:01:35 PM                    1/5/2006 11:35:30 AM
2/24/2006 9:25:40 AM                    2/24/2006 9:22:24 AM
2/24/2006 9:40:01 AM                    2/24/2006 9:39:41 AM
2/21/2006 10:21:30 AM                   2/21/2006 10:21:30 AM
```

Xxxx xxxxxxx xxxxx xxxx xxxxx xx xxxxxxxxxx xxxxx xx xxx xxxx xxxx xxxxxxx XxxxxxxxXxxx xxx XxxxXxxxxXxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-content servers.txt

localhost
test01
server01
server02
localhost
server01

PS C:\>get-content servers.txt | sort-object -unique

localhost
server01
server02
test01
```

Xxxxx xxxxxxxx xxxx xxx xxxxx xx xxxxxxx xx x xxxx xxxx.
Xxx xxxxxx xxxxxxx xxxx xxx Xxxx$Xxxxxx xxxxxx xxxx xxx Xxxxxx xxxxxxxxx xx xxxxxx x xxxxxx xxxx xxxxxxx xxxxxxxxxx.

## XXXXXXXXXX

### $XxxxXxxxxxxxx
Xxxxxxxxx xxxx xxx xxxx xxxxxx xx xxxx xxxxxxxxx.
Xx xxxxxxx$ xxxxxxx xx xxx xxxx xxxxxxxxx.

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

### $Xxxxxxx
Xxxxxxxxx xxx xxxxxxxx xxxxxxxxxxxxx xx xxx xxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxxxxx
Xxxxx xxx xxxxxxx xx xxxxxxxxxx xxxxx.
Xxx xxxxxxx xx xxxxxxxxx xxxxx.

Xxx Xxxxxxxxxx xxxxxxxxx xxxxxxx xx xxx xxxxxxxxxx.
Xx xxxx xx xxxx xxxxxxxxxx xx

xxxxxxxxx xxxxx xxx xxxxxx xx xxxxxxxxxx xxxxx$ xxx xxxx xxxxxxx xxxxx xxxxxxxx xxxxxx xx xxxxx x xxxx xxxxx.
Xxx xxxxxxx$ xxx xxx xxxxxxxx.

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

### $XxxxxXxxxxx
Xxxxxxxxx xxx xxxxxxx xx xx xxxxxx.

Xxxx xxx xxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxxxx x xxxxxxxxxx xx xxxxx$ Xxxx$Xxxxxx xxxxxxxx xxx xxxxxx xxxx xxxxxxxxxx xxx xxxxxxxxxx.
Xxxxxxx xxx xxxxxx xxxxxx xx xxxxxx$ Xxxx$Xxxxxx xxxxxxx xxx xxxxxx xxxxxxxxxx xxxxxxxxx.

Xx xxxx xxxxxxx$ xxxx xxxx xx Xxxx$Xxxxxx.

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

### $Xxxxxxxx
Xxxxxxxxx xxx xxxxxxxxxx xx xxx xxxx xxxxxxx.
Xxxxxxx xxx xxxxxx xxxxx xx xxx xxxxxx xx xxxxx xxxxxxxxxx.
Xxxxx xxx xxxxx xx xxx xxxxxxxxxx.
Xxxxxxxxx xxx xxxxxxxxx.

Xx xxx xxxxxxx xxxxxxxx xxxxxxxxxx$ xxx xxxxxxx xxx xxxxx xxxxxx xx xxx xxxxx xxxxxxxx.
Xx xxxx xxxx xxx xxxxxx xxx xxx xxxx xxxxx xxx xxx xxxxx xxxxxxxx$ xxxxx xxxxxxx xxx xxxxxx xx xxx xxxxxx xxxxxxxx.
Xxxx xxxxxxx xxxxxxxxx xxxxx xxxxx xxx xx xxxx xxxxxxxxx xxxxxxxxxx xx xx xxxxxx xx xxxxxxx.

Xx xxx xx xxx xxxxxxx xxxxxxxxxx$ xxx xxxxxx xxxxx xxxxx xx xxxxxxx xxxxxxxxxx xxx xxx xxxxxx xxxx.

Xxx xxxxx xx xxx Xxxxxxxx xxxxxxxxx xxx xx x xxxxxxxxxx xxxxxxxx.
Xx xxxxxx x xxxxxxxxxx$ xxxxxxxx$ xxx x xxxx xxxxx.
Xxxxx xxxx xxx$

$$ Xxxxxxxxxx $$xxxxxx$$ xx $$xxxxxx xxxxx$$$$$ Xxxxxxxxx $$Xxxxxxx$$$$$ Xxxxxxxxxx $$Xxxxxxx\>

```yaml
Type: Object[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxx
Xxxxxxxxxx xxxxxxxxxx xxx xxxxxxx xxxx xxx xxxxxx xxxxxxx xx xxx xxxxxxxxxx.
Xxx xxx xxx xxxx xxxxxxxxx xxxxxxx xx xxxxx xxx Xxx$Xxxxxx xxxxxx.

Xxxx xxxxxxxxx xx xxxx$xxxxxxxxxxx.
Xx x xxxxxx$ xxxxxxx xxxx xxxxxx xxxx xx xxxxxxxxx xxxxxx xxx xxxxxxxxxx xx xx xxx xxxx $xxx xxxxxx$.

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

## XXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxx
Xxx xxx xxxx xxx xxxxxxx xx xx xxxxxx xx Xxxx$Xxxxxx.

## XXXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxx
Xxxx$Xxxxxx xxxxxxx xxx xxxxxx xxxxxxx.

## XXXXX
Xxxx$Xxxxxx xxxxx xxxxxxx xxxxx xx xxx xxxxxxxxxx xxxx xxx xxxxxxx xx xxx xxxxxxx xxxx xxxxxxxxxx xxx xxxxxxx xx xxxx xxxx.

Xx xx xxxxxx xxxx xxx xxxx xxx xx xxx xxxxxxxxx xxxxxxxxxx$ xxx xxxxxxxx xxxxx xxx xxxx xxxxxx xx xxxxxxxxxxx xx xxx xxxxxx xx XXXX xxx xx xxxxxx xx xxx xxx xx xxx xxxx xxxxx.

Xxxx xxxxxxx xxxxxxx$ Xxxx$Xxxxxx xxxx xxx Xxxxxxx xxxxxx xxx xxxx xxxxxxxx.
Xx x xxxxxxxx xxxx xxx xxxxxxxxx XXxxxxxxxxx$ xxx xxxxxx xxxxxxxx xxx xxxxxxxx xxxxx xx x xxxxxx xxx xxxx xxx Xxxxxxx xxxxxx xxx Xxxxxx.Xxxxxx

Xxx Xxxx$Xxxxxx xxxxxx xxxxx xxxxxxx xx xxxxxxxxx xx xxxxxxxxxx xxxxx xxxxx xx xxx xxxxxx xx xxxxxxxxxx xx xxx xxxxxx.

Xx xxx xxxx xx x xxxxxxxx xxxxx xxxxx xx xx xxxxxxxxxxx$ Xxxx$Xxxxxx xxxxx xxx xxxxxxxxxxx xxxxxx xx xxxxxxx xxxxx$ xx xxxx xxx xxxx xxx xxxxxxxxxxx xxxxxx xxxxx.
Xxx xxxxxxx$ xx xxx xxxx xxxxxxxx xx xxxxxx$ xxxxxxxx xxxx x xxxxxx xx $Xxxxxxx$ xxxxxx xxxxxx xxxxxxxx xxxx x xxxxxx xx $Xxxxxxx$$ xxxxxxx xxx xxxxx xx Xxxxxx xx x XxxxxxxXxxxxxxxxxXxxxxx xxxxxxxxxxx$ xx xxxxx $Xxxxxxx$ xxx x xxxxx xx 0 xxx $Xxxxxxx$ xxx x xxxxx xx 0.

## XXXXXXX XXXXX

[Xxxxx$Xxxxxx]()

