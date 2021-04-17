---
title: Các sự cố khi đăng nhập vào ứng dụng Microsoft 365
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
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833061"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="12153-102">Màn hình đăng nhập trống trong các ứng dụng Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="12153-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="12153-103">Để khắc phục sự cố này, hãy thử làm như sau:</span><span class="sxs-lookup"><span data-stu-id="12153-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="12153-104">Cài đặt các bản cập nhật mới nhất cho [Windows](https://support.microsoft.com/help/4027667/windows-10-update) và [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="12153-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="12153-105">Đặt lại tùy chọn Internet Explorer: đi tới **công cụ**  >  **tùy chọn Internet**  >  **nâng cao**  >  **thiết đặt đặt lại Internet Explorer** (lưu ý rằng bạn sẽ mất thiết đặt tùy chỉnh), rồi thử đăng nhập lại vào Office.</span><span class="sxs-lookup"><span data-stu-id="12153-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="12153-106">Tắt bộ bảo vệ ứng dụng Windows Defender (WDAG) hoặc các tường lửa tương tự hoặc chương trình chống vi-rút:</span><span class="sxs-lookup"><span data-stu-id="12153-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="12153-107">Trong Pa-nen điều khiển, đi tới **chương trình**, rồi chọn **bật hoặc tắt tính năng Windows**.</span><span class="sxs-lookup"><span data-stu-id="12153-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="12153-108">Nếu bộ bảo vệ ứng dụng Windows Defender được bật, hãy thử tắt tính năng này.</span><span class="sxs-lookup"><span data-stu-id="12153-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="12153-109">**Lưu ý:** Bạn có thể cần phải khởi động lại máy tính.</span><span class="sxs-lookup"><span data-stu-id="12153-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="12153-110">Đảm bảo rằng Microsoft...... [](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ...........................................</span><span class="sxs-lookup"><span data-stu-id="12153-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="12153-111">[Xóa](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) thông tin xác thực Office bằng trình quản lý chứng danh Windows.</span><span class="sxs-lookup"><span data-stu-id="12153-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="12153-112">**Lưu ý:** Các đường dẫn đăng ký cho Office 2016 đã thay đổi thành 16,0.</span><span class="sxs-lookup"><span data-stu-id="12153-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="12153-113">(Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="12153-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="12153-114">Để biết thêm thông tin, hãy xem các [vấn đề về kết nối trong đăng nhập sau khi cập nhật lên Office 2016 bản dựng 16.0.7967 trên Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="12153-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>