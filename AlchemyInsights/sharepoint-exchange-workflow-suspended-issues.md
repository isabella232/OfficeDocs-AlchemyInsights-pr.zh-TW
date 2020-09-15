---
title: 線上開始使用 SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700698"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="fe678-102">SharePoint 中的工作流程</span><span class="sxs-lookup"><span data-stu-id="fe678-102">Workflows in SharePoint</span></span>

<span data-ttu-id="fe678-103">如果 SharePoint 的工作流程未傳送電子郵件，則您的組織可能發生 Exchange Online 寄件者限制。</span><span class="sxs-lookup"><span data-stu-id="fe678-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="fe678-104">如果您有下列其中一個專案，則可能會出現「工作流程已擱置」錯誤訊息：</span><span class="sxs-lookup"><span data-stu-id="fe678-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="fe678-105">您在使用 SharePoint 2010 或 SharePoint 2013 工作流程平臺類型的 SharePoint Online 中有工作流程。</span><span class="sxs-lookup"><span data-stu-id="fe678-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="fe678-106">工作流程設定為一次傳送自訂的電子郵件訊息給超過200位使用者、每天超過10000個收件者，或每分鐘超過30封郵件。</span><span class="sxs-lookup"><span data-stu-id="fe678-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="fe678-107">當您執行工作流程時，未傳送電子郵件訊息，您會注意到錯誤訊息，內部狀態是設定為 [已擱置]，或顯示 [無法傳送給收件者]。</span><span class="sxs-lookup"><span data-stu-id="fe678-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="fe678-108">如需詳細資訊，請參閱下列 [文章](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)。</span><span class="sxs-lookup"><span data-stu-id="fe678-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

