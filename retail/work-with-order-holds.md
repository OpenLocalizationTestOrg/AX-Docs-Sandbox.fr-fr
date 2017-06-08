---
title: Order holds
description: This topic describes holds on orders using Retail and commerce in Dynamics AX.
author: josaw1
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.search.scope: AX 7.0.0, Operations, Core, Retail
ms.custom: 79132
ms.assetid: 7c00dc35-73e5-400a-8587-22f37ddfc0e0
ms.search.region: global
ms.search.industry: Retail
ms.author: josaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: Human Translation
ms.sourcegitcommit: d421b161216d700f7819f1da8c0ca8ad089b5670
ms.openlocfilehash: 5e18a488fed92de3278b438af67ae72fdbe229b4
ms.contentlocale: fr-fr
ms.lasthandoff: 06/01/2017


---

# <a name="order-holds"></a>Order holds

[!include[banner](includes/banner.md)]


This topic describes holds on orders using Retail and commerce in Dynamics AX.

An order can be put on hold for various reasons. For example, you might put an order on hold until the customer address or payment method can be verified, or until a manager can review the customer’s credit limit. During the sales process, there are times when sales orders must be put on hold. For example, a sales order might be put on hold because of issues with a customer payment, because of suspected fraud, or because a manager must review the order. When a sales order is put on hold, an order hold code is assigned to the sales order to indicate the reason for the hold. Sales order hold codes are configured at **Sales and marketing** &gt; **Setup** &gt; **Sales orders** &gt; **Order holds codes**. A sales order can be put on hold manually at the time of order creation or later. Additionally, an order can be put on hold automatically, based on fraud rules. While a sales order is on hold, you might have to update it with more information. Alternatively, you might want to check out the sales order as you continue to work on it. You can check out a sales order, check it back in, and even override the checkout of another user by using the order hold workbench (**Retail and commerce** &gt; **Customers** &gt; **Order holds**). When an order is ready to be completed, you must remove the hold before you can complete the order process.




