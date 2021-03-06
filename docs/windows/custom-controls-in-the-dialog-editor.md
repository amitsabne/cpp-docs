---
title: "Custom Controls in the Dialog Editor | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-cpp"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "Custom Control"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "controls [C++], templates"
  - "custom controls [Visual Studio], dialog boxes"
  - "custom controls [Visual Studio]"
  - "dialog box controls, custom (user) controls"
  - "Dialog editor, custom controls"
ms.assetid: f494b314-4000-4bbe-bbd0-4b18fb71ede1
caps.latest.revision: 9
author: "mikeblome"
ms.author: "mblome"
manager: "ghogen"
translation.priority.ht: 
  - "cs-cz"
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "pl-pl"
  - "pt-br"
  - "ru-ru"
  - "tr-tr"
  - "zh-cn"
  - "zh-tw"
---
# Custom Controls in the Dialog Editor
The Dialog editor lets you use existing "custom" or "user" controls in a dialog box template.  
  
> [!NOTE]
>  Custom controls in this sense are not to be confused with ActiveX controls. ActiveX controls were sometimes called OLE custom controls. Also, don't confuse these controls with the owner-drawn controls in Windows.  
  
 This functionality is intended to let you use controls other than those supplied by Windows. At run time, the control is associated with a window class (not the same as a C++ class). A more common way to accomplish the same task is to install any control, such as a static control, in your dialog box. Then at run time, in the [OnInitDialog](../mfc/reference/cdialog-class.md#oninitdialog) function, remove that control and replace it with your own custom control.  
  
 This is an old technique. Today you are advised in most cases to write an ActiveX control or subclass a Windows common control.  
  
 For these custom controls, you are limited to:  
  
-   Setting the location in the dialog box.  
  
-   Typing a caption.  
  
-   Identifying the name of the control's Windows class (your application code must register the control by this name).  
  
-   Typing a 32-bit hexadecimal value that sets the control's style.  
  
-   Setting the extended style.  
  
 For information on adding resources to managed projects, please see [Resources in Desktop Apps](https://msdn.microsoft.com/library/f45fce5x.aspx) in the *.NET Framework Developer's Guide.* For information on manually adding resource files to managed projects, accessing resources, displaying static resources, and assigning resource strings to properties, see [Creating Resource Files for Desktop Apps](https://msdn.microsoft.com/library/xbx3z216.aspx). For information on globalization and localization of resources in managed apps, see [Globalizing and Localizing .NET Framework Applications](https://msdn.microsoft.com/library/h6270d0z.aspx).  
  
## Requirements  
 Win32  
  
## See Also  
 [Controls in Dialog Boxes](../windows/controls-in-dialog-boxes.md)   
 [Controls](../mfc/controls-mfc.md)

