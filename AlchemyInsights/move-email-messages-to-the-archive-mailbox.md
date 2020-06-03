---
title: 將電子郵件訊息移至封存信箱
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511031"
---
# <a name="move-email-to-the-archive-mailbox"></a>將電子郵件移至封存信箱

1. 確認已啟用封存**信箱**。 如果不是，請使用[本文](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)中的步驟來啟用封存信箱。

2. 若要將郵件自動封存到封存信箱，必須將具有 [**移至**封存] 動作的保留標記設定為 [**自動套用至整個信箱（預設）] 標記**。 使用這裡的步驟來建立標記：封存[預設](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)標籤。

3. 接下來，將**Archive**封存標籤新增至保留原則。 在 Exchange 系統管理中心中，選擇 [**保留原則**] > 將 [**移至**封存] 標記新增至原則 >**儲存**]。

4. 現在[將保留原則指派](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)給特定使用者的信箱。 相同的原則會同時套用至**主要**和**封存信箱。**

您可能需要強制受管理的資料夾助理（MFA）執行，並將新的設定套用至使用者的信箱。 在[連線至 EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)時執行下列命令，以啟動特定信箱的受管理的資料夾助理：
  
Start-ManagedFolderAssistant 身分識別<name of the mailbox>

如需設定封存原則的詳細資訊，請參閱[設定信箱的封存和刪除原則](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)。
  