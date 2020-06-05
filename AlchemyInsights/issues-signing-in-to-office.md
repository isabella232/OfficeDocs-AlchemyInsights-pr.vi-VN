---
title: Sự cố khi đăng nhập vào ứng dụng Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579923"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="06d0c-102">Màn hình đăng nhập trống trong ứng dụng Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="06d0c-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="06d0c-103">Để khắc phục sự cố này, hãy thử như sau:</span><span class="sxs-lookup"><span data-stu-id="06d0c-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="06d0c-104">Cài đặt các bản cập nhật mới nhất cho [Windows](https://support.microsoft.com/help/4027667/windows-10-update) và [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="06d0c-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="06d0c-105">Đặt lại tùy chọn Internet Explorer: đi tới **công cụ**  >  **tùy chọn Internet**  >  **nâng cao**thiết lập  >  **lại Internet Explorer cài đặt** (lưu ý rằng bạn sẽ mất cài đặt tuỳ chỉnh), và sau đó thử đăng nhập vào Office một lần nữa.</span><span class="sxs-lookup"><span data-stu-id="06d0c-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="06d0c-106">Vô hiệu hoá Windows Defender Application guard (WDAG) hoặc bất kỳ tường lửa tương tự hoặc chương trình chống vi-rút:</span><span class="sxs-lookup"><span data-stu-id="06d0c-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="06d0c-107">Trong Pa-nen điều khiển, đi tới **chương trình**, sau đó chọn **bật hoặc tắt tính năng của Windows**.</span><span class="sxs-lookup"><span data-stu-id="06d0c-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="06d0c-108">Nếu bộ bảo vệ ứng dụng Windows Defender được bật, hãy thử tắt.</span><span class="sxs-lookup"><span data-stu-id="06d0c-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="06d0c-109">**Lưu ý:** Bạn có thể phải khởi động lại máy tính.</span><span class="sxs-lookup"><span data-stu-id="06d0c-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="06d0c-110">Đảm bảo rằng Microsoft. AAD. BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) không bị chặn bởi bất kỳ ứng dụng hoặc tường lửa/chương trình chống vi-rút.</span><span class="sxs-lookup"><span data-stu-id="06d0c-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="06d0c-111">[Thông tin đăng nhập văn phòng rõ ràng](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) bằng cách sử dụng trình quản lý ủy nhiệm Windows.</span><span class="sxs-lookup"><span data-stu-id="06d0c-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="06d0c-112">**Lưu ý:** Đường dẫn đăng ký cho Office 2016 đã thay đổi để 16,0.</span><span class="sxs-lookup"><span data-stu-id="06d0c-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="06d0c-113">(Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="06d0c-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="06d0c-114">Để biết thêm thông tin, [hãy xem sự cố kết nối trong đăng nhập sau khi Cập Nhật cho Office 2016 xây dựng 16.0.7967 trên Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="06d0c-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>