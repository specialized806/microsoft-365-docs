---
title: Microsoft 365 admin center features that configure Microsoft 365 Copilot
description: Learn about some of the Microsoft 365 Copilot features IT admins can configure in the Microsoft 365 admin center.
f1.keywords:
- NOCSH
ms.author: camillepack
author: camillepack
manager: scotv
ms.date: 01/30/2025
ms.reviewer: elvaf
audience: Admin
ms.topic: how-to
ms.service: microsoft-365-copilot
ms.localizationpriority: medium
ms.collection: 
- scotvorg
- m365copilot
- magic-ai-copilot
appliesto:
  - ✅ Microsoft 365 Copilot
---

# Admins can manage some Microsoft 365 Copilot features in the Microsoft 365 admin center

When Microsoft 365 Copilot is available in a tenant, there are some Copilot features that admins can configure in the Microsoft 365 admin center.

The admin center also gives shortcuts to other features that can affect how Copilot is used in your organization, like the Power Platform pay-as-you-go plan, and Copilot Chat in Bing, Edge, and Windows.

This article is for IT administrators, and lists some of the Copilot features you can control in the Microsoft 365 admin center.

> [!NOTE]
> If you're an end user on a work device, then it's possible your IT admin group turned on Copilot for you. The [Copilot Prompt Gallery](https://copilot.cloud.microsoft/prompts) can help you get started.
>
> If you're an end user on a Windows personal device, then you might automatically get Microsoft Copilot, which is the free consumer version. To learn how Copilot can help you, see [How can Copilot help you?](https://www.microsoft.com/microsoft-copilot/for-individuals).

This article applies to:

- Microsoft 365 Copilot

## Before you begin

- The Copilot experience in the Microsoft 365 admin center depends on the Copilot license you have.

  If your organization has a Microsoft 365 Copilot license, then you see settings that can manage some Microsoft 365 Copilot features. If your organization doesn't have a Copilot license, then the features you see are for Microsoft Copilot, which is the consumer version of Copilot.

  For more information, see:

  - [Which Copilot is right for your organization?](which-copilot-for-your-organization.md)
  - [Get started with Microsoft 365 Copilot](microsoft-365-copilot-setup.md)

- Any admin role can access the Copilot page, but only certain roles can change the settings. To make changes to Copilot features in the Microsoft 365 admin center, sign in with one of the following accounts:

  - AI Administrator
  - ??

  ??Which roles can see everyting but not change anything??
  ??Which roles can change everything??
  ?? List minimum role for each feature??

  To learn more about the different roles, and what they can do, see [About admin roles in the Microsoft 365 admin center](/microsoft-365/admin/add-users/about-admin-roles).

- This article lists more features than what you might see. Some features might not be shown to your account. If you want to see all the available features, then sign in with one of the following accounts:

  - AI Administrator
  - ??

  For features that link to other admin centers, you need the appropriate role to access those admin centers.

  To learn more about the different roles, and what they can do, see [About admin roles in the Microsoft 365 admin center](/microsoft-365/admin/add-users/about-admin-roles).

- Microsoft 365 Copilot used with Microsoft Entra ID is governed by your agreement for Online Services. For more information, see the [Microsoft Online Services Terms](https://www.microsoft.com/licensing/docs/customeragreement).

- The Microsoft 365 admin center changes frequently. So the features in this article can be different than what you see in the Microsoft 365 admin center.

## Open the Copilot page

1. Sign in to the [Microsoft 365 admin center](https://admin.microsoft.com) as the AI Administrator. For more information on this role, see [About admin roles in the Microsoft 365 admin center](/microsoft-365/admin/add-users/about-admin-roles).

    ?? Ask Elva about minimum perms role to update settings? What is minimum perms role for viewing?

2. In the left navigation, select **Copilot**. You can select **Overview** and **Settings**:

    :::image type="content" source="media/microsoft-365-copilot-page/microsoft-365-admin-center-copilot-page.png" alt-text="Screenshot that shows the Overview and Settings options in the Copilot page in the Microsoft 365 admin center." lightbox="media/microsoft-365-copilot-page/microsoft-365-admin-center-copilot-page.png":::

## Features you can manage

This section lists some of the features shown in the Microsoft 365 admin center. Some features are configured in the admin center, while others are shortcuts to other admin centers.

### Reports and licenses

In the [Microsoft 365 admin center](https://admin.microsoft.com) > **Copilot** > **Overview** page, you can view reports and assign (or unassign) Copilot licenses. You can also view the number of active users and the number of licenses that are available.

This view lists some of the popular features that are available in Microsoft 365 Copilot. It also provides shortcuts to more in-depth settings in the admin center, like more usage reports (**Reports** > **Usage**) and license management (**Billing** > **Licenses**).

To learn more about these features, see:

- [Microsoft 365 reports in the admin center](/microsoft-365/admin/activity-reports/microsoft-365-copilot-usage)
- [Set up Microsoft 365 Copilot](microsoft-365-copilot-setup.md) and [Enable users for Microsoft 365 Copilot](microsoft-365-copilot-enable-users.md)

### Copilot agent consumption meter

✅ Shortcut to the Power Platform pay-as-you-go plan

In the [Microsoft 365 admin center](https://admin.microsoft.com) > **Copilot** > **Settings** page, select **Copilot agent consumption meter**.

In the admin center, this feature is a shortcut to the [Power Platform pay-as-you-go plan](/power-platform/admin/pay-as-you-go-overview). You don't configure this feature in the Microsoft 365 admin center.

This feature creates a billing plan that tracks and manages Microsoft 365 Copilot Chat consumption. When you set up a billing plan, you also select an Azure subscription, and link the necessary environments. This configuration helps manage message capacity, monitor usage, and handle overages, which can help with costs.

To learn more, see:

- [Learn more about the Power Platform pay-as-you-go plan](/power-platform/admin/pay-as-you-go-overview)
- [Set up a Power Platform pay-as-you-go plan](/power-platform/admin/pay-as-you-go-set-up)

### Copilot diagnostics logs

✅ Configure in the Microsoft 365 admin center

In the [Microsoft 365 admin center](https://admin.microsoft.com) > **Copilot** > **Settings** page, select **Copilot diagnostics logs**.

When users have an issue and aren't able to send feedback logs to Microsoft, you can submit feedback logs on their behalf. The data include prompts and generated responses, relevant content samples, and additional log files. Using this feature to send feedback logs temporarily override any user level feedback policy.

??screen shot??

To learn more, see [Submit admin-initiated Copilot feedback from the Microsoft 365 admin center](provide-feedback.md).

??Requires Global Admin? Or is AI Admin enough??

### Copilot image generation

✅ Enable in the Microsoft 365 admin center

In the [Microsoft 365 admin center](https://admin.microsoft.com) > **Copilot** > **Settings** page, select **Copilot image generation**.

When this feature is allowed, end users can ask Copilot to create, design, and edit images. Users can add these images to their work.

:::image type="content" source="media/microsoft-365-copilot-page/microsoft-365-admin-center-copilot-image-generation.png" alt-text="Screenshot that allows admins to allow or prevent end users from creating images using Microsoft 365 Copilot in the Microsoft 365 admin center." :::

To learn more, see:

- [How to Create AI Art with Copilot](https://www.microsoft.com/microsoft-copilot/for-individuals/do-more-with-ai/ai-art-and-creativity/how-to-create-ai-art-with-copilot)
- [Data, Privacy, and Security for Microsoft 365 Copilot](microsoft-365-copilot-privacy.md)

### Copilot in Bing, Edge, and Windows

✅ Includes information about Copilot Chat that admins should know

In the [Microsoft 365 admin center](https://admin.microsoft.com) > **Copilot** > **Settings** page, select **Copilot in Bing, Edge, and Windows**.

This feature refers to AI-powered **Copilot Chat** and is automatically available to Bing, Edge, and Windows users. You don't configure this feature in the Microsoft 365 admin center. But, you should know that Copilot Chat for the web is available to everyone.

For organizations with a Microsoft 365 subscription, you get **Microsoft 365 Copilot Chat**. It gives your users internet-based chat and work-based chat with [enterprise data protection](/copilot/privacy-and-protections). Enterprise data protection applies to Copilot Chat prompts and responses when users sign in with a Microsoft Entra account, and is designed for work and education.

- To ensure that users in your organization access Copilot Chat, see [Manage Microsoft 365 Copilot Chat](/copilot/manage).

- To configure AI features for Copilot in Microsoft Edge, you can create a configuration profile and configure the settings in the profile. To learn more, see [Configure Copilot in Microsoft Edge with configuration profiles](/deployedge/microsoft-edge-management-service).

  ??Why is Edge separate??

- [Updated Windows and Microsoft 365 Copilot Chat experience)](/windows/client-management/manage-windows-copilot)

- ?? is there a config profile for Bing??

For users signed with a personal account, they can use Microsoft Copilot, which is the consumer version of Copilot Chat ([copilot.microsoft.com](https://copilot.microsoft.com/) and [bing.com/chat](https://bing.com/chat)).

To learn more, see:

- [Manage Copilot Chat](/copilot/manage)
- [Copilot Chat FAQ](/copilot/faq)
- [Which Copilot is right for your organization?](which-copilot-for-your-organization.md)

### Copilot in Teams meetings

✅ Shortcut to the Microsoft Teams admin center

In the [Microsoft 365 admin center](https://admin.microsoft.com) > **Copilot** > **Settings** page, select **Copilot in Bing, Edge, and Windows**.

This feature is a shortcut to the [Microsoft Teams admin center](https://admin.teams.microsoft.com). You don't configure this feature in the Microsoft 365 admin center.

In the Teams admin center, you can manage how Copilot interacts with some Teams features, including meeting transcripts.

To learn more, see:

- [Microsoft 365 Copilot in Teams meetings and events](/microsoftteams/copilot-teams-transcription)
- [Teams Rooms and Copilot overview](/microsoftteams/rooms/copilot-admin-mtr)

### Copilot in Viva

[Microsoft Viva](/viva/microsoft-viva-overview) is an integrated employee experience in Microsoft 365 and Microsoft Teams. It gives you the ability to support connection, insight, purpose, and growth in your organization.

There are several ways to use Copilot in Microsoft Viva:

- **Copilot in Viva Engage** provides conversation starters and writing assistance to help people create Engage posts. Use a combination of the org-wide setting and custom policies to refine access for the people in your organization.

  To learn more, see [Copilot in Viva Engage](/viva/copilot/viva-copilot-overview#copilot-in-viva-engage).

- **Copilot in Viva Goals** helps people brainstorm new goals, refine and improve existing ones, and summarize key information. Use a combination of the org-wide setting and custom policies to refine access for the people in your organization.

  To learn more, see [Copilot in Viva Goals](/viva/copilot/viva-copilot-overview#copilot-in-viva-goals).

- **Copilot in Viva Insights** simplifies the query building process for analysts by suggesting a template, metrics, filters, and attributes relevant to their analysis. Use a combination of org-wide setting and custom policies to refine access for the people in your organization.

  To learn more, see [Copilot queries in Viva Insights](/viva/insights/advanced/analyst/copilot-query).

  ?? Removed??

### Data, Security, and Compliance

✅ Shortcut to Microsoft Purview portal

In the [Microsoft 365 admin center](https://admin.microsoft.com) > **Copilot** > **Settings** page, select **Data, Security, and Compliance**.

This feature is a shortcut to the [Microsoft Purview portal](https://purview.microsoft.com/). You don't configure this feature in the Microsoft 365 admin center.

Microsoft Purview has several features that can help get your data ready for Copilot. You can create sensitivity labels and apply them to your data, create retention policies to remove outdated data, and analyze Copilot prompts and responses.

To learn more, see:

- [Protect and manage Microsoft 365 Copilot interactions with Microsoft Purview](/purview/ai-microsoft-purview)
- [Microsoft 365 Copilot admin guide for E3 + SAM licenses](microsoft-365-copilot-e3-guide.md)
- [Microsoft 365 Copilot admin guide for E5 + SAM licenses](microsoft-365-copilot-e5-guide.md)

### Extensions

✅ Configure in the Microsoft 365 admin center

In the [Microsoft 365 admin center](https://admin.microsoft.com) > **Copilot** > **Settings** page, select **Extensions**.

This setting lets you allow (or block) user access to [Copilot agents](https://support.microsoft.com/topic/introducing-copilot-agents-943e563d-602d-40fa-bdd1-dbc83f582466). It also provides a shortcut to more in-depth settings in the admin center (**Settings** > **Integrated apps**).

:::image type="content" source="media/microsoft-365-copilot-page/microsoft-365-admin-center-copilot-extensions.png" alt-text="Screenshot that lets you allow or block users from using Microsoft 365 Copilot extensions and agents in the Copilot page in the Microsoft 365 admin center.":::

Agents are focused interactions (chats and responses) with Microsoft 365 Copilot that focus on a specific task. You can create your own agents and include sample prompts that users can ask Copilot. For example, you can create agents that help users creat meeting agendas or write blog posts. End users can ask questions not related to the task, but agents are designed to help users with specific tasks.

You can also learn how to control the integration of non-Microsoft apps and first-party apps.

To learn more, see:

- [Manage Copilot agents in Integrated Apps](/microsoft-365/admin/manage/manage-copilot-agents-integrated-apps)
- [Introducing Copilot agents](https://support.microsoft.com/topic/introducing-copilot-agents-943e563d-602d-40fa-bdd1-dbc83f582466)

### Microsoft 365 Copilot self-service purchases

✅ Configure in the Microsoft 365 admin center

In the [Microsoft 365 admin center](https://admin.microsoft.com) > **Copilot** > **Settings** page, select **Microsoft 365 Copilot self-service purchases**.

This setting lets you allow (or block) users from purchasing Microsoft 365 Copilot licenses without admin approval or help. This feature can help admins understand and manage the demand.

:::image type="content" source="media/microsoft-365-copilot-page/microsoft-365-admin-center-copilot-self-service.png" alt-text="Screenshot that allows users to purchase Microsoft 365 Copilot without admin approval in the Copilot page in the Microsoft 365 admin center.":::

To see a list of all self-service trials and purchases in the [Microsoft 365 admin center](https://admin.microsoft.com), select **Home** > **Settings** > **Org settings**.

To learn more, see:

- [Self-service purchase FAQ](/microsoft-365/commerce/subscriptions/self-service-purchase-faq)
- [Use AllowSelfServicePurchase for the MSCommerce PowerShell module](/microsoft-365/commerce/subscriptions/allowselfservicepurchase-powershell)

### Pin Copilot Chat

✅ Configure in the Microsoft 365 admin center

In the [Microsoft 365 admin center](https://admin.microsoft.com) > **Copilot** > **Settings** page, select **Pin Copilot Chat**.

This setting lets you pin Microsoft 365 Copilot Chat to the navigation bar in Teams, Outlook and the Microsoft 365 Copilot app. Users with a Microsoft 365 Copilot license have it pinned by default.

:::image type="content" source="media/microsoft-365-copilot-page/microsoft-365-admin-center-pin-copilot-chat.png" alt-text="Screenshot that lets admins pin Microsoft 365 Copilot Chat to the navigation bar in the Copilot page in the Microsoft 365 admin center." lightbox="media/microsoft-365-copilot-page/microsoft-365-admin-center-pin-copilot-chat.png":::

When it's pineed, it makes it easier for people in your organization to access Copilot Chat.

To learn more, see:

- [Pin Microsoft 365 Copilot Chat to the navigation bar](pin-copilot.md)
- [Pin apps to the taskbar](/windows/configuration/taskbar/pinned-apps)

### Web search for Microsoft 365 Copilot and Microsoft Copilot

✅ Shortcut to create a cloud policy in the Microsoft 365 Apps admin center

In the [Microsoft 365 admin center](https://admin.microsoft.com) > **Copilot** > **Settings** page, select **Web search for Microsoft 365 Copilot and Microsoft Copilot**.

This feature is a shortcut to create a cloud policy in the Microsoft 365 Apps admin center. You don't configure this feature in the Microsoft 365 admin center.

When the **Allow web search in Copilot** policy is enabled, Copilot can reference web content to improve the quality of its responses.

To learn more, see:

- [Overview of Cloud Policy service for Microsoft 365](/microsoft-365-apps/admin-center/overview-cloud-policy)
- [Data, privacy, and security for web search in Microsoft 365 Copilot and Microsoft 365 Copilot Chat](manage-public-web-access.md)







### Microsoft Security Copilot

?? Removed??

✅ Shortcut to Microsoft Security Copilot

In the [Microsoft 365 admin center](https://admin.microsoft.com) > **Copilot** > **Settings** page, select **Microsoft Security Copilot**.

This feature is a shortcut to the Security Copilot portal to manage settings. You don't configure this feature in the Microsoft 365 admin center.

Security Copilot is a separate product and license from Microsoft 365 Copilot. If purchased, you can use this link to navigate to Security Copilot settings page.

To learn more, see [Security Copilot](/copilot/security).

### Copilot in Power Platform and Dynamics 365

?? Removed??

This links directs you to the Power Platform admin center to manage settings specific to Microsoft Copilot, agents, and Copilot agents in Power Platform and Dynamics 365 products.

To learn more, see [Copilot in Viva Edge](/power-platform/copilot).

## Related articles

- [About admin roles in the Microsoft 365 admin center](/microsoft-365/admin/add-users/about-admin-roles)
- [Microsoft 365 license feature comparison list for Microsoft 365 Copilot](microsoft-365-copilot-license-feature-overview.md)
- [Remove or prevent installation of the Copilot app](/windows/client-management/manage-windows-copilot#remove-or-prevent-installation-of-the-copilot-app)
