---
title: Take While 子句 (Visual Basic)
ms.date: 07/20/2015
f1_keywords:
- vb.QueryTakeWhile
helpviewer_keywords:
- queries [Visual Basic], Take While
- Take While clause [Visual Basic]
- Take While statement [Visual Basic]
ms.assetid: db8f9f2f-fc9f-4a6c-b0b8-1bf048147e11
ms.openlocfilehash: 7e0a6bd77ca2594e9d74e669fcd9cddf91ee1cad
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="take-while-clause-visual-basic"></a>Take While 子句 (Visual Basic)
包括集合中指定条件为 `true` 的任何元素，并绕过剩余元素。  
  
## <a name="syntax"></a>语法  
  
```  
Take While expression  
```  
  
## <a name="parts"></a>部件  
  
|术语|定义|  
|---|---|  
|`expression`|必须的。 一个表示要测试的元素的条件的表达式。 该表达式必须返回`Boolean`值或等效的功能，如`Integer`作为计算`Boolean`。|  
  
## <a name="remarks"></a>备注  
 `Take While`子句之前提供包括从查询结果的开始元素`expression`返回`false`。 后`expression`返回`false`，查询将跳过所有剩余元素。 `expression`对于剩余的结果，将忽略。  
  
 `Take While`子句不同于`Where`中的子句`Where`子句可用来进行包括从查询满足特定条件的所有元素。 `Take While`子句之前未满足的条件的第一个时间仅包括元素。 `Take While`子句在你正在使用排序的查询结果时最有用。  
  
## <a name="example"></a>示例  
 下面的代码示例使用`Take While`子句来检索结果，直到找到第一个客户没有任何订单。  
  
 [!code-vb[VbSimpleQuerySamples#2](../../../visual-basic/language-reference/queries/codesnippet/VisualBasic/take-while-clause_1.vb)]  
  
## <a name="see-also"></a>请参阅  
 [Visual Basic 中的 LINQ 简介](../../../visual-basic/programming-guide/language-features/linq/introduction-to-linq.md)  
 [查询](../../../visual-basic/language-reference/queries/queries.md)  
 [Select 子句](../../../visual-basic/language-reference/queries/select-clause.md)  
 [From 子句](../../../visual-basic/language-reference/queries/from-clause.md)  
 [Take 子句](../../../visual-basic/language-reference/queries/take-clause.md)  
 [Skip While 子句](../../../visual-basic/language-reference/queries/skip-while-clause.md)  
 [Where 子句](../../../visual-basic/language-reference/queries/where-clause.md)
