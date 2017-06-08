---
title: Use quick import/export
description: The purpose of Quick import export is to let you import and export with fewer steps.
author: margoc
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: dynamics-ax-2012
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.search.scope: AX 2012 R3 CU8
ms.custom: 89041
ms.assetid: 990d64e6-d436-4c79-9bb5-bf8c5c5a048f
ms.search.region: Global
ms.author: margoc
ms.search.validFrom: 
ms.dyn365.ops.version: AX 2012 R3 CU8
ms.translationtype: Human Translation
ms.sourcegitcommit: d421b161216d700f7819f1da8c0ca8ad089b5670
ms.openlocfilehash: 11cf53af2db453471175cec5de63d38f8b680c9b
ms.contentlocale: fr-fr
ms.lasthandoff: 06/01/2017


---

# <a name="run-the-test-data-transfer-tool-beta-for-dynamics-ax-ax-2012"></a>Run the Test Data Transfer Tool (beta) for Dynamics AX (AX 2012)

[!include[banner](../../includes/banner.md)]


The purpose of Quick import export is to let you import and export with fewer steps.

We added the Quick Import Export feature to let users import or export simple jobs that they want to execute quickly. Ideally this feature is used in scenarios in which a file automatically maps to the system and user does not need to go through advanced mapping or create repeated import or export jobs.

-   This feature supports working with both out-of-the-box and custom entities.
-   You can import from files, and if you are using an ODBC data source, you can select a query to use to define your import.
-   You must have previously defined source data formats for either AX or File, and know where they are located.
-   You do not need to create a processing group to use quick import/export, one will be automatically created by the system when executing the import or export job. You can also choose keep the history of the data imported by the quick import/export.

  Note that Quick import export assumes that you are familiar with the concepts of DIXF.




