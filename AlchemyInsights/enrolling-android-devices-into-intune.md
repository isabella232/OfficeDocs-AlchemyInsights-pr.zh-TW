---
title: 將 Android 裝置登記至 Intune
ms.author: erikje
author: erikje
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000652"
- "2494"
ms.openlocfilehash: c39fec48f791d5cc4a97688cc7b5cd93010403a2
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791249"
---
# <a name="enrolling-android-devices-into-intune"></a><span data-ttu-id="a1bc4-102">將 Android 裝置登記至 Intune</span><span class="sxs-lookup"><span data-stu-id="a1bc4-102">Enrolling Android devices into Intune</span></span>

<span data-ttu-id="a1bc4-103">如果您想要將使用者從 Android 裝置管理員註冊遷移至 Android Enterprise，請參閱： [從裝置管理員移動 Android 裝置以運作設定檔管理](https://docs.microsoft.com/mem/intune/enrollment/android-move-device-admin-work-profile)。</span><span class="sxs-lookup"><span data-stu-id="a1bc4-103">If you are looking to migrate users from Android Device Administrator enrollment to Android Enterprise, please review: [Move Android devices from device administrator to work profile management](https://docs.microsoft.com/mem/intune/enrollment/android-move-device-admin-work-profile).</span></span>

<span data-ttu-id="a1bc4-104">Intune 支援註冊下列 Android 裝置：</span><span class="sxs-lookup"><span data-stu-id="a1bc4-104">Intune supports the enrollment of the following Android devices:</span></span>  

- [<span data-ttu-id="a1bc4-105">Samsung Knox，Zebra，裝置管理員</span><span class="sxs-lookup"><span data-stu-id="a1bc4-105">Samsung Knox, Zebra, Device Administrator</span></span>](https://docs.microsoft.com/mem/intune/enrollment/android-enroll-device-administrator)
- [<span data-ttu-id="a1bc4-106">Android Enterprise 工作設定檔</span><span class="sxs-lookup"><span data-stu-id="a1bc4-106">Android Enterprise work profile</span></span>](https://docs.microsoft.com/mem/intune/enrollment/android-enterprise-overview)
- [<span data-ttu-id="a1bc4-107">Android 企業專用</span><span class="sxs-lookup"><span data-stu-id="a1bc4-107">Android Enterprise dedicated</span></span>](https://docs.microsoft.com/mem/intune/enrollment/android-dedicated-devices-fully-managed-enroll)
- [<span data-ttu-id="a1bc4-108">完全管理的 Android 企業</span><span class="sxs-lookup"><span data-stu-id="a1bc4-108">Android Enterprise fully managed</span></span>](https://docs.microsoft.com/mem/intune/enrollment/android-fully-managed-enroll)

<span data-ttu-id="a1bc4-109">在設定 Android 裝置的註冊之前，請先 [複查](https://docs.microsoft.com/intune/enrollment/android-enroll)必要條件。</span><span class="sxs-lookup"><span data-stu-id="a1bc4-109">Before setting up enrollment for Android devices, [review the pre-requisites](https://docs.microsoft.com/intune/enrollment/android-enroll).</span></span>  

<span data-ttu-id="a1bc4-110">如需一般和某些 Android 註冊錯誤疑難排解的詳細資訊，請參閱 [疑難排解 Microsoft Intune 中的裝置註冊](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-android-enrollment)。</span><span class="sxs-lookup"><span data-stu-id="a1bc4-110">For information on troubleshooting device enrollment in general and some Android enrollment errors, see [Troubleshoot device enrollment in Microsoft Intune](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-android-enrollment).</span></span>

<span data-ttu-id="a1bc4-111">您也可以使用描述 Intune 疑難排解 blade 的內容，協助識別您的使用者遇到的 enrolment 問題。</span><span class="sxs-lookup"><span data-stu-id="a1bc4-111">You can also use the content describing the Intune Troubleshooting blade to help identify what enrolment issues your users are experiencing.</span></span>
