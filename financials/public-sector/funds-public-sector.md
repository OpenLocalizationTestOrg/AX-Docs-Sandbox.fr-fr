---
title: Funds in the public sector | Microsoft Docs
description: A fund is a self-balancing set of financial books that is used to control and monitor the planned use of resources, often in compliance with legal and administrative requirements. Public-sector organizations use funds to demonstrate their fiscal accountability.
author: rschloma
manager: AnnBe
ms.date: 2015-12-07 16:20:40
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
keywords: LedgerFund, LedgerFundType
audience: Application User
ms.reviewer: rschloma
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 19571
ms.assetid: 6d9646fe-b4cf-48cd-ae81-913bbd2f59d9
ms.region: Global
ms.industry: Public sector
ms.author: brpotter
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: fb68df55de6448dd4611ca92fd5c81d1fc929492


---

# <a name="funds-in-the-public-sector"></a>Funds in the public sector

A fund is a self-balancing set of financial books that is used to control and monitor the planned use of resources, often in compliance with legal and administrative requirements. Public-sector organizations use funds to demonstrate their fiscal accountability.

<a name="what-general-ledger-parameters-should-be-set-for-funds"></a>What General ledger parameters should be set for funds?
-------------------------------------------------------

To learn about the General ledger parameters required for funds, see [General ledger in the public sector](https://docs.microsoft.com/en-us/dynamics365/operations/financials/public-sector/general-ledger-in-the-public-sector).

## <a name="what-fund-classes-and-fund-types-do-i-need-to-set-up"></a>What fund classes and fund types do I need to set up?
The Governmental Accounting Standards Board (GASB) recommends a set of Generally Accepted Accounting Principles (GAAP) for state and local governmental accounting.  The GAAP identifies eight fund types that are categorized under the three fund classes:

-   Governmental funds
    -   General fund
    -   Special revenue funds
    -   Capital project funds
    -   Debt service funds
-   Proprietary, or business-type, funds
    -   Enterprise funds
    -   Internal service funds
-   Fiduciary funds
    -   Trust funds
    -   Agency funds

The three GAAP fund classes, plus a **Memo** class, are predefined options in Microsoft Dynamics 365 for Operations. Fund types are defined according to the needs of the organization. In most cases, you’ll set up the eight GAAP fund types. The fund types group funds for detailed fiscal tracking and reporting. Many funds can be included in a single high-level report, but each fund remains a separate fiscal and accounting entity with its own general ledger, income statements, and balance sheet reports. Each fund must have a unique fund number. In Dynamics 365 for Operations, fund numbers are used as dimension values in financial account numbers where a dimension has been mapped to a fund. When an account number is linked to a particular fund, it belongs to the set of financial books that are contained by that fund.

### <a name="example"></a>Example

Here’s a list of some of the funds that might be used by a town government:

-   General Fund
-   School of Technology
-   Information Technology
-   Farmers Market
-   Utilities Commission
-   Courier Service
-   Worker’s Compensation Fund
-   Comprehensive Major Medical Plan
-   Deferred Compensation
-   Local Sales Tax Collections
-   Clerk of Courts

The following table shows these funds grouped by fund class and fund type.

|                |                        |                 |                                  |
|----------------|------------------------|-----------------|----------------------------------|
| **Fund class** | **Fund type**          | **Fund number** | **Fund name**                    |
| Governmental   | General Fund           | 1103            | General Fund                     |
|                | Special Revenue Funds  | 1343            | School of Technology             |
|                |                        | 1372            | Information Technology           |
| Proprietary    | Enterprise Funds       | 2501            | Farmers Market                   |
|                |                        | 2541            | Utilities Commission             |
|                | Internal Service Funds | 2723            | Courier Service                  |
|                |                        | 2738            | Worker’s Compensation Fund       |
| Fiduciary      | Pension Trust Funds    | 3320            | Comprehensive Major Medical Plan |
|                |                        | 3324            | Deferred Compensation            |
|                | Agency Funds           | 3912            | Local Sales Tax Collections      |
|                |                        | 3914            | Clerk of Courts                  |

## <a name="how-are-financial-dimensions-used-with-funds"></a>How are financial dimensions used with funds?
Each fund must have a unique fund number. In Dynamics 365 for Operations, fund numbers are used as dimension values in financial account numbers where a dimension has been mapped to a fund. When an account number is linked to a particular fund, it belongs to the set of financial books that are contained by that fund. Public sector organizations usually require balanced entries for financial dimensions related to funds. When a financial dimension or a combination of dimensions is marked to require balanced entries, the system will not post a transaction where debits do not equal credits for the financial dimension.

## <a name="how-do-i-set-a-fund-balance-to-carry-over-to-the-new-year"></a>How do I set a fund balance to carry over to the new year?
To learn about year-end processing for funds, see [Year-end processing in the public sector](https://docs.microsoft.com/en-us/dynamics365/operations/financials/public-sector/year-end-processing-in-the-public-sector).




<!--HONumber=Feb17_HO3-->


