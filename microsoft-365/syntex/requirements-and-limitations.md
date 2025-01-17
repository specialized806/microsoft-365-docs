---
title: Requirements and limitations for pay-as-you-go services in SharePoint
ms.author: chucked
author: chuckedmonson
manager: jtremper
ms.reviewer: ssquires
ms.date: 01/16/2025
audience: admin
ms.topic: conceptual
ms.service: microsoft-syntex
search.appverid: 
ms.collection: 
    - essentials-manage
    - m365initiative-syntex
ms.localizationpriority:  medium
description: Learn about file limitations, file types, supported languages, and other requirements for pay-as-you-go services in SharePoint.
---

# Requirements and limitations for pay-as-you-go services in SharePoint

<!---<sup>**Applies to:**  &ensp; &#10003; All custom models &ensp; | &ensp; &#10003; All prebuilt models</sup>--->

Certain services might have additional or specific requirements, including file type and size, supported languages, geographical considerations, and other factors that might guide your decision on how to use the service.
<!---
Services:

- [Document translation](#document-translation)
- [Prebuilt document processing](#prebuilt-document-processing)
- [Structured and freeform document processing](#structured-and-freeform-document-processing)
- [Unstructured document processing](#unstructured-document-processing)--->
<!---
Models and services:

- [Document translation](#document-translation)
- [Prebuilt document processing](#prebuilt-document-processing)
    - [Contract processing](#contract-processing)
    - [Invoice processing](#invoice-processing)
    - [Receipt processing](#receipt-processing)
    - [Sensitive information processing](#sensitive-information-processing)
    - [Simple document processing](#simple-document-processing)
- [Structured and freeform document processing](#structured-and-freeform-document-processing)
    - [Freeform document processing](#freeform-document-processing)
    - [Structured document processing](#structured-document-processing)
- [Unstructured document processing](#unstructured-document-processing)
--->
## Document translation

| Icon          | Description   |
| ------------- | ------------- |
| ![Files symbol.](/office/media/icons/files-blue.png)  | **Supported file types** <br>This service supports the following file types: .csv, .docx, .htm, .html, .markdown, .md, .msg, .pdf, .pptx, .txt, and .xlsx. <br>For older file types like .doc, .rtf, .xls, .ods, .ppt, and .odp, the translated copy will be created in the modern equivalent formats: .docx, .xlsx, or .pptx. <br>SharePoint site pages aren't supported at this time. |
| ![Check mark in a circle symbol.](/office/media/icons/success-blue.png)  | **Supported file sizes** <br>The maximum file size for documents to be translated is limited to 40 MB. |
| ![Conversation symbol.](/office/media/icons/chat-room-conversation-blue.png)  | **Supported languages** <br>This service is available for [all supported languages and dialects](/azure/ai-services/translator/language-support?source=recommendations#translation). |
| ![Globe symbol.](/office/media/icons/globe-internet.png)  | **Multi-Geo environments** <br>When setting up this service in a [Microsoft 365 Multi-Geo](/microsoft-365/enterprise/microsoft-365-multi-geo) environment, you can only configure it to use the service in the central location. If you want to use this service in a satellite location, contact Microsoft support. |

## Prebuilt document processing

- [Contract processing](#contract-processing)
- [Invoice processing](#invoice-processing)
- [Receipt processing](#receipt-processing)
- [Sensitive information processing](#sensitive-information-processing)
- [Simple document processing](#simple-document-processing)

### Contract processing

| Icon          | Description   |
| ------------- | ------------- |
| ![Files symbol.](/office/media/icons/files-blue.png)  | **Supported file types** <br>This model supports the following file types: .bmp, .jpeg, .pdf, .png, and .tiff. |
| ![Conversation symbol.](/office/media/icons/chat-room-conversation-blue.png)  | **Supported languages** <br>This model supports only English language contracts. |
| ![Paragraph symbol.](/office/media/icons/paragraph-writing-blue.png)  | **OCR considerations** <br>This model uses optical character recognition (OCR) technology to scan .pdf files, image files, and .tiff files. OCR processing works best on documents that meet the following requirements: <br> - File format of .jpg, .png, or .pdf (text or scanned). Text-embedded .pdf files are better, because there won't be any errors in character extraction and location. <br> - For .pdf and .tiff files, up to 2,000 pages can be processed. <br> - The file size must be less than 50 MB. <br> -  For images, dimensions must be between 50 x 50 and 10,000 x 10,000 pixels. <br> - For .pdf files, dimensions must be at most 11 x 17 inches, corresponding to Legal or A3 paper sizes and smaller. <br> - The total size of the training data is 500 pages or less. |
| ![Globe symbol.](/office/media/icons/globe-internet.png)  | **Multi-Geo environments** <br>When setting up Syntex in a [Microsoft 365 Multi-Geo](/microsoft-365/enterprise/microsoft-365-multi-geo) environment, you can only configure it to use the model type in the central location. If you want to use this model type in a satellite location, contact Microsoft support. |
| ![Objects symbol.](/office/media/icons/objects-blue.png)  | **Multi-model libraries** <br>If two or more trained models are applied to the same library, the file is classified using the model that has the highest average confidence score. The extracted entities will be from the applied model only. |

### Invoice processing

| Icon          | Description   |
| ------------- | ------------- |
| ![Files symbol.](/office/media/icons/files-blue.png)  | **Supported file types** <br>This model supports the following file types: .bmp, .jpeg, .pdf, .png, and .tiff. |
| ![Conversation symbol.](/office/media/icons/chat-room-conversation-blue.png)  | **Supported languages** <br>This model supports invoices in English, Spanish, German, French, Italian, Portuguese, and Dutch. |
| ![Paragraph symbol.](/office/media/icons/paragraph-writing-blue.png)  | **OCR considerations** <br>This model uses optical character recognition (OCR) technology to scan .pdf files, image files, and .tiff files. OCR processing works best on documents that meet the following requirements: <br> - File format of .jpg, .png, or .pdf (text or scanned). Text-embedded .pdf files are better, because there won't be any errors in character extraction and location. <br> - For .pdf and .tiff files, up to 2,000 pages can be processed. <br> - The file size must be less than 50 MB. <br> -  For images, dimensions must be between 50 x 50 and 10,000 x 10,000 pixels. <br> - For .pdf files, dimensions must be at most 11 x 17 inches, corresponding to Legal or A3 paper sizes and smaller. <br> - The total size of the training data is 500 pages or less. |
| ![Globe symbol.](/office/media/icons/globe-internet.png)  | **Multi-Geo environments** <br>When setting up Syntex in a [Microsoft 365 Multi-Geo](/microsoft-365/enterprise/microsoft-365-multi-geo) environment, you can only configure it to use the model type in the central location. If you want to use this model type in a satellite location, contact Microsoft support. |
| ![Objects symbol.](/office/media/icons/objects-blue.png)  | **Multi-model libraries** <br>If two or more trained models are applied to the same library, the file is classified using the model that has the highest average confidence score. The extracted entities will be from the applied model only. |

### Receipt processing

| Icon          | Description   |
| ------------- | ------------- |
| ![Files symbol.](/office/media/icons/files-blue.png)  | **Supported file types** <br>This model supports the following file types: .bmp, .jpeg, .pdf, .png, and .tiff. |
| ![Conversation symbol.](/office/media/icons/chat-room-conversation-blue.png)  | **Supported languages** <br>This model supports receipts in English, Croation, Czech, Danish, Dutch, Finnish, German, Hungarian, Italian, Japanese, Latvian, Lithuanian, Norwegian, Portuguese, Spanish, Swedish, and Vietnamese. |
| ![Paragraph symbol.](/office/media/icons/paragraph-writing-blue.png)  | **OCR considerations** <br>This model uses optical character recognition (OCR) technology to scan .pdf files, image files, and .tiff files. OCR processing works best on documents that meet the following requirements: <br> - File format of .jpg, .png, or .pdf (text or scanned). Text-embedded .pdf files are better, because there won't be any errors in character extraction and location. <br> - For .pdf and .tiff files, up to 2,000 pages can be processed. <br> - The file size must be less than 50 MB. <br> -  For images, dimensions must be between 50 x 50 and 10,000 x 10,000 pixels. <br> - For .pdf files, dimensions must be at most 11 x 17 inches, corresponding to Legal or A3 paper sizes and smaller. <br> - The total size of the training data is 500 pages or less. |
| ![Globe symbol.](/office/media/icons/globe-internet.png)  | **Multi-Geo environments** <br>When setting up Syntex in a [Microsoft 365 Multi-Geo](/microsoft-365/enterprise/microsoft-365-multi-geo) environment, you can only configure it to use the model type in the central location. If you want to use this model type in a satellite location, contact Microsoft support. |
| ![Objects symbol.](/office/media/icons/objects-blue.png)  | **Multi-model libraries** <br>If two or more trained models are applied to the same library, the file is classified using the model that has the highest average confidence score. The extracted entities will be from the applied model only. |

### Sensitive information processing

| Icon          | Description   |
| ------------- | ------------- |
| ![Files symbol.](/office/media/icons/files-blue.png)  | **Supported file types** <br>This model supports the following file types: .csv, .doc, .docx, .eml, .heic, .heif, .htm, .html, .jpeg, .jpg, .md, .msg, .pdf, .png, .ppt, .pptx, .rtf, .tif, .tiff, .txt, .xls, and .xlsx. |
| ![Conversation symbol.](/office/media/icons/chat-room-conversation-blue.png)  | **Supported languages** <br>This model supports the following languages: see [supported languages](/azure/ai-services/language-service/personally-identifiable-information/language-support?tabs=documents#pii-language-support). <br>This model also supports languages for both [handwritten text](/azure/ai-services/computer-vision/language-support#handwritten-text) and [print text](/azure/ai-services/language-service/personally-identifiable-information/language-support?tabs=documents#pii-language-support). |
| ![Paragraph symbol.](/office/media/icons/paragraph-writing-blue.png)  | **OCR considerations** <br>This model uses optical character recognition (OCR) technology to scan .pdf files, image files, and .tiff files. OCR processing works best on documents that meet the following requirements: <br> - File format of .jpg, .png, or .pdf (text or scanned). Text-embedded .pdf files are better, because there won't be any errors in character extraction and location. <br> - For .pdf and .tiff files, up to 2,000 pages can be processed. <br> - The file size must be less than 50 MB. <br> -  For images, dimensions must be between 50 x 50 and 10,000 x 10,000 pixels. <br> - For .pdf files, dimensions must be at most 11 x 17 inches, corresponding to Legal or A3 paper sizes and smaller. <br> - The total size of the training data is 500 pages or less.<br>Supports languages for both [handwritten text](/azure/ai-services/computer-vision/language-support#handwritten-text) and [print text](/azure/ai-services/computer-vision/language-support#print-text). |
| ![Globe symbol.](/office/media/icons/globe-internet.png)  | **Multi-Geo environments** <br>When setting up Syntex in a [Microsoft 365 Multi-Geo](/microsoft-365/enterprise/microsoft-365-multi-geo) environment, you can only configure it to use the model type in the central location. If you want to use this model type in a satellite location, contact Microsoft support. |
| ![Objects symbol.](/office/media/icons/objects-blue.png)  | **Multi-model libraries** <br>If two or more trained models are applied to the same library, the file is classified using the model that has the highest average confidence score. The extracted entities will be from the applied model only. |

### Simple document processing

| Icon          | Description   |
| ------------- | ------------- |
| ![Files symbol.](/office/media/icons/files-blue.png)  | **Supported file types** <br>This model supports the following file types: .bmp, .jpeg, .pdf, .png, and .tiff. |
| ![Conversation symbol.](/office/media/icons/chat-room-conversation-blue.png)  | **Supported languages** <br>This model supports documents in more than 100 languages. |
| ![Paragraph symbol.](/office/media/icons/paragraph-writing-blue.png)  | **OCR considerations** <br>This model uses optical character recognition (OCR) technology to scan .pdf files, image files, and .tiff files. OCR processing works best on documents that meet the following requirements: <br> - File format of .jpg, .png, or .pdf (text or scanned). Text-embedded .pdf files are better, because there won't be any errors in character extraction and location. <br> - For .pdf and .tiff files, up to 2,000 pages can be processed. <br> - The file size must be less than 50 MB. <br> -  For images, dimensions must be between 50 x 50 and 10,000 x 10,000 pixels. <br> - For .pdf files, dimensions must be at most 11 x 17 inches, corresponding to Legal or A3 paper sizes and smaller. <br> - The total size of the training data is 500 pages or less. |
| ![Globe symbol.](/office/media/icons/globe-internet.png)  | **Multi-Geo environments** <br>When setting up Syntex in a [Microsoft 365 Multi-Geo](/microsoft-365/enterprise/microsoft-365-multi-geo) environment, you can only configure it to use the model type in the central location. If you want to use this model type in a satellite location, contact Microsoft support. |
| ![Objects symbol.](/office/media/icons/objects-blue.png)  | **Multi-model libraries** <br>If two or more trained models are applied to the same library, the file is classified using the model that has the highest average confidence score. The extracted entities will be from the applied model only. |


## Structured and freeform document processing

- [Freeform document processing](#freeform-document-processing)
- [Structured document processing](#structured-document-processing)

### Freeform document processing

| Icon          | Description   |
| ------------- | ------------- |
| ![Files symbol.](/office/media/icons/files-blue.png)  | **Supported file types** <br>This model supports the following file types: see [file type requirements](/ai-builder/form-processing-model-requirements#requirements). |
| ![Conversation symbol.](/office/media/icons/chat-room-conversation-blue.png)  | **Supported languages** <br>This model supports the following languages: see [Model for General documents](/ai-builder/form-processing-model-requirements#model-for-general-documents). |
| ![Paragraph symbol.](/office/media/icons/paragraph-writing-blue.png) | **OCR considerations** <br>This model uses optical character recognition (OCR) technology to scan .pdf files, image files, and .tiff files. OCR processing works best on documents that meet [these requirements](/ai-builder/form-processing-model-requirements#requirements). |
| ![Bandwidth/efficiency symbol.](/office/media/icons/bandwidth-efficiency-blue.png)  | **Optimization tips** <br>If your model isn't performing as you want it to, try [these steps to improve the performance of your model](/ai-builder/improve-form-processing-performance). |
| ![Globe symbol.](/office/media/icons/globe-internet.png)  | **Multi-Geo environments** <br>When setting up Syntex in a [Microsoft 365 Multi-Geo](/microsoft-365/enterprise/microsoft-365-multi-geo) environment, you can only configure it to use the model type in the central location. If you want to use this model type in a satellite location, contact Microsoft support. |
| ![Blocks symbol.](/office/media/icons/blocks-blue.png)  | **Custom Power Platform environments** <br>If you use a custom environment (rather than the default environment) for Power Platform processing, there are additional setup requirements. For more information, see [Custom Power Platform environments](/microsoft-365/contentunderstanding/set-up-content-understanding#custom-power-platform-environments). |
| ![Objects symbol.](/office/media/icons/objects-blue.png)  | **Multi-model libraries** <br>If two or more trained models are applied to the same library, the file is classified using the model that has the highest average confidence score. The extracted entities will be from the applied model only. You can have only one freeform or one structured model per library. |

### Structured document processing

| Icon          | Description   |
| ------------- | ------------- |
| ![Files symbol.](/office/media/icons/files-blue.png)  | **Supported file types** <br>This model supports the following file types: see [file type requirements](/ai-builder/form-processing-model-requirements#requirements). |
| ![Conversation symbol.](/office/media/icons/chat-room-conversation-blue.png)  | **Supported languages** <br>This model supports the following languages: see [Model for Fixed-template documents](/ai-builder/form-processing-model-requirements#model-for-fixed-template-documents). |
| ![Paragraph symbol.](/office/media/icons/paragraph-writing-blue.png) | **OCR considerations** <br>This model uses optical character recognition (OCR) technology to scan .pdf files, image files, and .tiff files. OCR processing works best on documents that meet [these requirements](/ai-builder/form-processing-model-requirements#requirements). |
| ![Bandwidth/efficiency symbol.](/office/media/icons/bandwidth-efficiency-blue.png)  | **Optimization tips** <br>If your model isn't performing as you want it to, try [these steps to improve the performance of your model](/ai-builder/improve-form-processing-performance). |
| ![Globe symbol.](/office/media/icons/globe-internet.png)  | **Multi-Geo environments** <br>When setting up Syntex in a [Microsoft 365 Multi-Geo](/microsoft-365/enterprise/microsoft-365-multi-geo) environment, you can only configure it to use the model type in the central location. If you want to use this model type in a satellite location, contact Microsoft support. |
| ![Blocks symbol.](/office/media/icons/blocks-blue.png)  | **Custom Power Platform environments** <br>If you use a custom environment (rather than the default environment) for Power Platform processing, there are additional setup requirements. For more information, see [Custom Power Platform environments](/microsoft-365/contentunderstanding/set-up-content-understanding#custom-power-platform-environments). |
| ![Objects symbol.](/office/media/icons/objects-blue.png)  | **Multi-model libraries** <br>If two or more trained models are applied to the same library, the file is classified using the model that has the highest average confidence score. The extracted entities will be from the applied model only. You can have only one freeform or one structured model per library. |

## Unstructured document processing

| Icon          | Description   |
| ------------- | ------------- |
| ![Files symbol.](/office/media/icons/files-blue.png)  | **Supported file types** <br>This model supports the following file types: .csv, .doc, .docx, .eml, .heic, .heif, .htm, .html, .jpeg, .jpg, .md, .msg, .pdf, .png, .ppt, .pptx, .rtf, .tif, .tiff, .txt, .xls, and .xlsx ( formulas in .xls and .xlsx files are not run).|
| ![Conversation symbol.](/office/media/icons/chat-room-conversation-blue.png)  | **Supported languages** <br>This model supports all of the Latin-based languages, including: English, French, German, Italian, and Spanish. |
| ![Paragraph symbol.](/office/media/icons/paragraph-writing-blue.png)  | **OCR considerations** <br>This model uses optical character recognition (OCR) technology to scan .pdf files, image files, and .tiff files. OCR processing works best on documents that meet the following requirements: <br> - File format of .jpg, .png, or .pdf (text or scanned). Text-embedded .pdf files are better, because there won't be any errors in character extraction and location. <br> - If your .pdf files are password-locked, you must remove the lock before submitting them. <br> - The combined file size of the documents used for training per collection must not exceed 50 MB, and PDF documents shouldn't have more than 500 pages. <br> - For images, dimensions must be between 50 x 50 and 10,000 x 10,000 pixels. Images that are very wide or have odd dimensions (for example, floor plans) might get truncated in the OCR process and lose accuracy. <br> - For .pdf files, dimensions must be at most 11 x 17 inches, corresponding to Legal or A3 paper sizes and smaller. <br> - If scanned from paper documents, scans should be high-quality images. <br> - Must use the Latin alphabet (English characters). <br> Note the following differences about Microsoft Office text-based files and OCR-scanned files (.pdf, image, or .tiff): <br> - All files: Truncated at 64,000 characters (in training and when run against files in a document library). <br> - OCR-scanned files: There's a 500-page limit. Only PDF and image file types are processed by OCR. |
| ![Globe symbol.](/office/media/icons/globe-internet.png)  | **Multi-Geo environments** <br>When setting up Syntex in a [Microsoft 365 Multi-Geo](/microsoft-365/enterprise/microsoft-365-multi-geo) environment, you can only configure it to use the model type in the central location. If you want to use this model type in a satellite location, contact Microsoft support. |
| ![Objects symbol.](/office/media/icons/objects-blue.png)  | **Multi-model libraries** <br>If two or more trained models are applied to the same library, the file is classified using the model that has the highest average confidence score. The extracted entities will be from the applied model only. |
