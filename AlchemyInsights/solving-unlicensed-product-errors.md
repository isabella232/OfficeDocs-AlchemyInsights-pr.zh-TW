---
title: 解決未經許可的產品錯誤
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
- "3412"
- "9001428"
ms.openlocfilehash: 7922a2c5306f9d16856502b5e57e585cb90f2f7c9abaad0366f72ed46de786d5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957091"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>解決「未經許可的產品」錯誤的建議

若要解決「未經許可的產品」的錯誤，請嘗試下列步驟：

- 查看您的訂閱狀態是否已過期。
- 請確定您有允許用戶端授權（如 Microsoft 365 Apps 商務版或商務進階版）的訂閱，並[確認使用者已指派授權](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)。 
- 請確定使用者已使用指派授權的相同帳戶登入 Office。
- 檢查 [ [服務健康](https://docs.microsoft.com/office365/enterprise/view-service-health) 情況] 頁面，查看服務是否有任何已知的問題。
- 檢查您的防火牆、防毒軟體及 proxy 設定，以確認其不會封鎖 Microsoft 365 應用程式對網際網路的存取。 請參閱 [URLs 及 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。

您也可以嘗試下列疑難排解動作： 

- 開啟[Office 應用程式並登出任何現有的使用者](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)帳戶。 [移除](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users)並[重新指派](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)Office 授權，然後使用受影響的使用者帳戶登[入 Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) 。
- 執行 [啟動疑難排解](https://aka.ms/SARA-OfficeActivation-Alchemy)程式。
- [重設 Office 啟用狀態](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)。 
- [對 Office 執行線上修復](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)。

如需其他疑難排解解決方案，請參閱： 

- [Office 中的「未授權產品」及啟用錯誤](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [啟用 Office 時，「很抱歉，我們無法連線至您的帳戶。請稍後再試一次」的錯誤](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365) (英文)