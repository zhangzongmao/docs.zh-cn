---
title: as（C# 参考）
ms.date: 07/20/2015
f1_keywords:
- as_CSharpKeyword
- as
helpviewer_keywords:
- type conversion [C#], as keyword
- as keyword [C#]
ms.assetid: a9be126b-cbf4-4990-a70d-d0e1983cad0e
ms.openlocfilehash: 6ea5346119259d70ac1a42f3f72a8b2746b8f536
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="as-c-reference"></a>as（C# 参考）
可以使用 `as` 运算符在符合的引用类型或[可以为 null 的类型](../../../csharp/programming-guide/nullable-types/index.md)之间执行某些类型的转换。 以下代码显示一个示例。  
  
 [!code-csharp[csrefKeywordsOperator#1](../../../csharp/language-reference/keywords/codesnippet/CSharp/as_1.cs)]  
  
## <a name="remarks"></a>备注  
 `as` 运算符类似于转换运算。 但是，如果无法进行转换，则 `as` 会返回 `null`，而不是引发异常。 请看下面的示例：  
  
```  
expression as type  
```  
  
 该代码等效于以下表达式，但 `expression` 变量仅进行一次计算。  
  
```  
expression is type ? (type)expression : (type)null  
```  
  
 请注意，`as` 运算符仅执行引用转换、可以为 null 的转换和装箱转换。 `as` 运算符无法执行其他转换，例如用户定义的转换，应使用转换表达式执行此转换。  
  
## <a name="example"></a>示例  
 [!code-csharp[csrefKeywordsOperator#2](../../../csharp/language-reference/keywords/codesnippet/CSharp/as_2.cs)]  
  
## <a name="c-language-specification"></a>C# 语言规范  
 [!INCLUDE[CSharplangspec](~/includes/csharplangspec-md.md)]  
  
## <a name="see-also"></a>请参阅  
 [C# 参考](../../../csharp/language-reference/index.md)  
 [C# 编程指南](../../../csharp/programming-guide/index.md)  
 [C# 关键字](../../../csharp/language-reference/keywords/index.md)  
 [is](../../../csharp/language-reference/keywords/is.md)  
 [?: 运算符](../../../csharp/language-reference/operators/conditional-operator.md)  
 [运算符关键字](../../../csharp/language-reference/keywords/operator-keywords.md)
