---
title: Vấn đề đăng nhập vào ứng dụng văn phòng
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
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938391"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="31dbd-102">Đăng nhập màn hình trống trong các ứng dụng văn phòng</span><span class="sxs-lookup"><span data-stu-id="31dbd-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="31dbd-103">Để khắc phục vấn đề này, hãy thử như sau:</span><span class="sxs-lookup"><span data-stu-id="31dbd-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="31dbd-104">Cài đặt các bản cập nhật mới nhất cho [Windows](https://support.microsoft.com/help/4027667/windows-10-update) và [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="31dbd-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="31dbd-105">Đặt lại tuỳ chọn Internet Explorer: vào **Tools** > **Internet Options** > **cao** > **Reset Internet Explorer Settings** (lưu ý rằng bạn sẽ mất các thiết đặt tùy chỉnh), và sau đó cố gắng đăng nhập vào văn phòng một lần nữa.</span><span class="sxs-lookup"><span data-stu-id="31dbd-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="31dbd-106">Vô hiệu hóa Windows Defender áp dụng Guard (WDAG) hoặc bất kỳ chương trình tương tự như tường lửa hoặc chống vi-rút:</span><span class="sxs-lookup"><span data-stu-id="31dbd-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="31dbd-107">Trong bảng điều khiển, đi đến **các chương trình**, và sau đó chọn **Turn Windows features Baät hoaëc taét**.</span><span class="sxs-lookup"><span data-stu-id="31dbd-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="31dbd-108">Nếu bảo vệ ứng dụng Windows Defender được bật, hãy thử vô hiệu hóa nó.</span><span class="sxs-lookup"><span data-stu-id="31dbd-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="31dbd-109">**Lưu ý:** Bạn có thể cần phải khởi động lại máy tính.</span><span class="sxs-lookup"><span data-stu-id="31dbd-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="31dbd-110">Đảm bảo rằng Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) không bị chặn bởi bất kỳ ứng dụng hoặc tường lửa/chống-virus chương trình.</span><span class="sxs-lookup"><span data-stu-id="31dbd-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="31dbd-111">[Rõ ràng văn phòng thông tin đăng nhập](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) bằng cách sử dụng trình quản lý ủy nhiệm của Windows.</span><span class="sxs-lookup"><span data-stu-id="31dbd-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="31dbd-112">**Lưu ý:** Các đường dẫn đăng ký đối với Office 2016 đã thay đổi để 16.0.</span><span class="sxs-lookup"><span data-stu-id="31dbd-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="31dbd-113">(Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="31dbd-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="31dbd-114">Để biết thêm chi tiết, hãy xem [kết nối các vấn đề trong đăng nhập sau khi Cập Nhật cho Office 2016 build 16.0.7967 trên Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="31dbd-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>