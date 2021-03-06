---
title: reset
description: "Windows Commands topic for **** - "
ms.custom: na
ms.prod: windows-server-threshold
ms.reviewer: na
ms.suite: na
ms.technology: manage-windows-commands
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: afbdab44-199c-4e11-884f-e96804965c21
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/12/2016
---
# reset

>Applies To: Windows Server 2016, Windows Server 2012 R2, Windows Server 2012

resets diskshadow.exe to the default state. **reset** is especially useful in separating compound diskshadow operations such as **create**, **import**, **backup**, or **restore**.  
  
## Syntax  
  
```  
reset  
```  
  
## remarks  
  
-   When you use the **reset** command, you lose state from commands such as **add**, **set**, **load**, or **writer**. **reset** also releases IVssBackupcomponent interfaces and loses non\-persistent shadow copies.  
  
#### additional references  
[Command-Line Syntax Key](command-line-syntax-key.md)  
  

