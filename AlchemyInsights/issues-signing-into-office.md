---
title: Sự cố khi đăng nhập vào ứng dụng Office
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
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763023"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="436f0-102">Sự cố khi đăng nhập vào ứng dụng Office</span><span class="sxs-lookup"><span data-stu-id="436f0-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="436f0-103">Để khắc phục sự cố đăng nhập với ứng dụng Office, hãy thử như sau:</span><span class="sxs-lookup"><span data-stu-id="436f0-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="436f0-104">Xóa tất cả tài khoản công việc, ngoại trừ tài khoản bị ảnh hưởng, sử dụng cài đặt Windows > **truy cập công việc hoặc trường học**.</span><span class="sxs-lookup"><span data-stu-id="436f0-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="436f0-105">[Thông tin đăng nhập văn phòng rõ ràng](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) bằng cách sử dụng trình quản lý ủy nhiệm Windows.</span><span class="sxs-lookup"><span data-stu-id="436f0-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="436f0-106">**Lưu ý:** Đường dẫn đăng ký cho Office 2016 đã thay đổi để 16,0.</span><span class="sxs-lookup"><span data-stu-id="436f0-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="436f0-107">(Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="436f0-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="436f0-108">Mở ứng dụng Office, chọn**đăng**xuất**tài khoản** >  **tệp** > . Sau đó đăng nhập bằng tài khoản người dùng có giấy phép hợp lệ.</span><span class="sxs-lookup"><span data-stu-id="436f0-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="436f0-109">Để biết thông tin chi tiết, xem [tài khoản trong Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="436f0-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="436f0-110">Đối với Mac, xem [không thể đăng nhập vào một Office 2016 cho Mac ứng dụng](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="436f0-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="436f0-111">Nếu lỗi xảy ra khi kết nối với Microsoft 365 bằng cách sử dụng Office 2013, cho phép xác thực hiện đại cho khách hàng Office.</span><span class="sxs-lookup"><span data-stu-id="436f0-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="436f0-112">Để biết thêm thông tin, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="436f0-112">For more information, see:</span></span>
- [<span data-ttu-id="436f0-113">Bạn không thể đăng nhập vào Microsoft 365, Azure hoặc InTune</span><span class="sxs-lookup"><span data-stu-id="436f0-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="436f0-114">Sự cố kết nối trong đăng nhập sau khi Cập Nhật Office 2016 xây dựng 16.0.7967 trên Windows 10</span><span class="sxs-lookup"><span data-stu-id="436f0-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="436f0-115">"Xin lỗi, một tài khoản khác từ tổ chức của bạn đã đăng nhập vào máy tính này" trong Office</span><span class="sxs-lookup"><span data-stu-id="436f0-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="436f0-116">Khắc phục sự cố đăng nhập với Office hiện đại xác thực khi bạn sử dụng ADFS</span><span class="sxs-lookup"><span data-stu-id="436f0-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)