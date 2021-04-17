---
title: 安裝 Power BI 報表伺服器
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1304"
- "2500001"
ms.openlocfilehash: 8479be2a538228b71033aca3907d3aba2f5e28fb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832085"
---
# <a name="install-power-bi-report-server"></a><span data-ttu-id="fda65-102">安裝 Power BI 報表伺服器</span><span class="sxs-lookup"><span data-stu-id="fda65-102">Install Power BI Report Server</span></span>

1. <span data-ttu-id="fda65-103">尋找 PowerBIReportServer.exe 的位置，然後啟動安裝程式。</span><span class="sxs-lookup"><span data-stu-id="fda65-103">Find the location of PowerBIReportServer.exe and launch the installer.</span></span>

2. <span data-ttu-id="fda65-104">選取 [ **安裝 POWER BI Report Server**]。</span><span class="sxs-lookup"><span data-stu-id="fda65-104">Select **Install Power BI Report Server**.</span></span>

3. <span data-ttu-id="fda65-105">選擇要安裝的版本，然後選取 **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="fda65-105">Choose an edition to install and then select **Next**.</span></span>

4. <span data-ttu-id="fda65-106">您可以從下拉式清單中選擇 [評估] 或 [開發人員] 版本。</span><span class="sxs-lookup"><span data-stu-id="fda65-106">You can choose either Evaluation or Developer edition from the drop down.</span></span>  <span data-ttu-id="fda65-107">否則，您可以輸入您從 Power BI 服務或大量授權服務中心取得之伺服器的產品金鑰。</span><span class="sxs-lookup"><span data-stu-id="fda65-107">Otherwise, you can enter a product key for the server that you acquired from either the Power BI service or the Volume License Service Center.</span></span> <span data-ttu-id="fda65-108">如需如何取得產品金鑰的詳細資訊，請參閱「開始之前」一節。</span><span class="sxs-lookup"><span data-stu-id="fda65-108">For more information about how to get your product key, see the Before you begin section.</span></span> <span data-ttu-id="fda65-109">閱讀並同意授權條款及條件，然後選取 **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="fda65-109">Read and agree to the license terms and conditions, and then select **Next**.</span></span>

5. <span data-ttu-id="fda65-110">您需要有可用的資料庫引擎來儲存報表伺服器資料庫。</span><span class="sxs-lookup"><span data-stu-id="fda65-110">You need to have a Database Engine available to store the report server database.</span></span> <span data-ttu-id="fda65-111">選取 **[下一步]** 只安裝報表服務器。</span><span class="sxs-lookup"><span data-stu-id="fda65-111">Select **Next** to install the report server only.</span></span>

6. <span data-ttu-id="fda65-112">指定報表伺服器的安裝位置。</span><span class="sxs-lookup"><span data-stu-id="fda65-112">Specify the install location for the report server.</span></span> <span data-ttu-id="fda65-113">選取 [ **安裝** ] 以繼續。</span><span class="sxs-lookup"><span data-stu-id="fda65-113">Select **Install** to continue.</span></span>

7. <span data-ttu-id="fda65-114">成功安裝之後，請選取 [ **設定報表伺服器** ] 以啟動 Reporting Services Configuration Manager。</span><span class="sxs-lookup"><span data-stu-id="fda65-114">After a successful setup, select **Configure Report Server** to launch the Reporting Services Configuration Manager.</span></span>

<span data-ttu-id="fda65-115">您不需要在安裝時提供 SQL Server 資料庫引擎伺服器。</span><span class="sxs-lookup"><span data-stu-id="fda65-115">You don't need a SQL Server Database Engine server available at the time of install.</span></span> <span data-ttu-id="fda65-116">安裝之後，您將需要一個設定 Reporting Services 的使用者。</span><span class="sxs-lookup"><span data-stu-id="fda65-116">You will need one to configure Reporting Services after install.</span></span>

<span data-ttu-id="fda65-117">如需詳細資訊： https://docs.microsoft.com/power-bi/report-server/install-report-server</span><span class="sxs-lookup"><span data-stu-id="fda65-117">For more information: https://docs.microsoft.com/power-bi/report-server/install-report-server</span></span>
