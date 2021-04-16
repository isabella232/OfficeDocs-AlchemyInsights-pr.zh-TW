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
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796668"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>使用 Windows 10 中的指紋解除鎖定選項

**啟用 Windows Hello 指紋**

若要使用您的指紋解除 Windows 10 的鎖定，您需要透過新增 (讓 Windows 瞭解至少有一個手指可辨識) ，以設定 Windows Hello 指紋。 

1. 移至 [ **設定] > 帳戶 > 登入選項** ] (或按一下 [ [這裡](ms-settings:signinoptions?activationSource=GetHelp)) ]。 將會列出可用的登入選項。 例如：

    ![登入選項。](media/sign-in-options.png)

2. 按一下或點擊 [ **Windows Hello 指紋**]，然後按一下 [ **設定**]。 按一下 [Windows Hello 安裝程式] 視窗中的 [ **開始**]。 指紋感應器將啟動，系統會要求您將手指置於感應器上：

   ![指紋感應器。](media/fingerprint-sensor.png)

3. 遵循指示，它會要求您重複掃描手指。 完成此作業後，您可以選擇新增您可能想要用於登入的其他手指。 當您下次登入 Windows 10 時，您可以選擇使用您的指紋來執行此動作。

**Windows Hello 指紋無法當作登入選項使用**

如果 Windows Hello 指紋未顯示為 [登入] **選項** 中的選項，表示 windows 不會察覺電腦上連接的任何指紋辨識器/掃描器，或者如果您的電腦是由您的工作地點) 所管理，則系統原則可以避免其使用 (。 若要疑難排解： 

1. 選取工作列中的 [ **開始** ] 按鈕，然後搜尋 [ **裝置管理員**]。

2. 按一下或點擊以開啟 [ **裝置管理員**]。

3. 在 [裝置管理員] 中，按一下 [生物] 裝置的燕尾展開。

   ![生物識別單元。](media/biometric-devices.png)

4. 您的指紋掃描器應列為生物識別單元，例如 Synaptics WBDI 掃描程式：

   ![生物識別單元。](media/biometric-devices-expanded.png)

5. 如果您的指紋掃描器未顯示，且掃描器已整合到您的電腦，請移至電腦製造商的網站。 在您的電腦型號的技術支援區段中，搜尋您可以安裝之掃描器的 Windows 10 驅動程式。

6. 如果掃描器與 PC 不同于透過 USB) 相連 (，請移至掃描器製造商的網站，針對您所擁有的掃描器模型，尋找並安裝 Windows 10 裝置驅動程式軟體。
