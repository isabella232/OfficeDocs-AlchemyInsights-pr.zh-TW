---
title: 解決未經許可的產品錯誤
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
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737944"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>解決「未經許可的產品」錯誤的建議

若要解決「未經許可的產品」的錯誤，請嘗試下列步驟：

- 查看您的訂閱狀態是否已過期。
- 請確定您有允許用戶端授權的訂閱，例如 Microsoft 365 應用程式的商務用帳戶或商務版，並 [確保使用者已指派授權](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)。 
- 請確定使用者正在使用已指派授權的相同帳戶登入 Office。
- 檢查 [ [服務健康](https://docs.microsoft.com/office365/enterprise/view-service-health) 情況] 頁面，查看服務是否有任何已知的問題。
- 檢查您的防火牆、防毒軟體及 proxy 設定，以確認他們不會封鎖 Microsoft 365 應用程式對網際網路的存取。 請參閱 [URLs 及 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。

您也可以嘗試下列疑難排解動作： 

- 開啟 Office 應用程式， [並登出](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) 任何現有的使用者帳戶。 [移除](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) 並 [重新指派](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) office 授權，然後使用受影響的使用者帳戶登 [入 office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) 。
- 執行 [啟動疑難排解](https://aka.ms/SARA-OfficeActivation-Alchemy)程式。
- [重設 Office 啟用狀態](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)。 
- [執行 Office 的線上修復](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)。

如需其他疑難排解解決方案，請參閱： 

- [Office 中的「未授權產品」及啟用錯誤](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [啟用 Office 時，「很抱歉，我們無法連線至您的帳戶。請稍後再試一次」的錯誤](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365) (英文)