---
title: Sửa chữa các ứng dụng văn phòng tài khoản của bạn đang ở trạng thái xấu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969935"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="b3968-102">Sửa chữa các ứng dụng Office "tài khoản của bạn đang ở trạng thái xấu" lỗi</span><span class="sxs-lookup"><span data-stu-id="b3968-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="b3968-103">Để khắc phục lỗi này, hãy thử các tuỳ chọn sau trên máy tính bị ảnh hưởng:</span><span class="sxs-lookup"><span data-stu-id="b3968-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="b3968-104">Mở ứng dụng Office, chọn \*\*\*\* > **tài khoản** > tệp**đăng xuất khỏi tất cả tài khoản**.</span><span class="sxs-lookup"><span data-stu-id="b3968-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="b3968-105">Đăng nhập lại bằng tài khoản người dùng có giấy phép hợp lệ.</span><span class="sxs-lookup"><span data-stu-id="b3968-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="b3968-106">Để biết thông tin chi tiết, xem [tài khoản trong Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="b3968-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="b3968-107">[Thông tin đăng nhập văn phòng rõ ràng](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) bằng cách sử dụng trình quản lý ủy nhiệm Windows.</span><span class="sxs-lookup"><span data-stu-id="b3968-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="b3968-108">**Lưu ý:** Đường dẫn đăng ký cho Office 2016 đã thay đổi để 16,0.</span><span class="sxs-lookup"><span data-stu-id="b3968-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="b3968-109">Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="b3968-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="b3968-110">Trên máy tính bị ảnh hưởng, đặt EnableADAL = 0 bằng cách sử dụng các bước sau:</span><span class="sxs-lookup"><span data-stu-id="b3968-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="b3968-111">Bấm chuột phải vào nút Windows và chọn **chạy**.</span><span class="sxs-lookup"><span data-stu-id="b3968-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="b3968-112">Trong hộp **mở** , gõ **regedit**, và sau đó chọn **OK**.</span><span class="sxs-lookup"><span data-stu-id="b3968-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="b3968-113">Chọn **có** khi được nhắc để cho phép Registry Editor thay đổi thiết bị của bạn.</span><span class="sxs-lookup"><span data-stu-id="b3968-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="b3968-114">Trong trình chỉnh sửa sổ đăng ký, thêm giá trị EnableADAL với thiết đặt 0 trong HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="b3968-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="b3968-115">Nếu xảy ra lỗi khi kết nối với Office 365 bằng cách sử dụng Office 2013, [kích hoạt xác thực hiện đại](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) cho khách hàng Office.</span><span class="sxs-lookup"><span data-stu-id="b3968-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="b3968-116">Để biết thêm thông tin, hãy xem [cách khắc phục sự cố ứng dụng không có trình duyệt không thể đăng nhập vào Office 365, Azure hoặc InTune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="b3968-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

