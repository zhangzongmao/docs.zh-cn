---
title: '&#39;每个&#39;类型&#39; &lt;typename&gt; &#39;不明确，因为该类型实现多个实例化&#39;如 (Of T)&#39;'
ms.date: 07/20/2015
f1_keywords:
- vbc32096
- bc32096
helpviewer_keywords:
- BC32096
ms.assetid: ed20d09c-913f-482e-89f8-c0a596c3ec24
ms.openlocfilehash: 8c48a7134eb8da83fb418b9aa91d55dcbe8e8bcb
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="39for-each39-on-type-39lttypenamegt39-is-ambiguous-because-the-type-implements-multiple-instantiations-of-39systemcollectionsgenericienumerableof-t39"></a>&#39;每个&#39;类型&#39; &lt;typename&gt; &#39;不明确，因为该类型实现多个实例化&#39;如 (Of T)&#39;
A`For Each`语句指定具有多个迭代器变量<xref:System.Collections.IEnumerable.GetEnumerator%2A>方法。  
  
 迭代器变量必须实现的类型为<xref:System.Collections.IEnumerable?displayProperty=nameWithType>或<xref:System.Collections.Generic.IEnumerable%601?displayProperty=nameWithType>接口之一`Collections`命名空间中的， [!INCLUDE[dnprdnshort](~/includes/dnprdnshort-md.md)]。 它有可能实现多个构造的泛型接口，使用每个构造的不同的类型自变量的类。 如果执行此类用于迭代器变量，该变量具有多个<xref:System.Collections.IEnumerable.GetEnumerator%2A>方法。 在这种情况下，Visual Basic 不能选择要调用的方法。  
  
 **错误 ID:** BC32096  
  
## <a name="to-correct-this-error"></a>更正此错误  
  
-   使用[DirectCast 运算符](../../../visual-basic/language-reference/operators/directcast-operator.md)或[TryCast 运算符](../../../visual-basic/language-reference/operators/trycast-operator.md)与接口定义的迭代器变量类型转换<xref:System.Collections.IEnumerable.GetEnumerator%2A>你想要使用的方法。  
  
## <a name="see-also"></a>请参阅  
 [For Each...Next 语句](../../../visual-basic/language-reference/statements/for-each-next-statement.md)  
 [接口](../../../visual-basic/programming-guide/language-features/interfaces/index.md)
