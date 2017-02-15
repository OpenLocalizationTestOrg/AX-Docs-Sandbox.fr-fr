---
title: Chronological invoice and voucher numbers for France | Microsoft Docs
description: This topic explains how to set up and use chronological numbers for invoices and vouchers in Accounts receivable for legal entities in France.
author: ShylaThompson
manager: AnnBe
ms.date: 2016-12-19 16:05:52
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
keywords: CustParameters, NumberSequenceGroup
audience: Application User
ms.reviewer: 81
ms.suite: Released- Dynamics 365 for Operations version 1611
ms.custom: 264514
ms.assetid: f3712d16-f1d0-4f52-8f88-4735c450cc5f
ms.region: France
ms.author: ilyako
translationtype: Human Translation
ms.sourcegitcommit: d331960307ba214de4382feac7941aa5065c523d
ms.openlocfilehash: 973c1191d727e6797975ef5d0a62f8d2dd7d8ce4


---

# <a name="chronological-invoice-and-voucher-numbers-for-france"></a>Chronological invoice and voucher numbers for France

This topic explains how to set up and use chronological numbers for invoices and vouchers in Accounts receivable for legal entities in France.  

In France, there is a legal requirement that all invoices and related vouchers that are issued be numbered in chronological order. The chronology must be supported by fiscal periods. All the numbers that belong to earlier periods must be less than the numbers that belong to later periods. Within one fiscal period, chronological order isn't mandatory, but there must be no gaps in the numbering. To meet this requirement, chronological numbering in Accounts receivable affects the following documents:

-   Free text invoice
-   Free text invoice voucher
-   Free text credit note
-   Free text credit note voucher
-   Sales invoice
-   Sales invoice voucher
-   Sales credit note
-   Sales credit note voucher

## <a name="prerequisites"></a>Prerequisites
<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Category</th>
<th>Prerequisite</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Country/region</td>
<td>The primary address of the legal entity must be in France.</td>
</tr>
<tr class="even">
<td>Related setup tasks</td>
<td><ul>
<li>On the <strong>Accounts receivable parameters</strong> page, on the <strong>Updates</strong> tab, set the <strong>Chronological numbering</strong> option to <strong>Yes</strong>.</li>
<li>On the <strong>Number sequences</strong> page, define as many number sequences as you require to cover the affected fiscal periods. You should specify a company for each number sequence. The segments of the number sequences must be defined so that they provide chronological order for periods. For example, the segment names can contain a special prefix that identifies a specific period.</li>
</ul></td>
</tr>
</tbody>
</table>

## <a name="set-up-chronological-numbering"></a>Set up chronological numbering
### <a name="accounts-receivable-parameters"></a>Accounts receivable parameters

On the **Accounts receivable parameters** page, on the **Number sequences** tab, select one of the supported references, such as **Free text invoice**. Then click the **Chronological numbering setup** button that will be available for the supported references. On the **Chronological numbering setup** page, define the date-effective number sequences that have valid periods.

### <a name="number-sequence-groups"></a>Number sequence groups

If different customers use different patterns for numbering, you must set up chronological numbering at the level of the number sequence group. On the **Accounts receivable parameters** page, on the **Number sequences** tab, select one of the supported references, and then click **Group**. On the **Number sequence group** page, select an existing group, or create a new group. In the **Reference** section, select one of the supported references, and then click **Chronological numbering setup**. On the **Chronological numbering setup** page, define date-effective number sequences that have valid periods.

## <a name="invoice-posting"></a>Invoice posting
When you post an invoice or a credit note, the appropriate number sequence is used to generate a number. This number sequence is selected based on the valid period that contains the invoice date. Customer-specific chronological numbering has higher priority than chronological numbering.




<!--HONumber=Feb17_HO3-->


