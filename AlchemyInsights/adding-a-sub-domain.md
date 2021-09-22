---
title: 加入子域
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
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/22/2021
ms.locfileid: "59475937"
---
# <a name="adding-a-sub-domain"></a>加入子域

子域可以新增至與父項網域相同或不同的承租人。 在這兩種情況下，您必須在註冊機構網站上管理自己的 DNS 設定。 如果您已讓 Microsoft 使用 NS 記錄來管理您的 DNS 設定，或者您購買的是 Microsoft 的網域，您就無法新增子域，除非先變更此值。

請先新增上層網域，然後再新增子網域。 如果子域位於相同租使用者，則不需要進行其他驗證。 若要將子系新增至不同的租使用者，必須先進行擁有權驗證的 DNS txt 記錄，再新增網域以及所選取服務的其他 DNS 記錄。

- 若要新增網域或子域，請遵循 [[新增網域] 嚮導](https://admin.microsoft.com/Adminportal#/Domains/Wizard)，或是手動新增網域或子域，方法是 **移至 [**  >  **網域**] [  >  **新增網域**]。

必要時：

- 若要變更管理現有網域之 DNS 設定的人員，請移至 **設定**  >  [**網域**](https://admin.microsoft.com/Adminportal/Home#/Domains)]，選取網域旁的核取方塊，然後選取 [**管理 DNS**]。 在嚮導中，選取 [ **新增您自己的 DNS 記錄** ]，然後完成該嚮導。
- 若要將子域新增至 Microsoft 購買的網域，請先將網域轉接至另一個註冊機構，然後進行上述變更，以管理您自己的 DNS 記錄。 如需相關指示，請參閱將 [網域從 Microsoft 轉接至其他主機](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)。
- 如果您收到的錯誤是您的組織中的其他成員或人員已使用您的網域，則在使用網域之前，您必須先接管此非管理帳戶。 如需相關指示，請參閱[在 Azure Active Directory 中以系統管理員身分使用非受管理的目錄](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover)。
