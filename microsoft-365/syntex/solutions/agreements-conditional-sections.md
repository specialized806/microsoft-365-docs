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

# Create a conditional section in a template in SharePoint Agreements

Conditional sections in a template let you create documents that change based on the information given by the authors.

Before you can create a conditional section, you first need to add fields to the template on which the condition is based. Then, follow these steps to create a conditional section.
1.	In the document, open the Manage templates panel and select “Define Conditional Sections”
 
2.	On the “Conditional Sections” panel, click on “+ New” to start adding the condition. 
 
3.	On the New conditional section panel, in the Name box, enter a name that reflects the content you've selected. (For this example, we named it Reimbursement Section.)
 
Set conditions
You can add conditions to specify whether this section of the template will be included in the final generated document based on the values of the fields entered by the author.
For this example, we want to show the selected content for two conditions: if the fees are lesser than ten thousand and if the nature of employment is full time.
To add the first condition
a)	On the Set condition panel, from the Choose a field dropdown list, select the appropriate field. (For this example, we selected Fees.)
b)	From the Choose a condition dropdown list, select the appropriate condition. (For this example, we selected lesser than.)
c)	In the Enter a value box, enter the appropriate value. (For this example, we entered 10000.)
 
To add additional conditions
a)	On the Set condition panel, select + And or Or, depending how you want the additional condition to be linked to the first condition. (For this example, we chose And.)
b)	On the Set condition panel, from the Choose a field dropdown list, the appropriate field. (For this example, we selected Nature of Employment.)
c)	From the Choose a condition dropdown list, select the appropriate condition. (For this example, we selected exact match.)
d)	In the Enter a value box, enter the appropriate value. (For this example, we entered Full Time.)
 

When you're done entering conditions, select Save. The new condition is visible in the Conditional Sections panel.
 
Once the condition is created you need to map the condition to the section of the document which you want to be displayed based on this condition. To map a section, select the relevant section in the document and then click on “Map”
 
If you want to change the section of the document mapped to this condition, you can click on “Unmap” and then repeat the process of mapping a section to the condition again
Edit a conditional section
To edit the conditions in a conditional section, select the three dots, and then select Edit.
 
Delete a conditional section
To edit the conditions in a conditional section, select the three dots, and then select Delete. This will delete the condition and also unmap the selected section
 

 Note
•	You can create conditional sections around text, complete paragraphs and entire tables. To create conditional sections around images, ensure the images are inline images
•	You cannot add conditions around table rows and columns.
•	You cannot map multiple sections in the document to one condition. One condition can only be mapped to one section in the document.
•	You can't add nested conditions. To achieve nested conditions, you need to create conditional sections around every section and specify all the required conditions.


