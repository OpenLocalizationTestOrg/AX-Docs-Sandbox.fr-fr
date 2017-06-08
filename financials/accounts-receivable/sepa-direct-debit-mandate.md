---
title: Set up SEPA direct debit mandate
description: 
author: twheeloc
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.search.scope: AX 7.0.0, Operations, Core
ms.custom: 59491
ms.assetid: 653a135f-c515-4ae3-9da2-82b5e1f103b5
ms.search.region: Global
ms.author: mfalkner
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: Human Translation
ms.sourcegitcommit: d421b161216d700f7819f1da8c0ca8ad089b5670
ms.openlocfilehash: ebf80efa32b21184a8effdde4d46c4d0d2179efd
ms.contentlocale: fr-fr
ms.lasthandoff: 06/01/2017


---

# <a name="set-up-sepa-direct-debit-mandate"></a>Set up SEPA direct debit mandate

[!include[banner](../includes/banner.md)]




A Single Euro Payment Area (SEPA) direct debit lets a creditor collect funds from a customer's bank account, provided that the customer has granted a signed mandate to the creditor. The mandate that the customer signs authorizes the creditor to collect a payment and instructs the customer's bank to pay the collection. This topic is organized to show the process for setting up SEPA direct debit mandates.

## <a name="prerequisites"></a>Prerequisites
The following table shows the prerequisites that must be in place before you start.

| Category       | Prerequisite                                                                                                                                              |
|----------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| Country/region | The primary address for the legal entity must be in the following countries/regions: Austria, Belgium, Germany, Spain, France, Italy, or the Netherlands. |

1. Set up a number sequence for direct debit mandates Each direct debit mandate must have a unique number. Use the **Number sequences** page to create a number sequence for direct debit mandates. You will use this identifier to assign the number sequence to the direct debit mandate system on the **Accounts receivable parameters** page.

2. Set up Accounts receivable parameters for direct debit mandates Use the **Accounts receivable parameters** page to set up parameters for direct debit mandates. To set up the parameters, on the **Direct debit** tab, change the default parameters as you require. Then, on the **Number sequences** tab, update the **Direct debit mandate ID** field with the number sequence that you set up earlier.

3. Set up a method of payment for direct debit mandates You must set up a method of payment for direct debit mandates. You use this method of payment to query for invoices to generate direct debit payments for. Use the **Methods of payment** page to set up the method of payment. To set up a method of payment for direct debit mandates, you must follow these additional steps for a method of payment:

-   In the **Payment type** field, select **Electronic payment**.
-   Optional: If you expect each of your customers to have multiple mandates, in the **Period** field, select **Invoice**. A separate payment will be created for each invoice, and each payment will use the mandate that is specified for the invoice.
-   Select the **Require mandate** option to create payments by using direct debit mandates. The **Require mandate** option is available only if you select **Electronic payment** in the **Payment type** field.

See Also [Direct debit overview](sepa-direct-debit-overview.md) 


