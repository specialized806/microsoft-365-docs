---
title: Create and use a custom glossary for document translation in Microsoft Syntex
ms.author: chucked
author: chuckedmonson
manager: jtremper
ms.reviewer: karlha, ssquires
ms.date: 11/15/2024
audience: admin
ms.topic: conceptual
ms.service: microsoft-syntex
ms.subservice: syntex-content-intelligence
search.appverid: 
ms.collection: 
    - enabler-strategic
    - m365initiative-syntex
ms.localizationpriority:  medium
description: Learn how to create, upload, and use a glossary file for document translation in Microsoft Syntex.
---

# Create and use a custom glossary for document translation in Microsoft Syntex

You can use a custom glossary file to ensure that the specific terminology is consistently and accurately translated. The glossary file contains a list of terms in the source language along with their corresponding translations in the target language.

For example, if your organization has a brand name that you don't want translated, you can add that to the glossary file. You can also choose specific translations for ambiguous words or designate specific meanings for your unique context.

## Create a glossary file

Follow these steps to create a glossary file. You need to create separate glossary file for each language.

1. Create a CSV file (or [other supported file format](/azure/ai-services/translator/document-translation/reference/get-supported-glossary-formats)) that contains all the terms and phrases you want to use in your translation.

2. Use the first column to list the terms in the source language. Use the second column to list the terms in the target language.

    ![Screenshot of a spreadsheet showing two columns with example source terms and target terms.](../media/content-understanding/translation-glossary-format-example.png)

3. Upload the file to the appropriate SharePoint document library or OneDrive folder.

## Use the glossary file

