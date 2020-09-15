---
title: 自動清除 Intune 中的過時裝置
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715012"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="e6e96-102">自動清除 Intune 中的過時裝置</span><span class="sxs-lookup"><span data-stu-id="e6e96-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="e6e96-103">Intune 允許管理員設定 90 到 270 天之間的時間間隔，在這之後，將從服務中删除過時裝置。</span><span class="sxs-lookup"><span data-stu-id="e6e96-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="e6e96-104">此設定適用全組織并會立即生效。</span><span class="sxs-lookup"><span data-stu-id="e6e96-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="e6e96-105">任何在超過設定的時間段內未簽入 Intune 服務器的裝置都將被永久删除。</span><span class="sxs-lookup"><span data-stu-id="e6e96-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="e6e96-106">**附註** 只有 MDM 裝置物件符合此清理動作的資格。</span><span class="sxs-lookup"><span data-stu-id="e6e96-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="e6e96-107">排除僅 EAS 裝置物件。</span><span class="sxs-lookup"><span data-stu-id="e6e96-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="e6e96-108">有關裝置何時符合刪除條件基於裝置的清理設定及其「狀態」的詳細資訊:</span><span class="sxs-lookup"><span data-stu-id="e6e96-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="e6e96-109">設定：**在上次簽入日期之後刪除裝置：是 (指定天數 (N) 值)**</span><span class="sxs-lookup"><span data-stu-id="e6e96-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="e6e96-110">根據設定中設定的值 (N)，Intune 服務會在上次成功簽入后的指定天數內刪除該裝置。</span><span class="sxs-lookup"><span data-stu-id="e6e96-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="e6e96-111">設定：**刪除上次簽入日期之後的裝置：否**</span><span class="sxs-lookup"><span data-stu-id="e6e96-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="e6e96-112">在裝置憑證過期且未續約 180 天之後，裝置就會被刪除。</span><span class="sxs-lookup"><span data-stu-id="e6e96-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="e6e96-113">**注意**，在這兩種情況下，裝置都必須成功在 Intune 上註冊。</span><span class="sxs-lookup"><span data-stu-id="e6e96-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="e6e96-114">在第一次使用 Intune 服務的簽入裝置時註冊。</span><span class="sxs-lookup"><span data-stu-id="e6e96-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="e6e96-115">如果裝置成功註冊到 Intune，但未變成已註冊 Intune 裝置，則會在註冊後的 270 天內刪除該裝置。</span><span class="sxs-lookup"><span data-stu-id="e6e96-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="e6e96-116">(90 天將裝置標示為 [已撤銷]，然後下一個180 天刪除記錄)。</span><span class="sxs-lookup"><span data-stu-id="e6e96-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="e6e96-117">Intune 主控台當前不存在為任何指定裝置建立裝置認證有效期限的機制。 </span><span class="sxs-lookup"><span data-stu-id="e6e96-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>