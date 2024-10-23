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

For example, if your organization has a trademarked name that you don't want translated, you can add that to the glossary file. You can also specify the capitalization to use for words, choose specific translations for ambiguous words, or designate specific meanings for your unique context.

## Create a glossary file

Follow these steps to create a glossary file. You need to create separate glossary file for each language.

1. Create a CSV file (or [other supported file format](/azure/ai-services/translator/document-translation/reference/get-supported-glossary-formats)) that contains all the terms and phrases you want to use in your translation.

2. Use the first column to list the terms in the source language. Use the second column to list the terms in the target language. The terms in the glossary are case-senstive.

    ![Screenshot of a spreadsheet showing two columns with example source terms and target terms.](../media/content-understanding/translation-glossary-format-example.png)

3. Upload the file to the appropriate SharePoint document library or OneDrive folder.

## Update a glossary file

Follow these steps to update a glossary file.

1. Download the file from the SharePoint library to your computer.

2. Make the necessary changes to the file.

3. Save the updated CSV file on your computer.

4. Upload the updated file back to the SharePoint library.

## Link to a glossary file

If the glossary file you want to use is in the same SharePoint library as the document you want to translate, you can select it from the drop-down list. If the glossary file is in a different library, you need to add a link to the file.

Follow these steps to add a link to a glossary file.

1. Select the glossary file you want to use.

2. Next to the file name in the list of documents, select **More actions** (**...**), and then select **Details**.

    ![Screenshot showing the Details option next to the document.](../media/content-understanding/translation-more-actions-details.png)

3. On the **Details** panel, go to **Path**, and select the **Copy direct link** icon (![Image of the Copy direct link button.](../media/content-understanding/translation-copy-direct-link-icon.png)).

4. Go back to the **Translate documents** screen, select the languge, and under **Translation glossary**, paste the link.

