---
title: "Level function in a paginated report"
description: Discover the Level function in Report Builder. This function returns the current level of depth in a recursive hierarchy in a paginated report.
author: maggiesMSFT
ms.author: maggies
ms.reviewer: rpatkar
ms.date: 06/16/2023
ms.service: powerbi
ms.subservice: report-builder
ms.topic: conceptual
ms.custom: updatefrequency5
---
# Report Builder functions - Level function in a paginated report (Power BI Report Builder)

[!INCLUDE [applies-yes-report-builder-no-desktop](../../includes/applies-yes-report-builder-no-desktop.md)]

  Returns the current level of depth in a recursive hierarchy in a paginated report.

## Syntax

```syntaxsql
Level(scope)
```

### Parameters

*scope*  
(**String**) (Optional). The name of a dataset, group, or data region that contains the report items to which to apply the aggregate function. If *scope* is not specified, the current scope is used.

## Return Type

Returns an **Integer**. If *scope* specifies a dataset or data region, or specifies a nonrecursive grouping (that is, a grouping with no **Parent** element), **Level** returns 0. If *scope* is omitted, it returns the level of the current scope.

## Remarks

The value returned by the **Level** function is zero based; that is, the first level in a hierarchy is 0.

The **Level** function can be used to provide indentation in a recursive hierarchy, such as an employee list.

For more information about recursive hierarchies, see [Creating Recursive Hierarchy Groups (Power BI Report Builder)](./creating-recursive-hierarchy-groups-report-builder.md).

## Example

The following code example provides the level of row in the Employees group:

```
=Level("Employees")
```

## See also

- [Expression Uses in Reports (Power BI Report Builder)](./expression-uses-reports-report-builder.md)
- [Expression Examples (Power BI Report Builder)](./report-builder-expression-examples.md)
- [Data Types in Expressions (Power BI Report Builder)](./data-types-expressions-report-builder.md)
- [Expression Scope for Totals, Aggregates, and Built-in Collections (Power BI Report Builder)](./expression-scope-for-totals-aggregates-and-built-in-collections.md)
