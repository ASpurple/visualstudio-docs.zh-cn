---
title: "IActiveScriptParseProcedureOld::ParseProcedureText | Microsoft Docs"
ms.custom: ""
ms.date: "01/18/2017"
ms.prod: "windows-script-interfaces"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "reference"
apiname: IActiveScriptParseProcedureOld.ParseProcedureText
apilocation: jscript.dll
helpviewer_keywords: 
  - "IActiveScriptParseProcedureOld::ParseProcedureText"
ms.assetid: 21a21313-35ce-432d-b9a6-7999065f19ac
caps.latest.revision: 8
author: "mikejo5000"
ms.author: "mikejo"
manager: "ghogen"
caps.handback.revision: 8
---
# IActiveScriptParseProcedureOld::ParseProcedureText
分析特定代码程序并添加匿名程序添加到命名空间。  
  
## 语法  
  
```  
HRESULT ParseProcedureText(  
   LPCOLESTR    pstrCode,  
   LPCOLESTR    pstrFormalParams,  
   LPCOLESTR    pstrItemName,  
   IUnknown*    punkContext,  
   LPCOLESTR    pstrDelimiter,  
   DWORD_PTR    dwSourceContextCookie,  
   ULONG        ulStartingLineNumber,  
   DWORD        dwFlags,  
   IDispatch**  ppdisp  
);  
```  
  
#### 参数  
 `pstrCode`  
 \[in\]计算的程序文本。  此字符串的解释取决于这种脚本语言。  
  
 `pstrFormalParams`  
 \[in\]形参名称程序。  必须分隔参数名后面加上脚本引擎的相应分隔符。  不应括在括号名称。  
  
 `pstrItemName`  
 \[in\]提供上下文此过程将计算指定项目的名称。  如果此参数是 `NULL`，代码对脚本引擎的全局上下文进行计算。  
  
 `punkContext`  
 \[out\]上下文对象。  此对象保留了用于调试环境，此上下文可能由调试器提供表示有效的运行时上下文。  如果此参数是 `NULL`，引擎使用 `pstrItemName` 标识上下文。  
  
 `pstrDelimiter`  
 \[in\]关闭程序分隔符。  当 `pstrCode` 从文本时流进行分析，宿主通常使用一个分隔符，例如两个引号\("\)，检测过程的结尾。  此参数指定例如使用的主机，允许脚本引擎提供某些条件，原始预处理的分隔符\(，一个单引号\[ \] “将两个单引号用作分隔符\)。  \(和\)，如果脚本引擎正确如何使用此信息取决于脚本引擎。  如果宿主不使用一个分隔符以指示该程序，结束时将此参数设置为 `NULL`。  
  
 `dwSourceContextCookie`  
 \[in\]使用了用于调试目的应用程序定义的值。  
  
 `ulStartingLineNumber`  
 \[in\]用于指定在的从零开始的值哪行分析将启动。  
  
 `dwFlags`  
 \[in\]标志与该程序。  可以是这些值的组合。  
  
|常量|值|含义|  
|--------|-------|--------|  
|SCRIPTPROC\_ISEXPRESSION|0x00000020|指示在 `pstrCode` 的代码是表示该过程的返回值的表达式。|  
|SCRIPTPROC\_IMPLICIT\_THIS|0x00000100|指示 `this` 指针包括在该过程范围内。|  
|SCRIPTPROC\_IMPLICIT\_PARENTS|0x00000200|指示 `this` 指针的父包括在该过程范围内。|  
  
 `ppdisp`  
 \[in\]返回默认方法与方法分析的过程计划包装。  
  
## 返回值  
 该方法返回 `HRESULT`。  可能的值包括，但是，并不限于，这些下表中。  
  
|值|说明|  
|-------|--------|  
|`S_OK`|方法成功。|  
|`E_INVALIDARG`|参数无效。|  
|`E_POINTER`|无效指针指定了。|  
|`E_NOTIMPL`|此方法不受支持。  脚本引擎不支持程序的运行时向命名空间。|  
|`E_UNEXPECTED`|调用非预期\(例如，脚本引擎在未初始化或已关闭状态\)。|  
|`OLESCRIPT_E_SYNTAX`|一个未指定的语法错误在过程生成的。|  
|`S_FALSE`|脚本引擎不支持计划对象；`ppdisp` 参数设置为 `NULL`。|  
  
## 备注  
 脚本代码不会计算在调用;相反，该程序被编译到方法在其可以由该脚本调用后立即 `ppdisp`。  
  
 此接口是否决了 `IActiveScriptParseProcedure` 接口。  `IActiveScriptParseProcedure::ParseProcedureText` 方法类似于方法，但是，它允许过程名称指定。  在任何情况下，应使用 `IActiveScriptParseProcedure::ParseProcedureText`。  
  
## 请参阅  
 [IActiveScriptParseProcedureOld 接口](../../winscript/reference/iactivescriptparseprocedureold-interface.md)   
 [IActiveScriptParseProcedure::ParseProcedureText](../../winscript/reference/iactivescriptparseprocedure-parseproceduretext.md)