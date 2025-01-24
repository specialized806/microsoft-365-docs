---
title: Create a conditional section in a template in SharePoint Agreements
ms.author: chucked
author: chuckedmonson
manager: jtremper
ms.reviewer: ssathyamoort
ms.date: 10/22/2024
audience: admin
ms.topic: conceptual
ms.service: microsoft-syntex
ms.subservice: syntex-content-intelligence
search.appverid: 
ms.collection: 
    - enabler-strategic
    - m365initiative-syntex
ms.localizationpriority:  medium
ROBOTS: NOINDEX, NOFOLLOW
description: Learn how to create conditional sections in a template in the SharePoint Agreements solution.
---

# Add a conditional section to a template in SharePoint Agreements

## Add a conditional section to a template

Conditional sections in a template let you create documents that change based on the information given by the document authors.

Before you can create a conditional section, you first need to add fields to the template on which the condition is based. Then, follow these steps to create a conditional section.

1. In the document, open the **Manage templates** panel and select **Define conditional sections**.

   ![A screenshot of an opened document and the Manage templates panel.](../../media/content-understanding/agreements-define-conditional-sections.png)

2. On the **Manage templates** panel, under **Conditional sections**, select **+ New** to start adding the condition.

   ![A screenshot of the Conditional sections area on the Manage templates panel.](../../media/content-understanding/agreements-new-conditional-section.png)

3. Under **New conditional section**, in the **Name** box, enter a name that reflects the content you've selected. (For this example, we named it *Reimbursement Section*.)

   ![A screenshot of the New conditional section area on the Manage templates panel.](../../media/content-understanding/agreements-name-new-conditional-section.png)

### Set conditions

You can add conditions to specify whether this section of the template will be included in the final generated document based on the values of the fields entered by the author.

For this example, we want to show the selected content for two conditions: if the fees are less 10,000 and if the nature of employment is full time.

#### Add the first condition

On the **Manage templates** panel, in the **Set up condition** section:

1. Select **Choose a field**, and then select the appropriate field. (For this example, we selected *Fees*.)

2. Select **Choose a condition**, and then select the appropriate condition. (For this example, we selected *lesser than*.)

3. Select **Enter a value**, and then enter the appropriate value. (For this example, we entered *10000*.)

   ![A screenshot of the first condition in the Set up condition section on the Manage templates panel.](../../media/content-understanding/agreements-add-first-condition.png)

#### Add additional conditions

In the **Set up condition** section:

1. Under the first condition, select **+ And** or **+ Or**, depending how you want the additional condition to be linked to the first condition. (For this example, we chose *And*.)

2. Select **Choose a field**, and then select the appropriate field. (For this example, we selected *Nature of employment*.)

3. Select **Choose a condition**, and then select the appropriate condition. (For this example, we selected *exact match*.)

4. Select **Enter a value**, and then enter the appropriate value. (For this example, we entered *FTE*.)

   ![A screenshot of an additional condition in the Set up condition section on the Manage templates panel.](../../media/content-understanding/agreements-add-additional-conditions.png)

5. When you're done entering conditions, select **Save**. You can see the new condition under **Conditional sections**.

   ![A screenshot of the new condition on the Condition sections panel on the Manage templates panel.](../../media/content-understanding/agreements-saved-condition.png)

#### Map the condition to a document section

After creating the condition, you need to map it to the section of the document that you want to display based on this condition. To do this, select the relevant section in the document and then select **Map**.

If you want to change the section of the document mapped to this condition, select **Unmap** and then repeat the process of mapping a section to the condition.

#### Edit a conditional section

To edit the conditions in a conditional section, select **More options** (**...**), and then select **Edit**.

   ![A screenshot of a condition section showing the Edit and Delete options on the Manage templates panel.](../../media/content-understanding/agreements-edit-delete-condition.png)

#### Delete a conditional section

To delete the conditions in a conditional section, select **More options** (**...**), and then select **Delete**. This deletes the condition and unmaps the selected section.

> [!NOTE]
> - You can create conditional sections around text, complete paragraphs, and entire tables. To create conditional sections around images, ensure the images are inline images.
>- You can't add conditions around table rows and columns.
>- You can't map multiple sections in the document to one condition. One condition can only be mapped to one section in the document.
>- You can't add nested conditions. To achieve nested conditions, you need to create conditional sections around every section and specify all the required conditions.


