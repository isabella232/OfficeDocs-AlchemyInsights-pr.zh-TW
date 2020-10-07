---
title: 將電子郵件傳遞問題修正至擁有郵件功能的公用資料夾
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366455"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>將電子郵件傳遞問題修正至擁有郵件功能的公用資料夾

如果外部寄件者無法將郵件傳送到擁有郵件功能的公用資料夾，且寄件者收到錯誤： **無法找到 (550 5.4.1) **，請確認公用資料夾的電子郵件網域已設定為內部轉送網域，而不是授權網域：

1. [ (EAC) 開啟 Exchange 系統管理中心](https://docs.microsoft.com/Exchange/exchange-admin-center)。

2. 移至 [ **郵件流程**] \> [公認的 **網域**]，選取公認的網域，然後按一下 [ **編輯**]。

3. 在開啟的 [屬性] 頁面中，如果網欄位型別設定為 [ **授權**]，請將值變更為 [ **內部轉送** ]，然後按一下 [ **儲存**]。

如果外部寄件者收到錯誤 **您沒有許可權 (550 5.7.13) **，請在 [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) 中執行下列命令，以查看公用資料夾中匿名使用者的許可權：

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` 例如， `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` 。

若要允許外部使用者將電子郵件傳送至此公用資料夾，請將 CreateItems 存取權新增給匿名使用者。 例如，`Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`。
