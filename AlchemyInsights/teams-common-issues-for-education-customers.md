---
title: Teams 教育版客戶的常見問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000701"
- "3831"
- "3832"
ms.openlocfilehash: 81b80d76530327767bc58adf2e06e5b7ae265f18
ms.sourcegitcommit: 7d787b8c5af223e2711b4c2a2ca55ce2bdc25aea
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/19/2020
ms.locfileid: "42856777"
---
# <a name="teams-common-issues-for-education-customers"></a>Teams 教育版客戶的常見問題

**適用於教育版客戶**：

如果您需要部署 Teams 來支援遠端學習的協助，請造訪[FastTrack 中心](https://www.microsoft.com/fasttrack)來提交要求。 查看 Teams 教育版客戶的下列常見問題：

- 您是否看到「**您錯過了！**」的訊息？ 請確定要[為您的學校啟用 Microsoft Teams](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams)。 在 EDU 租用戶中不會預設啟用 Microsoft Teams；您必須先將它開啟。

- **Teams 的新使用者嗎？** 請參閱 [Office 365 教育版中的遠端教學和學習](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4)，以了解如何設定學校、課程規劃、虛擬會議，以及與學生共用內容的最新指導方針。

- 開啟後，您的使用者就可以透過安裝[桌面](https://docs.microsoft.com/MicrosoftTeams/get-clients#desktop-client)和[行動用戶端](https://docs.microsoft.com/MicrosoftTeams/get-clients#mobile-clients)執行 Teams，或從瀏覽器，在 https://teams.microsoft.com 上執行。

- **啟用 Teams 來賓存取：** 參閱 [Teams 來賓存取檢查清單](https://docs.microsoft.com/microsoftteams/guest-access-checklist)，並確定已完成所有步驟。
    - [了解 Microsoft Teams 中的來賓存取](https://docs.microsoft.com/microsoftteams/guest-access)
    - [設定 – Microsoft Teams 來賓存取檢查清單](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [來賓加入小組的方式](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Teams 會議和電話撥入**：需要在 Microsoft Teams 中開啟或設定音訊會議的協助嗎？ 這名使用者是最近建立的嗎？ 如果是，您必須等待 2 至 24 小時設定才會生效。 若要驗證使用者已獲得音訊會議授權，並擁有預設付費電話號碼：
    1. 移至 [作用中使用者] 然後選取有問題的使用者。
    2. 視系統管理中心的版本而定，請選擇 [授權和應用程式]****，或按一下 [產品授權]**** 上的 [編輯]****。
    3. 確認使用者已選取 [Microsoft Teams 音訊會議] 和 [商務用 Skype Online (方案2)] 的授權。
    4. 使用者在 [系統管理中心] 按一下 [全部顯示]****，再按一下 [Teams]****。
    5. 在 [Microsoft Teams 系統管理中心] 中，按一下 [傳統入口網站]****。
    6. 在 [商務用 Skype 系統管理中心] 中，按一下 [音訊會議]****，再按一下 [使用者]****。
    7. 選取有問題的使用者，並確認使用者有 [預設付費電話號碼]。

    如需詳細資訊，請參閱 [Office 365 的通話方案](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365) (英文)，或撥打 Microsoft Commerce 收費團隊，取得授權相關問題的協助。

    其他資源

    - [Microsoft Teams 中的會議和召集會議](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Office 365 的音訊會議](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **會議原則**：會議原則是針對由您組織中使用者所安排的會議，控制會議參與者可用於會議的功能。 建立原則並進行變更之後，您可以將使用者指派給該原則。

    - **變更或建立會議原則**：若要變更或建立會議原則，請移至 [Microsoft Teams 系統管理中心] > [會議] > [會議原則]****。 從清單中選取原則，或按一下 [新增]****。 如果您要建立新原則，請新增原則的名稱和描述。 名稱不能包含特殊字元，且長度不可超過 64 個字元。 選擇您的設定，然後按一下 [儲存]****。 
    
        例如，假設您有多位使用者，並且想要限制其會議所需的頻寬。 您可以建立名為「有限頻寬」的新自訂原則，並停用下列設定：

        在 [音訊與視訊]**** 下：
        - 關閉 [允許雲端錄製]****。
        - 關閉 [允許 IP 視訊]****。

        在 [內容共用]**** 下：

        - 停用 [螢幕畫面分享模式]。
        - 關閉 [允許白板]****。
        - 關閉 [允許共用記事]****。

        然後，**將原則指派給使用者**：

    1. 在 Microsoft Teams 系統管理中心的左側瀏覽窗格中，移至 [使用者]****，然後按一下該使用者。
    2. 按一下使用者名稱左方以選取使用者，然後按一下 [編輯設定]****。
    3. 在 [會議原則]**** 下，選取要指派的原則，然後按一下 [套用]****。

    若要一次將原則指派給多個使用者，請參閱[大量編輯 Teams 使用者設定](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk)。

    或者，您可以執行下列內容︰
    1. 在 Microsoft Teams 系統管理中心的左側瀏覽窗格中，移至 [會議] > [會議原則]****。
    2. 按一下原則名稱的左側來選取原則。
    3. 按一下 [管理使用者]****。
    4. 在 [管理使用者]**** 窗格中，依顯示名稱或使用者名稱搜尋使用者，選取名稱，然後按一下 [新增]****。 針對要新增的每一個使用者重複此步驟。
    5. 新增完使用者之後，按一下 [儲存]****。

- **遺失撥號鍵台的疑難排解：**：
    - 請確認已指派使用者 [[Teams 授權]](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses)。
    - 請確認已指派使用者 [[通話方案]](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page)。
    - 為使用者啟用 [[企業語音]](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail)。

- **針對 Teams 登入問題進行疑難排解：** 首先，請確認 [Microsoft Teams 服務狀況良好](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth)。 然後檢查是否有任何常見的錯誤碼，並參閱[為何我無法登入 Microsoft Teams](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f)？ 您可能還需要參閱 [Microsoft Teams 中的身分識別模型和驗證方式](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication) (部分機器翻譯)。
