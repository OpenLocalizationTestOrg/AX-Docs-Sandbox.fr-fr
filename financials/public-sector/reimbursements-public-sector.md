---
title: Reimbursements in the public sector
description: This topic answers common questions related to reimbursements in the public sector.
author: twheeloc
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: CustBillingClassification
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: AX 7.0.0, Operations, Core
ms.custom: 27311
ms.assetid: 9d61d1d8-1672-4bd0-ae0d-605b09240890
ms.search.region: Global
ms.search.industry: Public sector
ms.author: brpotter
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: Human Translation
ms.sourcegitcommit: d421b161216d700f7819f1da8c0ca8ad089b5670
ms.openlocfilehash: 868018a921fd9ecf21dcd935c435ed0ccbf443ba
ms.contentlocale: fr-fr
ms.lasthandoff: 06/01/2017


---

# <a name="reimbursements-in-the-public-sector"></a>Reimbursements in the public sector

[!include[banner](../includes/banner.md)]


This topic answers common questions related to reimbursements in the public sector. 

<a name="what-happens-if-i-create-a-separate-reimbursement-transaction-for-each-billing-classification"></a>What happens if I create a separate reimbursement transaction for each billing classification?
----------------------------------------------------------------------------------------------

When you create a separate reimbursement transaction for each billing classification, the credit note transactions that are distributed to the same ledger account and that have the same billing classification will be combined into a single reimbursement transaction. Credit note transactions that are distributed to the same ledger account and that have different billing classifications will generate separate reimbursement transactions. For example, let’s say that you process reimbursements for three credit notes. All three credit notes are for $1000.

-   The first credit note has billing classification UTL, is distributed to three accounts, with 15% going to account 1110, 30% to account 2210, and 55% to account 3210.
-   The second credit note also has billing classification UTL. It is distributed 100% to account 3210.
-   The third credit note, with billing classification GEN, is distributed 100% to account 1110.

If you create a separate reimbursement transaction for each billing classification, four reimbursement transactions will be created, as follows:

-   $150 to account 1110
-   $1000 to account 1110
-   $300 to account 2210
-   $1550 to account 3210

The amounts going to account 3210 are combined, because they both use the same billing classification. The amounts going to account 1110 are not combined, because they do not use the same billing classification. If you do not create a separate reimbursement for each billing classification, the transactions for account 1110 would be combined, and only three reimbursement transactions would be created.

## <a name="how-do-billing-classifications-affect-reimbursements-for-overpayments"></a>How do billing classifications affect reimbursements for overpayments?
They don’t. Billing classifications are never applied to customer payments, so they aren’t used when processing reimbursements for overpayments.

## <a name="can-i-process-a-reimbursement-for-a-customer-who-has-outstanding-debit-transactions"></a>Can I process a reimbursement for a customer who has outstanding debit transactions?
Yes. If you need to process a reimbursement for a customer with outstanding debit transactions, use the filters on the reimbursement page to select the customer, and select the option to include customers with outstanding debit transactions. When you do this, reimbursement transactions are created for the full amount of all of the customer’s credit transactions. The outstanding debit amounts are not deducted from the credit amounts.

## <a name="can-i-process-reimbursements-for-customers-who-have-pending-settlements"></a>Can I process reimbursements for customers who have pending settlements?
No. Reimbursements are not processed for any customer who has pending settlements that have not been posted to the journal.

## <a name="can-i-reverse-reimbursement-settlements"></a>Can I reverse reimbursement settlements?
No, not directly. However, you could use general journal entries to create transactions that would have the effect of reversing the general ledger entries.






