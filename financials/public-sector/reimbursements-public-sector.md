---
title: Reimbursements in the public sector | Microsoft Docs
description: This topic answers common questions related to reimbursements in the public sector.
author: rschloma
manager: AnnBe
ms.date: 2015-12-13 05:21:25
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
keywords: CustBillingClassification
audience: Application User
ms.reviewer: rschloma
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 27311
ms.assetid: c9951d98-6623-42cf-b389-d8035b45c94a
ms.region: Global
ms.industry: Public sector
ms.author: brpotter
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: 96409cb75236065d40e3216927cd75f7cbce6e57


---

# <a name="reimbursements-in-the-public-sector"></a>Reimbursements in the public sector

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

<a name="see-also"></a>See also
--------

[Accounts receivable](https://docs.microsoft.com/en-us/dynamics365/operations/financials/accounts-receivable/accounts-receivable)

[Accounts receivable in the public sector](https://ax.help.dynamics.com/en/?post_type=incsub_wiki&p=169941)

[Billing classifications and billing codes in the public sector](https://ax.help.dynamics.com/en/?post_type=incsub_wiki&p=169891)




<!--HONumber=Feb17_HO3-->


