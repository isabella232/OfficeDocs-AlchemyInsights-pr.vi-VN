---
title: Các sự cố khi đăng nhập vào ứng dụng Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709128"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="0bfa4-102">Khắc phục các ứng dụng Microsoft 365 "mô-đun nền tảng tin cậy của máy tính của bạn không hoạt động đúng"</span><span class="sxs-lookup"><span data-stu-id="0bfa4-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="0bfa4-103">Để khắc phục lỗi này, hãy thử làm như sau:</span><span class="sxs-lookup"><span data-stu-id="0bfa4-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="0bfa4-104">Cài đặt các bản cập nhật mới nhất cho [Windows](https://support.microsoft.com/help/4027667/windows-10-update) và [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="0bfa4-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="0bfa4-105">[Xóa](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) thông tin xác thực Office bằng trình quản lý chứng danh Windows.</span><span class="sxs-lookup"><span data-stu-id="0bfa4-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="0bfa4-106">**Lưu ý:** Các đường dẫn đăng ký cho Office 2016 đã thay đổi thành 16,0.</span><span class="sxs-lookup"><span data-stu-id="0bfa4-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="0bfa4-107">(Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="0bfa4-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="0bfa4-108">Hãy thử [quy trình khôi phục người dùng](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) để khắc phục lỗi mô-đun nền tảng tin cậy (TPM).</span><span class="sxs-lookup"><span data-stu-id="0bfa4-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="0bfa4-109">Đặt EnableADAL = 0 bằng cách dùng các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="0bfa4-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="0bfa4-110">Bấm chuột phải vào nút bắt đầu của Windows, chọn **chạy**, nhập **regedit**, rồi chọn **OK**.</span><span class="sxs-lookup"><span data-stu-id="0bfa4-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="0bfa4-111">Chọn **có** để cho phép trình soạn thảo sổ đăng ký thực hiện thay đổi đối với thiết bị của bạn.</span><span class="sxs-lookup"><span data-stu-id="0bfa4-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="0bfa4-112">Trong trình soạn thảo sổ đăng ký, hãy thêm một giá trị DWORD của **Enableadal** với một thiết đặt của **0** dưới HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="0bfa4-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="0bfa4-113">Để biết thêm thông tin, hãy xem các [vấn đề về kết nối trong đăng nhập sau khi cập nhật lên Office 2016 bản dựng 16.0.7967 trên Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="0bfa4-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>