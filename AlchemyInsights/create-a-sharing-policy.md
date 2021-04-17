---
title: 建立共用原則，以允許您的使用者與組織外部人員共用行事曆
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 016b915a9e8f7e32d5d393bc47347991866647c7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816263"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a>建立共用原則，以允許您的使用者與組織外部人員共用行事曆

1. 從 Microsoft 365 系統管理中心儀表板，移至 [系統管理]  >  [Exchange]。
2. 移至 [組織]  >  [共用]。
3. 在清單檢視的 [個人共用] 下，按一下 [新增]。
4. 在 [新增共用原則] 的 [原則名稱] 方塊中輸入共用原則的好記名稱。
5. 按一下 [新增] 來定義原則的共用規則。
6. 在 [共用規則] 中，選取下列其中一個選項來指定要與其共用的網域：
    - **與所有網域共用**
    - **與特定網域共用**
8. 如果您選取了 [與特定網域共用]，請輸入要共用的網域名稱。 如果您需要為此共用原則輸入多個網域，請儲存第一個網域的設定，然後編輯共用規則以新增其他網域。
9. 若要指定可以共用的資訊，請選取 [共用您的行事曆資料夾] 核取方塊，然後選取下列其中一個選項：
    - **只包含時間的行事曆空閒/忙碌資訊**
    - **包含時間、主旨和位置的行事曆空閒/忙碌資訊**
    - **所有的行事曆約會資訊，包括時間、主旨、位置和標題**
11. 按一下 [儲存] 設定共用原則的規則。
12. 如果要將此共用原則設定為組織中所有使用者的新預設共用原則，請選取 [將此原則設為預設共用原則] 核取方塊。
13. 按一下 [儲存] 建立共用原則。  

**如需深入了解本主題，請參閱：**

- [在 Exchange Online 中建立共用原則](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [將共用原則套用到 Exchange Online 中的信箱](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [修改、停用或移除 Exchange Online 中的共用原則](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)