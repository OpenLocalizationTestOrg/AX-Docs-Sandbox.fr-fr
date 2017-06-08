---
title: Update standard costs in a manufacturing environment
description: This article provides guidance about how to update standard costs in a manufacturing environment.
author: YuyuScheller
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: CostingVersion, InventStdCostConv
audience: Application User
ms.search.scope: AX 7.0.0, Operations, Core
ms.custom: 79663
ms.assetid: 3a7c3d13-8dbc-442d-a281-ac0ebe99ec83
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: mguada
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: Human Translation
ms.sourcegitcommit: d421b161216d700f7819f1da8c0ca8ad089b5670
ms.openlocfilehash: 74ad59504d6bbea0c604e0f0b83e74c915e84019
ms.contentlocale: fr-fr
ms.lasthandoff: 06/01/2017


---

# <a name="update-standard-costs-in-a-manufacturing-environment"></a>Update standard costs in a manufacturing environment

[!include[banner](../includes/banner.md)]


This article provides guidance about how to update standard costs in a manufacturing environment. 

Updates can reflect new items, cost categories, or indirect cost calculation formulas. They can also reflect corrections and cost changes. The type of update affects the steps that you must complete to update standard costs, as illustrated in the following cases:

-   Enter expected standard cost changes for purchased items, and then change the status of the item cost records to **Active** on the appropriate date. However, don't recalculate the costs of manufactured items that use the purchased items.
-   Enter standard costs for a new purchased item, but don't recalculate the costs of manufactured items that have a bill of materials (BOM) version that contains the new purchased item as a component.
-   Correct or change the cost of a purchased item, or change the cost group that is assigned to a purchased item, and calculate the cost for all manufactured items that have a BOM version that contains the purchased item as a component.
-   Change the cost for a cost category, and calculate the cost for all manufactured items that have a route version that contains routing operations that use the cost category.
-   Change the cost categories that are assigned to routing operations or the cost group that is assigned to cost categories. Then calculate the cost for all manufactured items that have a route version that contains routing operations that use the cost category.
-   Change an indirect cost calculation formula, and calculate the cost for all manufactured items that are affected by the change.
-   Change or add a manufacturing site for a manufactured item, and calculate the item's manufactured cost for the site.
-   Calculate, or recalculate, the cost for a manufactured item, and recalculate the cost for all manufactured items that have a BOM version that contains the manufactured item as a component.
-   Calculate costs for a new manufactured item, based on its defined, approved, and active BOM and route information.

Each case requires careful consideration about how to update standard costs.




