---
title: Microsoft 365 匯入服務中的磁碟機寄送
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
- "11514"
- "9003046"
ms.openlocfilehash: e524935c4600d4f043e39dc3c261eb21be97bfbaeb30dc1279676e2d5578ba4b
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888293"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a>Microsoft 365 匯入服務中的磁碟機寄送

使用磁碟機寄送的方式是透過複製 PST 至硬碟，然後運送硬碟至 Microsoft。

若要啟動此工具：

1. 在 [Microsoft 365 合規性中心] 的 **[資訊控管]** 底下，選取 **[匯入]**。

1. 選取 **選擇匯入工作類型**，然後選取 **下一步**。

1. 若要查看此匯入選項的步驟，請選取 **將硬碟寄送到我們的其中一個實體位置**。

以下是一些要記住的事項：

- 您必須在 Exchange Online 中獲指派信箱匯出角色，才能將 PST 檔案匯入 Microsoft 365 信箱。如果 PST 大於 20GB，效能可能會受到影響。

- 只支援 2.5 吋固態硬碟 (SSD)，或是 2.5 吋或 3.5 吋 SATA II/III 內接式硬碟。
包含 PST 檔案的硬碟必須使用 BitLocker 進行加密。

- 使用磁碟機寄送以將 PST 檔案匯入到 Microsoft 365 信箱的成本，是每 GB 的資料 $2 USD。

如需使用磁碟機寄送方式匯入 PST 的其他資訊，請參閱 [使用磁碟機寄送以匯入貴組織的 PST 檔案](https://docs.microsoft.com/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)。