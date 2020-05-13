---
title: Bật ghi lại mật khẩu trong Azure AD kết nối
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: ab4b8692799d08363e1d726f72a3b80dcb598797
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204646"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="2bf3a-102">Bật ghi lại mật khẩu trong Azure AD kết nối</span><span class="sxs-lookup"><span data-stu-id="2bf3a-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="2bf3a-103">Để bật lại ghi lại mật khẩu tự dịch vụ, trước tiên cho phép tuỳ chọn quay lại trong Azure AD kết nối.</span><span class="sxs-lookup"><span data-stu-id="2bf3a-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="2bf3a-104">Từ máy chủ Azure AD kết nối, hoàn thành các bước sau:</span><span class="sxs-lookup"><span data-stu-id="2bf3a-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="2bf3a-105">Đăng nhập vào máy chủ Azure AD kết nối của bạn và khởi động thuật sĩ cấu hình **AZURE AD kết nối** .</span><span class="sxs-lookup"><span data-stu-id="2bf3a-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="2bf3a-106">Trên trang **chào mừng** , bấm **cấu hình**.</span><span class="sxs-lookup"><span data-stu-id="2bf3a-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="2bf3a-107">Trang **tác vụ bổ sung** , chọn **tuỳ chỉnh tùy chọn đồng bộ hóa**, và sau đó nhấp vào **tiếp theo**.</span><span class="sxs-lookup"><span data-stu-id="2bf3a-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="2bf3a-108">Trên trang **kết nối AZURE AD** , nhập uỷ nhiệm quản trị viên chung cho thuê Azure của bạn, và sau đó nhấp vào tiếp theo.</span><span class="sxs-lookup"><span data-stu-id="2bf3a-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click Next.</span></span>
5. <span data-ttu-id="2bf3a-109">Trên các **thư mục kết nối** và **miền/ou** lọc trang, bấm vào **tiếp theo**.</span><span class="sxs-lookup"><span data-stu-id="2bf3a-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="2bf3a-110">Trên trang **tính năng tùy chọn** , chọn hộp bên cạnh ghi **lại mật khẩu** và nhấp vào **tiếp theo**.</span><span class="sxs-lookup"><span data-stu-id="2bf3a-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="2bf3a-111">Trên **sẵn sàng để cấu hình** trang, bấm **cấu hình** và chờ cho quá trình kết thúc.</span><span class="sxs-lookup"><span data-stu-id="2bf3a-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="2bf3a-112">Khi bạn thấy kết thúc cấu hình, bấm **thoát**.</span><span class="sxs-lookup"><span data-stu-id="2bf3a-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="2bf3a-113">Với ghi lại mật khẩu được kích hoạt trong Azure AD kết nối, bây giờ cấu hình Azure AD SSPR để ghi lại.</span><span class="sxs-lookup"><span data-stu-id="2bf3a-113">With password writeback enabled in Azure AD Connect, now configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="2bf3a-114">Để kích hoạt ghi lại mật khẩu trong SSPR, hoàn thành các bước sau:</span><span class="sxs-lookup"><span data-stu-id="2bf3a-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="2bf3a-115">Đăng nhập vào cổng thông tin Azure bằng tài khoản quản trị viên chung.</span><span class="sxs-lookup"><span data-stu-id="2bf3a-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="2bf3a-116">Tìm kiếm và chọn **Azure Active Directory**, bấm **đặt lại mật khẩu**, sau đó chọn **tích hợp tại chỗ**.</span><span class="sxs-lookup"><span data-stu-id="2bf3a-116">Search for and select **Azure Active Directory**, click **Password reset**, then choose **On-premises integration**.</span></span>
3. <span data-ttu-id="2bf3a-117">Đặt tùy chọn **để ghi lại mật khẩu vào thư mục tại chỗ của bạn?** để **có**.</span><span class="sxs-lookup"><span data-stu-id="2bf3a-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="2bf3a-118">Thiết lập tùy chọn cho **phép người dùng mở khóa tài khoản mà không đặt lại mật khẩu của họ?** để **có**.</span><span class="sxs-lookup"><span data-stu-id="2bf3a-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="2bf3a-119">Khi đã sẵn sàng, hãy nhấp vào **lưu**.</span><span class="sxs-lookup"><span data-stu-id="2bf3a-119">When ready, click **Save**.</span></span>

<span data-ttu-id="2bf3a-120">Để biết thêm thông tin, xem [bật lại mật khẩu Azure Active Directory tự dịch vụ ghi ghi lại vào môi trường tại chỗ](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="2bf3a-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>
