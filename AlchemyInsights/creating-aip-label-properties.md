---
title: 建立 AIP 標籤原則
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/03/2020
ms.locfileid: "44542100"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="73dee-102">建立 AIP 標籤原則</span><span class="sxs-lookup"><span data-stu-id="73dee-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="73dee-103">Azure 資訊保護（AIP）標籤可以搭配組織通常建立及儲存的完整資料範圍（從最小的個人資料分類到最高的機密資料分類）使用。</span><span class="sxs-lookup"><span data-stu-id="73dee-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="73dee-104">Azure 資訊保護原則適用于 Azure 資訊保護（AIP）經典用戶端，不是[AIP 的整合標籤用戶端](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)。</span><span class="sxs-lookup"><span data-stu-id="73dee-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="73dee-105">您可以在 AIP 原則中設定多個元素，包括如下選項：</span><span class="sxs-lookup"><span data-stu-id="73dee-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="73dee-106">選項，可讓系統管理員或使用者分類及保護（選用）檔和電子郵件</span><span class="sxs-lookup"><span data-stu-id="73dee-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="73dee-107">當使用者儲存檔並傳送電子郵件時強制進行分類的選項</span><span class="sxs-lookup"><span data-stu-id="73dee-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="73dee-108">選項可根據其附件自動標記電子郵件。</span><span class="sxs-lookup"><span data-stu-id="73dee-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="73dee-109">控制是否要在 Office 應用程式中顯示資訊保護列的選項</span><span class="sxs-lookup"><span data-stu-id="73dee-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="73dee-110">如需 Azure 資訊保護原則的其他選項和資訊，請參閱： [Azure 資訊保護原則的概述](https://docs.microsoft.com/azure/information-protection/overview-policy)。</span><span class="sxs-lookup"><span data-stu-id="73dee-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="73dee-111">如需有關 AIP 原則的其他有用資源，請參閱：</span><span class="sxs-lookup"><span data-stu-id="73dee-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="73dee-112">教程：設定 Azure 資訊保護原則設定及建立新標籤</span><span class="sxs-lookup"><span data-stu-id="73dee-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="73dee-113">設定 Azure 資訊保護原則</span><span class="sxs-lookup"><span data-stu-id="73dee-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="73dee-114">建立及設定敏感度標籤及其原則</span><span class="sxs-lookup"><span data-stu-id="73dee-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="73dee-115">使用 Azure 資訊保護的常見案例的操作方法指南</span><span class="sxs-lookup"><span data-stu-id="73dee-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="73dee-116">複查 Azure 資訊保護檔</span><span class="sxs-lookup"><span data-stu-id="73dee-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="73dee-117">Azure 資訊保護的需求</span><span class="sxs-lookup"><span data-stu-id="73dee-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="73dee-118">Azure 資訊保護的快速入門教程</span><span class="sxs-lookup"><span data-stu-id="73dee-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="73dee-119">下載 Azure 資訊保護用戶端</span><span class="sxs-lookup"><span data-stu-id="73dee-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)