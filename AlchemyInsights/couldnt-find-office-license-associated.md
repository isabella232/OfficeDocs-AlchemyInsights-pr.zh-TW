---
title: 修正 Microsoft 365 應用程式無法找到與 office 授權相關聯的郵件
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747686"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>修正 Microsoft 365 應用程式「找不到相關聯的 office 授權」訊息

如果您收到這封郵件，請嘗試下列步驟：

1. 檢查您的防火牆、防毒軟體及 proxy 設定，以確認他們不會封鎖對 Microsoft 365 應用程式的網際網路存取。 請參閱 [Microsoft 365 URLs 和 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。
2. 移除並 [重新指派受影響使用者的 Office 授權](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) 。 
3. 開啟 Office 應用程式， [並登出](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) 任何現有的使用者帳戶。
4. 移至 Windows 設定 >**帳戶**  >  **電子郵件 & 帳戶**，並移除所有的工作帳戶（受影響的帳戶除外）。
5. 移至 Windows 設定 >**帳戶**  >  **存取工作或學校**，並中斷所有工作帳戶（受影響的帳戶除外）的連線。
6. 重設 Office 啟用狀態。 [Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. 使用受影響的使用者帳戶登[入](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)。

如需其他疑難排解解決方案，請參閱 [Office 中的未經許可產品和啟用錯誤](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)。