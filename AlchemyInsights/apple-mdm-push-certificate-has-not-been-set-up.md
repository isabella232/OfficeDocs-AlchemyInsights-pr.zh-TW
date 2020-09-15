---
title: 未設定 Apple MDM 推播憑證
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5f95c9bee29db44a4153e0de0b8f6fb49b274920
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716848"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>未設定 Apple MDM 推播憑證

您的訂閱尚未設定 Apple MDM 推播憑證 (又稱為 Apple 推播通知服務 (APN) 憑證)。 如果沒有設定 Apple MDM 推播憑證，您將無法註冊及管理 iOS 和 Mac OS 裝置。 將憑證新增至 Intune 之後，使用者就可以安裝公司入口網站應用程式來註冊其 iOS 裝置。

1. 選取 **[我同意]**。 允許 Microsoft 將資料傳送到 Apple。

2. 選取 Intune 憑證登入請求必要的 **[下載您的 CSR]** 以創建 Apple MDM 推播憑證。 該檔案用於從 Apple 推播憑證入口網站請求信任關係憑證。

3. 選取 **[建立您的 MDM 推播憑證]** 以移至 Apple 推播憑證入口網站。 使用您公司的 Apple ID 登入，然後選取**建立憑證**。 選取 **[選擇檔案]**，然後流覽至憑證簽署要求檔案，然後選擇 **[上傳]**。 在 [確認] 頁面上，選擇 **[下載]** 下載憑證 (.pem) 檔案，並將檔案儲存在本機。
 
**附註**：該憑證與建立它時使用的 Apple ID 相關聯。 最佳做法是使用公司 Apple ID 執行管理工作，並確認信箱由多人或使用通訊群組清單監視。 請勿使用個人 Apple ID。 每12個月使用相同的 Apple ID 續約 Apple 推播憑證。
 
4. 輸入建立 Apple MDM 推播憑證時使用的 Apple ID。 當您需要續約憑證時，請將此 ID 記錄為提醒。

5. 移至憑證 (.pem) 檔案，選取 **[開啟]**，然後選擇 **[上傳]**。 使用推播憑證，Intune 就能註冊及管理 Apple 裝置。