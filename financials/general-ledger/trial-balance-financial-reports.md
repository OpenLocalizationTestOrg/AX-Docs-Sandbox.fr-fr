---
title: Trial balance financial reports
description: This article describes the default reports for trial balances. It also describes the building blocks that are associated with these reports and how you can modify the reports to fit your business requirements.
author: twheeloc
manager: AnnBe
ms.date: 2015-11-04 19 - 44 - 32
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.reviewer: annbe
ms.search.scope: AX 7.0.0, Operations
ms.custom: 12314
ms.assetid: 3b77d6f3-fd07-41a7-9ddb-1b22d1ae33fc
ms.search.region: Global
ms.author: jcart
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 6d603bb16218644ea7113db794cc47e3dfb77261
ms.lasthandoff: 02/22/2017


---

# <a name="trial-balance-financial-reports"></a>Trial balance financial reports

This article describes the default reports for trial balances. It also describes the building blocks that are associated with these reports and how you can modify the reports to fit your business requirements. 

<a name="default-trial-balance-reports"></a>Default trial balance reports
-----------------------------

Three trial balance reports are available in Financial reporting in Microsoft Dynamics 'AX 7'.

| Default report                                 | What it does                                                                                                                                                                                        |
|------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Detailed Trial Balance - Default               | Provides balance information for all accounts, and includes debit and credit balances, and the net of these, together with the transaction date, voucher, and journal description.                  |
| Summary Trial Balance – Default                | Provides balance information for all accounts, and includes opening and closing balances, and debit and credit balances, together with their net difference.                                        |
| Summary Trial Balance Year Over Year – Default | Provides balance information for all accounts, and includes opening and closing balances, and debit and credit balances, together with their net difference for the current year and the past year. |

## <a name="building-blocks"></a>Building blocks
The trial balance financial reports use the following building blocks.

| Default report                                 | Row definition          | Column definition                              |
|------------------------------------------------|-------------------------|------------------------------------------------|
| Detailed Trial Balance - Default               | Trial Balance - Default | Detailed Trial Balance - Default               |
| Summary Trial Balance – Default                | Trial Balance - Default | Summary Trial Balance - Default                |
| Summary Trial Balance Year Over Year – Default | Trial Balance - Default | Summary Trial Balance Year Over Year - Default |

### <a name="row-definition"></a>Row definition

The row definition, Trial Balance – Default, contains a single row that pulls in all main accounts. Therefore, anyone can generate the report without having to make any modifications. When you view the report, you drill into the single row to see details about each account. You can modify the row definition so that it includes more detail. To modify the Trial Balance – Default row definition so that it includes rows for all accounts, follow these steps.

1.  Click **Edit**, and then click **Insert Rows from Dimensions**. The **Insert Rows from Dimensions** command lets you choose the dimensions that you want to have in your row definition. For this row definition, you're going to use **Main Account**.
2.  Make sure that **Main Account** contains all ampersands (&), and then click **OK**.

The row definition now contains all the main accounts for your default legal entity.

### <a name="column-definition"></a>Column definition

Each trial balance report uses a different column definition. These column definitions contain different types of columns to provide different levels of detail and financial data.

-   **Detailed Trial Balance – Default column types:**
    -   **DESC** – The description from the row definition
    -   **ACCT** – Account codes
    -   **ATTR (3)** – Attributes:
        -   Transaction Date
        -   Voucher
        -   Journal Description
    -   **FD** – Financial data that contains only debits
    -   **FD** – Financial data that contains only credits
    -   **CALC** – The net difference
-   **Summary Trial Balance – Default columns types:**
    -   **ACCT** – Account codes
    -   **DESC** – The description from the row definition
    -   **ATTR** – An attribute:
        -   Voucher
    -   **FD** – The beginning balance financial data
    -   **FD** – Financial data that contains only debits
    -   **FD** – Financial data that contains only credits
    -   **CALC** – The net difference
    -   **CALC** – The closing balance
-   **Summary Trial Balance Year Over Year – Default:**
    -   **ACCT** – Account codes
    -   **DESC** – The description from the row definition
    -   **ATTR** – An attribute
        -   Voucher
    -   **FD** – The beginning balance financial data for the current year
    -   **FD** – Financial data that contains only debits for the current year
    -   **FD** – Financial data that contains only credits for the current year
    -   **CALC** – The net difference
    -   **CALC** – The closing balance
    -   **FD** – Financial data that contains only debits for the last year
    -   **FD** – Financial data that contains only credits for the last year

 

<a name="see-also"></a>See also
--------

[Financial reporting](financial-reporting-getting-started.md)

[View financial reports](view-financial-reports.md)

[Dynamics Financial Reporting Blog](http://blogs.msdn.com/b/dynamics_financial_reporting/)

