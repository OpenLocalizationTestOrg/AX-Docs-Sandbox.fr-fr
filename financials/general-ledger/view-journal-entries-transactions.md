---
title: View journal entries and transactions
description: This article explains the various ways that you can view journal entries and transactions.
author: RobinARH
manager: AnnBe
ms.date: 2015-12-01 16 - 42 - 09
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: LedgerTransVoucher
audience: Application User
ms.reviewer: RobinARH
ms.search.scope: AX 7.0.0, Operations
ms.custom: 13031
ms.assetid: 281c7ea6-4dfd-4d1f-994f-c361ee299dbe
ms.search.region: Global
ms.author: aolson
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 2793c7a26d4ffa3b3b5edd67d0cb1a7aa57a0ae3
ms.lasthandoff: 02/22/2017


---

# <a name="view-journal-entries-and-transactions"></a>View journal entries and transactions

This article explains the various ways that you can view journal entries and transactions. 

Users who want to view journals and transactions have several ways to access the data. They can take advantage of inquiry pages that provide drill-down ability, or they can use various report options in the general ledger.

## <a name="voucher-transactions"></a>Voucher transactions
**Voucher transactions** is an inquiry page where you can select from various tables and fields to specify criteria for the balance or transaction that you're searching for. For example, you can view all transactions for a specific date or account, or all transactions of the **Operating** type that are in a specific posting layer. By default, the page shows the journal number, voucher, date, and main account, but you can add additional tables, fields, and criteria to narrow down your search.

## <a name="audit-trail"></a>Audit trail
**Audit trail** is an inquiry page that shows the types of transactions, descriptions, who the transactions were created by, and when they were created. From the **Audit trail** inquiry page, you can view the voucher transactions.

## <a name="financial-reports"></a>Financial reports
You can also explore and analyze general ledger transactions by running financial reports. Because the design of financial reports can be based on accounts, dimensions, account categories, or a combination of the three, you can view the transactions by drilling down in various ways. If you require more information for general ledger transactions, you can also include multiple transaction properties as part of the report design. Additionally, if you want to see the transactions that make up a general ledger balance, you can drill down to account transactions, just as you can from the **Trial balance** list page.

## <a name="ledger-reports"></a>Ledger reports
In addition to the financial reports, you can use the following ledger reports to view general ledger transactions:

-   **Dimension statement** – This report shows transactions by day and account, and there are also options to show transactions by dimension and period.
-   **Ledger transaction list** – This report shows transactions in transaction, accounting, and reporting currencies for an account.
-   **Print journal** – This report shows the result of a posted journal. You can run the report by journal batch number or journal type, or add additional fields.
-   **Posted transactions by journal** – This report shows the transactions that have been posted to a journal, grouped by voucher.
-   **Transaction list by date** – This report shows all the transactions by date, together with the journal number, voucher, and ledger account. It also shows the transactions in the transaction, accounting, and reporting currencies.
-   **Transaction origin** – This transaction report shows the account by journal, and by transaction, accounting, and reporting currency. It also shows each line of the journal that was used as an offset.


<a name="see-also"></a>See also
--------

[General ledger account balances](general-ledger-account-balances.md)

[Accounting source explorer](https://ax.help.dynamics.com/en/?post_type=incsub_wiki&p=245244)

[Financial reporting](financial-reporting-getting-started.md)

