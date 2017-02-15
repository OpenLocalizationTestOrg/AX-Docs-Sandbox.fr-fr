---
title: Year-end processing in the public sector | Microsoft Docs
description: This article provides information about year-end processing for a public sector organizations.
author: rschloma
manager: AnnBe
ms.date: 2015-12-07 16:21:31
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
keywords: PurchYearEndClose
audience: Application User
ms.reviewer: rschloma
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 19601
ms.assetid: a1a255fc-5fa5-46ec-928b-3cb04172c347
ms.region: Global
ms.industry: Public sector
ms.author: brpotter
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: 4b3bfdabcea5da4275a39aecfb464d22d3636420


---

# <a name="year-end-processing-in-the-public-sector"></a>Year-end processing in the public sector

This article provides information about year-end processing for a public sector organizations.

This topic describes the year-end functionality available for the public sector. At the end of a fiscal year, you must generate closing transactions and prepare your accounts for the next fiscal year.  Public sector clients have the following capabilities:

-   Select accounts by fund for year-end closing.
-   Close funds to different accounts. For example, you can close nominal accounts that are associated with governmental funds to fund balances. You can also close nominal accounts that are associated with proprietary funds to retained earnings.
-   Set up year-end closing for all funds and non-funds. Non-funds don't have a fund dimension in the account structure.
-   Set up multiple closing periods to segregate different types of closing entries, such as general year-end closing and audit adjustments.

## <a name="can-the-yearend-process-be-run-more-than-one-time-on-the-same-data"></a>Can the yearend process be run more than one time on the same data?
Yes, the year-end process can be run multiple times for the same set of data. Typically, if additional transactions must be processed after a general ledger year-end process is run, the year-end process can be run again to close out the nominal accounts and correctly set the opening balances in the new year.

## <a name="how-do-i-set-up-funds-for-yearend-processing"></a>How do I set up funds for yearend processing?
Year-end processing of general ledger balances is controlled by fund configuration settings in two places:

-   The year-end process of closing ledger balances in the old year and establishing opening balances in the new year is done by using the **Opening transactions** page. A single fund or range of funds is required for processing.
-   The year-end processing option for purchase order encumbrances is set on the **Purchase order year-end process** page. You can override the option on a specific fund, provided that the general ledger parameters have been set to allow for overrides. To learn more about the parameter settings, see [General ledger in the public sector](https://docs.microsoft.com/en-us/dynamics365/operations/financials/public-sector/general-ledger-in-the-public-sector).

## <a name="how-do-i-set-up-main-accounts-for-yearend-processing"></a>How do I set up main accounts for yearend processing?
You must select a close type for every account in your chart of accounts. The close type determines how the year-end process handles that main account. There are four close types:

-   **Real** – The balance is used to establish opening balances in the new year.
-   **Nominal** – The account is closed by the year-end process.
-   **Nominal – no close** – The account is managed by other closing processes, such as encumbrance accounts for purchase order close.
-   **Not applicable** – The account isn't included in year-end processing.

Posting definitions govern the accounting that occurs on the closing entries, and they also help create the opening transactions for the new year. To learn more, see [Posting definitions in the public sector](https://docs.microsoft.com/en-us/dynamics365/operations/financials/public-sector/posting-definitions-in-the-public-sector).




<!--HONumber=Feb17_HO3-->


