---
title: Advanced ledger entries in the public sector
description: Public-sector organizations can use advanced ledger entries to create, adjust, and reverse ledger entries. For example, advanced ledger entries can be used to reclassify expenditures if invoices are mistakenly posted to the wrong account or project.
author: rschloma
manager: AnnBe
ms.date: 2015-12-07 15 - 36 - 30
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: AdvancedLedgerEntry, BudgetControlConfiguration, LedgerParameters
audience: Application User
ms.reviewer: rschloma
ms.search.scope: AX 7.0.0, Operations
ms.custom: 19511
ms.assetid: 3db0233e-d767-4dc0-b008-733098b6ca70
ms.search.region: Global
ms.search.industry: Public sector
ms.author: brpotter
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: a5ec9dae77a2466520a28478497eff28fd3afcae
ms.lasthandoff: 02/22/2017


---

# <a name="advanced-ledger-entries-in-the-public-sector"></a>Advanced ledger entries in the public sector

Public-sector organizations can use advanced ledger entries to create, adjust, and reverse ledger entries. For example, advanced ledger entries can be used to reclassify expenditures if invoices are mistakenly posted to the wrong account or project.

<a name="how-do-i-set-up-advanced-ledger-entries"></a>How do I set up advanced ledger entries?
----------------------------------------

Verify that the **Advanced ledger entry** **License configuration** key is selected in the **License configuration** page. Advanced ledger entries require General ledger posting definitions. These posting definitions can be set up to generate multiple, balanced ledger entries based on the ledger account entered in the **Advanced ledger entries** page. For more information about posting definitions for advanced ledger entries, see [Posting definitions in the public sector](posting-definitions-public-sector.md).

## <a name="can-i-use-budget-control-with-advanced-ledger-entries"></a>Can I use budget control with advanced ledger entries?
Yes. If your organization uses budget control, you can enable budget control for advanced ledger entries on the **Budget control configuration** page.

## <a name="can-i-use-advanced-ledger-entries-with-projects"></a>Can I use advanced ledger entries with projects?
Yes. If you want users to be able to change the financial dimensions for a project on the advanced ledger entry line, you’ll need to select the **Allow the financial dimensions to be edited on the advanced ledger entry form** option on the **General ledger parameters** page. If you don’t select this option, users can change the financial dimensions in the **Ledger account** field only if the financial dimensions are not the default financial dimensions for a project.

## <a name="how-do-i-use-advanced-ledger-entries-to-record-yearend-accrual-entries"></a>How do I use advanced ledger entries to record yearend accrual entries?
Create an advanced ledger entry, select the **Reversing entry** option, and enter a reversing date. The reversing advanced ledger entry is created when the advanced ledger entry is posted. The reversing advanced ledger entry will have a new transaction number and a draft status. The reversing date will be used as the accounting date and the debit or credit amount on each line of the original entry will be reversed. The same posting definition will be used. The transaction text for the header and lines will contain the words “Reversing entry from,” the transaction number of the original advanced ledger entry, and the transaction text of the original advanced ledger entry.

<a name="see-also"></a>See also
--------

[General ledger](general-ledger.md)

[General ledger in the public sector](https://ax.help.dynamics.com/en/?post_type=incsub_wiki&p=164121)


