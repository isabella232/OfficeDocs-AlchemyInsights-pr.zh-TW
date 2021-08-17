---
title: 建立及管理裝置標籤
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: c06fbd377159e55cf34c79ef0aa1e34f0412a908e8d4e3dec5ad088c9b8b818a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898191"
---
# <a name="create-and-manage-device-tags-or-groups"></a>建立及管理裝置標籤

在裝置上新增標籤以建立邏輯群組關係。 裝置標籤支援網路的正確對應，使您能够附加不同的標籤以擷取内容，並作為事件的一部分啟用動態清單建立。 標籤可以用作裝置清單檢視中的篩檢，也可以用於對裝置進行分組。 有關裝置分組的詳細資訊，請參閱[建立和管理裝置標籤](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/machine-tags)。

可以使用以下方法在裝置上新增標籤：

- 使用入口網站

- 設定登錄機碼值
 
**注意：** 從將標籤新增到裝置的時間，到其在裝置清單和裝置頁中的顯示可用的時間，會有一些延遲。

要使用 API 新增裝置標籤，請參閲[新增或移除裝置標籤 API](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)。

## <a name="add-and-manage-device-tags-using-the-portal"></a>使用入口網站新增和管理裝置標籤

1. 選取要在其上管理標籤的裝置。 您可以從以下任何檢視中選取或搜尋裝置：

    - **安全性操作儀表板** - 從具有作用中警示的頂端裝置區段中選取裝置名稱。
    - **警示佇列** - 從警示佇列中選取裝置圖示旁邊的裝置名稱。
    - **裝置清單** - 從裝置清單中選取裝置名稱。
    - **搜尋方塊** - 從下拉式功能表中選取裝置並輸入裝置名稱。

    您還可以透過檔案和 IP 檢視存取警示頁。

1. 從回應動作列中選取 **管理標籤**。

1. 輸入以尋找或建立標籤。

新增至裝置檢視中的標籤，也會反映在裝置清單檢視中。 然後可以使用 [標籤] 篩選查看相關的裝置清單。

如需詳細資訊，請參閱，請參閱[建立和管理裝置標籤](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/machine-tags)。