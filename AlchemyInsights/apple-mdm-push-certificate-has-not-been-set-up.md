---
title: 未設定 Apple MDM 推播憑證
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431460"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="82a06-102">未設定 Apple MDM 推播憑證</span><span class="sxs-lookup"><span data-stu-id="82a06-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="82a06-103">您的訂閱尚未設定 Apple MDM 推播憑證 (又稱為 Apple 推播通知服務 (APN) 憑證)。</span><span class="sxs-lookup"><span data-stu-id="82a06-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="82a06-104">如果沒有設定 Apple MDM 推播憑證，您將無法註冊及管理 iOS 和 Mac OS 裝置。</span><span class="sxs-lookup"><span data-stu-id="82a06-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="82a06-105">將憑證新增至 Intune 之後，使用者就可以安裝公司入口網站應用程式來註冊其 iOS 裝置。</span><span class="sxs-lookup"><span data-stu-id="82a06-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="82a06-106">選取 **[我同意]**。</span><span class="sxs-lookup"><span data-stu-id="82a06-106">Select **"I agree."**</span></span> <span data-ttu-id="82a06-107">允許 Microsoft 將資料傳送到 Apple。</span><span class="sxs-lookup"><span data-stu-id="82a06-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="82a06-108">選取 Intune 憑證登入請求必要的 **[下載您的 CSR]** 以創建 Apple MDM 推播憑證。</span><span class="sxs-lookup"><span data-stu-id="82a06-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="82a06-109">該檔案用於從 Apple 推播憑證入口網站請求信任關係憑證。</span><span class="sxs-lookup"><span data-stu-id="82a06-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="82a06-110">選取 **[建立您的 MDM 推播憑證]** 以移至 Apple 推播憑證入口網站。</span><span class="sxs-lookup"><span data-stu-id="82a06-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="82a06-111">使用您公司的 Apple ID 登入，然後選取**建立憑證**。</span><span class="sxs-lookup"><span data-stu-id="82a06-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="82a06-112">選取 **[選擇檔案]**，然後流覽至憑證簽署要求檔案，然後選擇 **[上傳]**。</span><span class="sxs-lookup"><span data-stu-id="82a06-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="82a06-113">在 [確認] 頁面上，選擇 **[下載]** 下載憑證 (.pem) 檔案，並將檔案儲存在本機。</span><span class="sxs-lookup"><span data-stu-id="82a06-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="82a06-114">**附註**：該憑證與建立它時使用的 Apple ID 相關聯。</span><span class="sxs-lookup"><span data-stu-id="82a06-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="82a06-115">最佳做法是使用公司 Apple ID 執行管理工作，並確認信箱由多人或使用通訊群組清單監視。</span><span class="sxs-lookup"><span data-stu-id="82a06-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="82a06-116">請勿使用個人 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="82a06-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="82a06-117">每12個月使用相同的 Apple ID 續約 Apple 推播憑證。</span><span class="sxs-lookup"><span data-stu-id="82a06-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="82a06-118">輸入建立 Apple MDM 推播憑證時使用的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="82a06-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="82a06-119">當您需要續約憑證時，請將此 ID 記錄為提醒。</span><span class="sxs-lookup"><span data-stu-id="82a06-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="82a06-120">移至憑證 (.pem) 檔案，選取 **[開啟]**，然後選擇 **[上傳]**。</span><span class="sxs-lookup"><span data-stu-id="82a06-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="82a06-121">使用推播憑證，Intune 就能註冊及管理 Apple 裝置。</span><span class="sxs-lookup"><span data-stu-id="82a06-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>