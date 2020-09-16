---
title: 在 SharePoint 或 OneDrive 中限制存取權
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: cc6f93ba8ae3a030f83da5eca2d28dcf38f0f8f7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47800887"
---
# <a name="irm-protection-to-sharepoint-files"></a><span data-ttu-id="76a11-102">SharePoint 檔案的 IRM 保護</span><span class="sxs-lookup"><span data-stu-id="76a11-102">IRM Protection to SharePoint files</span></span>


<span data-ttu-id="76a11-103">在 SharePoint Online 中，IRM 保護會套用至清單和文件庫層級的檔案。</span><span class="sxs-lookup"><span data-stu-id="76a11-103">Within SharePoint Online, IRM protection is applied to files at the list and library level.</span></span> <span data-ttu-id="76a11-104">您的組織在使用 IRM 保護之前，必須先設定 Rights Management。</span><span class="sxs-lookup"><span data-stu-id="76a11-104">Before your organization can use IRM protection, you must first set up Rights Management.</span></span> <span data-ttu-id="76a11-105">IRM 依賴 azure Rights Management service 從 Azure 資訊保護來加密及指派使用限制。</span><span class="sxs-lookup"><span data-stu-id="76a11-105">IRM relies on the Azure Rights Management service from Azure Information Protection to encrypt and assign usage restrictions.</span></span> <span data-ttu-id="76a11-106">有些 Microsoft 365 訂閱包含 Azure 版權管理，但並非全部。</span><span class="sxs-lookup"><span data-stu-id="76a11-106">Some Microsoft 365 subscriptions include Azure Rights Management, but not all.</span></span> 

<span data-ttu-id="76a11-107">若要深入了解，請參閱：</span><span class="sxs-lookup"><span data-stu-id="76a11-107">To learn more, see:</span></span>

- <span data-ttu-id="76a11-108">[Office 應用程式和服務如何支援 Azure 版權管理](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support)。</span><span class="sxs-lookup"><span data-stu-id="76a11-108">[How Office applications and services support Azure Rights Management](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span></span>

- <span data-ttu-id="76a11-109">[在 SharePoint 系統管理中心中設定資訊版權管理 (IRM) ](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center)。</span><span class="sxs-lookup"><span data-stu-id="76a11-109">[Set up Information Rights Management (IRM) in SharePoint admin center](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center).</span></span>

- <span data-ttu-id="76a11-110">[IRM-啟用 SharePoint 文件庫和清單](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists)。</span><span class="sxs-lookup"><span data-stu-id="76a11-110">[IRM-enable SharePoint document libraries and lists](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span></span>

- <span data-ttu-id="76a11-111">[Office 中的資訊版權管理](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c)。</span><span class="sxs-lookup"><span data-stu-id="76a11-111">[Information Rights Management in Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span></span>

- <span data-ttu-id="76a11-112">[Exchange Online 中的資訊版權管理](https://docs.microsoft.com/microsoft-365/compliance/information-rights-management-in-exchange-online)。</span><span class="sxs-lookup"><span data-stu-id="76a11-112">[Information Rights Management in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/information-rights-management-in-exchange-online).</span></span>


