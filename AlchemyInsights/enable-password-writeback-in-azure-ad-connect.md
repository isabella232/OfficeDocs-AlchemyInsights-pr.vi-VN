---
title: Bật lại mật khẩu trong Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 9dbb88492a3906f6780a345cf880327d411dcc66
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709749"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="d6142-102">Bật lại mật khẩu trong Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="d6142-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="d6142-103">Để bật lại bản đặt lại mật khẩu tự phục vụ, trước tiên, bật tùy chọn writeback trong Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d6142-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="d6142-104">Từ máy chủ Azure AD Connect của bạn, hãy hoàn thành các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="d6142-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="d6142-105">Đăng nhập vào máy chủ Azure AD Connect của bạn và bắt đầu trình hướng dẫn cấu hình **AZURE AD Connect** .</span><span class="sxs-lookup"><span data-stu-id="d6142-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="d6142-106">Trên trang **chào mừng** , bấm **cấu hình**.</span><span class="sxs-lookup"><span data-stu-id="d6142-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="d6142-107">Trên trang **nhiệm vụ bổ sung** , hãy chọn tùy **chỉnh tùy chọn đồng bộ**, rồi bấm vào **tiếp theo**.</span><span class="sxs-lookup"><span data-stu-id="d6142-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="d6142-108">Trên trang **kết nối đến AZURE AD** , nhập thông tin xác thực người quản trị toàn cầu cho đối tượng thuê Azure của bạn, rồi bấm vào tiếp theo.</span><span class="sxs-lookup"><span data-stu-id="d6142-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click Next.</span></span>
5. <span data-ttu-id="d6142-109">Trên trang các **thư mục kết nối** và **tên miền/ou** lọc, bấm **tiếp**.</span><span class="sxs-lookup"><span data-stu-id="d6142-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="d6142-110">Trên trang **tính năng tùy chọn** , chọn hộp bên cạnh **mật khẩu trở lại** và bấm **tiếp**.</span><span class="sxs-lookup"><span data-stu-id="d6142-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="d6142-111">Trên trang **sẵn sàng cấu hình** , hãy bấm **cấu hình** và chờ cho quá trình kết thúc.</span><span class="sxs-lookup"><span data-stu-id="d6142-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="d6142-112">Khi bạn nhìn thấy kết thúc cấu hình, hãy bấm **thoát**.</span><span class="sxs-lookup"><span data-stu-id="d6142-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="d6142-113">Với mật khẩu được bật lại trong Azure AD Connect, giờ đây, hãy cấu hình Azure AD SSPR cho writeback.</span><span class="sxs-lookup"><span data-stu-id="d6142-113">With password writeback enabled in Azure AD Connect, now configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="d6142-114">Để bật lại mật khẩu trong SSPR, hãy hoàn thành các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="d6142-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="d6142-115">Đăng nhập vào cổng thông tin Azure bằng tài khoản người quản trị toàn cầu.</span><span class="sxs-lookup"><span data-stu-id="d6142-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="d6142-116">Tìm kiếm và chọn **Azure Active Directory**, bấm vào **đặt lại mật khẩu**, sau đó chọn **tích hợp tại cơ sở**.</span><span class="sxs-lookup"><span data-stu-id="d6142-116">Search for and select **Azure Active Directory**, click **Password reset**, then choose **On-premises integration**.</span></span>
3. <span data-ttu-id="d6142-117">Đặt tùy chọn để **ghi lại mật khẩu vào thư mục tại chỗ của bạn?** để **có**.</span><span class="sxs-lookup"><span data-stu-id="d6142-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="d6142-118">Đặt tùy chọn cho **phép người dùng mở khóa tài khoản mà không đặt lại mật khẩu của họ?** để **có**.</span><span class="sxs-lookup"><span data-stu-id="d6142-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="d6142-119">Khi đã sẵn sàng, hãy bấm **lưu**.</span><span class="sxs-lookup"><span data-stu-id="d6142-119">When ready, click **Save**.</span></span>

<span data-ttu-id="d6142-120">Để biết thêm thông tin, hãy xem [bật thiết đặt lại mật khẩu tự phục vụ Azure Active Directory với môi trường tại chỗ](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="d6142-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>
