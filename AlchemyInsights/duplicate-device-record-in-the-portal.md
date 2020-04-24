---
title: 入口網站中的重複裝置記錄
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789589"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="f05f0-102">入口網站中的重複裝置記錄</span><span class="sxs-lookup"><span data-stu-id="f05f0-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="f05f0-103">如果裝置未正確將共同管理狀回報給 Configuration Manager 網站，您可能會在入口網站看到 2 筆裝置記錄。</span><span class="sxs-lookup"><span data-stu-id="f05f0-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="f05f0-104">若要檢查裝置的共同管理狀態，請在 Configuration Manager 主控台中查看該裝置 [Co-managed]\*\*\*\* 欄。</span><span class="sxs-lookup"><span data-stu-id="f05f0-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="f05f0-105">如果看不到該欄，您可以直接以滑鼠右鍵按一下任一欄標題，然後從清單中選取來新增欄。</span><span class="sxs-lookup"><span data-stu-id="f05f0-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="f05f0-106">Co-managed 值必須為 [是]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="f05f0-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="f05f0-107">如果該值是 [否]\*\*\*\*，請在用戶端裝置上開啟 Configuration Manager 用戶端小程式，然後在 [一般] 索引標籤中核取 **Co-management** 屬性。</span><span class="sxs-lookup"><span data-stu-id="f05f0-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="f05f0-108">如果此值為 [已啟用]\*\*\*\*，表示問題出在用戶端與管理點間的通訊。</span><span class="sxs-lookup"><span data-stu-id="f05f0-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="f05f0-109">請查看裝置上的 **CcmMessaging.log**，以調查可能的連線問題。</span><span class="sxs-lookup"><span data-stu-id="f05f0-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="f05f0-110">如果值為 [已停用]\*\*\*\* 且裝置已在 Intune 中註冊，請查看裝置上的 **CoManagementHandler.log**，以確保裝置收到共同管理原則。</span><span class="sxs-lookup"><span data-stu-id="f05f0-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
