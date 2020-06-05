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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579887"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="d25ae-102">Khắc phục các ứng dụng Microsoft 365 "mô-đun nền tảng đáng tin cậy của máy tính không hoạt động đúng" thông báo</span><span class="sxs-lookup"><span data-stu-id="d25ae-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="d25ae-103">Để khắc phục lỗi này, hãy thử như sau:</span><span class="sxs-lookup"><span data-stu-id="d25ae-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="d25ae-104">Cài đặt các bản cập nhật mới nhất cho [Windows](https://support.microsoft.com/help/4027667/windows-10-update) và [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="d25ae-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="d25ae-105">[Thông tin đăng nhập văn phòng rõ ràng](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) bằng cách sử dụng trình quản lý ủy nhiệm Windows.</span><span class="sxs-lookup"><span data-stu-id="d25ae-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="d25ae-106">**Lưu ý:** Đường dẫn đăng ký cho Office 2016 đã thay đổi để 16,0.</span><span class="sxs-lookup"><span data-stu-id="d25ae-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="d25ae-107">(Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="d25ae-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="d25ae-108">Hãy thử [quá trình khôi phục người dùng](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) để khắc phục lỗi nền tảng đáng tin cậy (TPM).</span><span class="sxs-lookup"><span data-stu-id="d25ae-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="d25ae-109">Đặt EnableADAL = 0 bằng cách sử dụng các bước sau:</span><span class="sxs-lookup"><span data-stu-id="d25ae-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="d25ae-110">Bấm chuột phải vào nút khởi động Windows, chọn **chạy**, gõ **regedit**, và sau đó chọn **OK**.</span><span class="sxs-lookup"><span data-stu-id="d25ae-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="d25ae-111">Chọn **có** để cho phép Registry Editor thực hiện thay đổi cho thiết bị của bạn.</span><span class="sxs-lookup"><span data-stu-id="d25ae-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="d25ae-112">Trong Registry Editor, thêm một giá trị của **Enableadal** với một thiết lập **0** trong HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="d25ae-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="d25ae-113">Để biết thêm thông tin, [hãy xem sự cố kết nối trong đăng nhập sau khi Cập Nhật cho Office 2016 xây dựng 16.0.7967 trên Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="d25ae-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>