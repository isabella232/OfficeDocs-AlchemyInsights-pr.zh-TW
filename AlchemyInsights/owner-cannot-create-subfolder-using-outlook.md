---
title: 擁有者無法使用 Outlook 建立子資料夾
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/12/2020
ms.locfileid: "44716536"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="ea1f0-102">擁有者無法使用 Outlook 建立子資料夾</span><span class="sxs-lookup"><span data-stu-id="ea1f0-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="ea1f0-103">**公用資料夾擁有者使用 Outlook 建立子資料夾時發生一個持續存在的問題。我們將盡快修正此問題。**</span><span class="sxs-lookup"><span data-stu-id="ea1f0-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="ea1f0-104">在此同時，您可以使用下列因應措施：</span><span class="sxs-lookup"><span data-stu-id="ea1f0-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="ea1f0-105">使用 MAC 版 Outlook 建立子資料夾，因為這個問題只會影響電腦版 Windows 的 Outlook (所有版本)</span><span class="sxs-lookup"><span data-stu-id="ea1f0-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="ea1f0-106">讓系統管理員使用 EXO Shell 或 EAC 建立子資料夾</span><span class="sxs-lookup"><span data-stu-id="ea1f0-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="ea1f0-107">將使用者的 DefaultPublicFolderMailbox/EffectivePublicFolderMailbox 變更為造成問題之資料夾的內容信箱以外的其他信箱</span><span class="sxs-lookup"><span data-stu-id="ea1f0-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="ea1f0-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="ea1f0-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="ea1f0-109">等候一小時，重新啟動 outlook 用戶端</span><span class="sxs-lookup"><span data-stu-id="ea1f0-109">Wait for an hour, restart outlook client</span></span>