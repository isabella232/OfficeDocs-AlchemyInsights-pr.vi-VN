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
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938390"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="a4dfd-102">Vấn đề đăng nhập vào ứng dụng văn phòng</span><span class="sxs-lookup"><span data-stu-id="a4dfd-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="a4dfd-103">Để khắc phục vấn đề đăng nhập với các ứng dụng văn phòng, hãy thử như sau:</span><span class="sxs-lookup"><span data-stu-id="a4dfd-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="a4dfd-104">Loại bỏ tất cả các tài khoản công việc, trừ các tài khoản bị ảnh hưởng, bằng cách sử dụng thiết đặt Windows > **truy cập làm việc hay trường học**.</span><span class="sxs-lookup"><span data-stu-id="a4dfd-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="a4dfd-105">[Rõ ràng văn phòng thông tin đăng nhập](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) bằng cách sử dụng trình quản lý ủy nhiệm của Windows.</span><span class="sxs-lookup"><span data-stu-id="a4dfd-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="a4dfd-106">**Lưu ý:** Các đường dẫn đăng ký đối với Office 2016 đã thay đổi để 16.0.</span><span class="sxs-lookup"><span data-stu-id="a4dfd-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="a4dfd-107">(Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="a4dfd-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="a4dfd-108">Mở một ứng dụng văn phòng, chọn **File** > **tài khoản** > **Đăng xuất**. Sau đó đăng nhập bằng tài khoản người dùng với một giấy phép hợp lệ.</span><span class="sxs-lookup"><span data-stu-id="a4dfd-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="a4dfd-109">Thông tin chi tiết, hãy xem [các tài khoản trong văn phòng](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="a4dfd-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="a4dfd-110">Dành cho Mac, hãy xem [không thể đăng nhập vào một Office 2016 cho Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="a4dfd-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="a4dfd-111">Nếu lỗi xảy ra trong khi kết nối với Office 365 sử dụng Office 2013, cho phép xác thực hiện đại cho văn phòng khách hàng.</span><span class="sxs-lookup"><span data-stu-id="a4dfd-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="a4dfd-112">Để biết thêm thông tin, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="a4dfd-112">For more information, see:</span></span>
- [<span data-ttu-id="a4dfd-113">Bạn không thể đăng nhập vào Office 365, Azure hoặc dành</span><span class="sxs-lookup"><span data-stu-id="a4dfd-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="a4dfd-114">Vấn đề kết nối trong đăng nhập sau khi Cập Nhật cho Office 2016 xây dựng 16.0.7967 trên Windows 10</span><span class="sxs-lookup"><span data-stu-id="a4dfd-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="a4dfd-115">"Xin lỗi, các tài khoản khác từ tổ chức của bạn đã được đăng nhập trên máy tính này" trong văn phòng</span><span class="sxs-lookup"><span data-stu-id="a4dfd-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="a4dfd-116">Khắc phục sự cố đăng nhập với văn phòng hiện đại xác thực khi bạn sử dụng ADFS</span><span class="sxs-lookup"><span data-stu-id="a4dfd-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)