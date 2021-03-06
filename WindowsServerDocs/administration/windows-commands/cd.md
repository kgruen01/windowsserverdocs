---
title: cd
description: "Windows Commands topic for **** - "
ms.custom: na
ms.prod: windows-server-threshold
ms.reviewer: na
ms.suite: na
ms.technology: manage-windows-commands
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 932d9cc1-3dff-40da-835c-1cb0894874f1
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/12/2016
---
# cd

>Applies To: Windows Server 2016, Windows Server 2012 R2, Windows Server 2012

Displays the name of or changes the current directory. If used with only a drive letter (for example, `cd C:`), **cd** displays the names of the current directory in the specified drive. If used without parameters, **cd** displays the current drive and directory.  
> [!NOTE]  
> This command is the same as the **chdir** command.  
for examples of how to use this command, see [Examples](#BKMK_examples).  
## Syntax  
```  
cd [/d] [<Drive>:][<path>]  
cd [..]  
chdir [/d] [<Drive>:][<path>]  
chdir [..]  
```  
## Parameters  
|Parameter|Description|  
|-------|--------|  
|/d|changes the current drive as well as the current directory for a drive.|  
|<Drive>:|Specifies the drive to display or change (if different from the current drive).|  
|<path>|Specifies the path to the directory that you want to display or change.|  
|[..]|Specifies that you want to change to the parent folder.|  
|/?|Displays help at the command prompt.|  
## remarks  
if command extensions are enabled, the following conditions apply to the **cd** command:  
-   The current directory string is converted to use the same case as the names on the disk. For example, `cd C:\TEMP` would set the current directory to C:\Temp if that is the case on the disk.  
-   Spaces are not treated as delimiters, so *path* can contain spaces without enclosing quotation marks. For example:  
    ```  
    cd username\programs\start menu  
    ```  
    is the same as:  
    ```  
    cd "username\programs\start menu"  
    ```  
    The quotation marks are required, however, if extensions are disabled.  
To disable command extensions, type:  
```  
cmd /e:off  
```  
## <a name="BKMK_examples"></a>Examples  
The root directory is the top of the directory hierarchy for a drive. To return to the root directory, type:  
```  
cd\  
```  
To change the default directory on a drive that is different from the one you are on, type:  
```  
cd [<Drive>:\[<directory>]]  
```  
To verify the change to the directory, type:  
```  
cd [<Drive>:]  
```  
#### additional references  
[Command-Line Syntax Key](command-line-syntax-key.md)  
