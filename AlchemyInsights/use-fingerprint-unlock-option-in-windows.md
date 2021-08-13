---
title: 使用 Windows 10 中的指紋解除鎖定選項
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
- "9001689"
- "3765"
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971878"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>使用 Windows 10 中的指紋解除鎖定選項

**啟用 Windows Hello 指紋**

若要使用您的指紋解除鎖定 Windows 10，您必須透過新增 (來設定 Windows Hello 指紋，Windows 瞭解至少一個手指可辨識) 。 

1. 移至 **設定 > 帳戶 > 登入選項** (或按一下 [這裡](ms-settings:signinoptions?activationSource=GetHelp)) 。 將會列出可用的登入選項。 例如：

    ![登入選項。](media/sign-in-options.png)

2. 按一下或點擊 [ **Windows Hello 指紋**]，然後按一下 [**設定**]。 在 [Windows Hello 設定] 視窗中，按一下 [**開始**]。 指紋感應器將啟動，系統會要求您將手指置於感應器上：

   ![指紋感應器。](media/fingerprint-sensor.png)

3. 遵循指示，它會要求您重複掃描手指。 完成此作業後，您可以選擇新增您可能想要用於登入的其他手指。 當您下次登入 Windows 10 時，您可以選擇使用指紋來執行。

**Windows Hello指紋不可當作登入選項**

如果 Windows Hello 指紋未顯示為 [登入]**選項** 中的選項，則表示 Windows 不會察覺電腦上連接的任何指紋辨識器/掃描器，或是系統原則避免其使用 (如果您的電腦是由您的工作場所) 所管理。 若要疑難排解： 

1. 選取工作列中的 [ **開始** ] 按鈕，然後搜尋 [ **裝置管理員**]。

2. 按一下或點擊以開啟 [ **裝置管理員**]。

3. 在 [裝置管理員] 中，按一下 [生物] 裝置的燕尾展開。

   ![生物識別單元。](media/biometric-devices.png)

4. 您的指紋掃描器應列為生物識別單元，例如 Synaptics WBDI 掃描程式：

   ![生物識別單元。](media/biometric-devices-expanded.png)

5. 如果您的指紋掃描器未顯示，且掃描器已整合到您的電腦，請移至電腦製造商的網站。 在您的電腦型號的技術支援區段中，搜尋您可以安裝之掃描器的 Windows 10 驅動程式。

6. 如果掃描器與 PC 不同于以 USB) 相連 (，請移至掃描器製造商的網站，尋找並安裝您所具備之掃描器型號的 Windows 10 裝置驅動程式軟體。
