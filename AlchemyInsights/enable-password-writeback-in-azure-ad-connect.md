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
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093377"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="b2ead-102">Bật lại mật khẩu trong Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="b2ead-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="b2ead-103">Để bật lại bản đặt lại mật khẩu tự phục vụ, trước tiên, bật tùy chọn writeback trong Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="b2ead-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="b2ead-104">Từ máy chủ Azure AD Connect của bạn, hãy hoàn thành các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="b2ead-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="b2ead-105">Đăng nhập vào máy chủ Azure AD Connect của bạn và bắt đầu trình hướng dẫn cấu hình **AZURE AD Connect** .</span><span class="sxs-lookup"><span data-stu-id="b2ead-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="b2ead-106">Trên trang **chào mừng** , bấm **cấu hình**.</span><span class="sxs-lookup"><span data-stu-id="b2ead-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="b2ead-107">Trên trang **nhiệm vụ bổ sung** , hãy chọn tùy **chỉnh tùy chọn đồng bộ**, rồi bấm vào **tiếp theo**.</span><span class="sxs-lookup"><span data-stu-id="b2ead-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="b2ead-108">Trên trang **kết nối đến AZURE AD** , nhập thông tin xác thực người quản trị toàn cầu cho đối tượng thuê Azure của bạn, rồi bấm vào **tiếp theo**.</span><span class="sxs-lookup"><span data-stu-id="b2ead-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="b2ead-109">Trên trang các **thư mục kết nối** và **tên miền/ou** lọc, bấm **tiếp**.</span><span class="sxs-lookup"><span data-stu-id="b2ead-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="b2ead-110">Trên trang **tính năng tùy chọn** , chọn hộp bên cạnh **mật khẩu trở lại** và bấm **tiếp**.</span><span class="sxs-lookup"><span data-stu-id="b2ead-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="b2ead-111">Trên trang **sẵn sàng cấu hình** , hãy bấm **cấu hình** và chờ cho quá trình kết thúc.</span><span class="sxs-lookup"><span data-stu-id="b2ead-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="b2ead-112">Khi bạn nhìn thấy kết thúc cấu hình, hãy bấm **thoát**.</span><span class="sxs-lookup"><span data-stu-id="b2ead-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="b2ead-113">Với mật khẩu được bật lại trong Azure AD Connect, hãy cấu hình Azure AD SSPR cho writeback.</span><span class="sxs-lookup"><span data-stu-id="b2ead-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="b2ead-114">Để bật lại mật khẩu trong SSPR, hãy hoàn thành các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="b2ead-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="b2ead-115">Đăng nhập vào cổng thông tin Azure bằng tài khoản người quản trị toàn cầu.</span><span class="sxs-lookup"><span data-stu-id="b2ead-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="b2ead-116">Tìm kiếm và chọn **Azure Active Directory**, bấm vào **đặt lại mật khẩu**, sau đó bấm **tích hợp tại cơ sở**.</span><span class="sxs-lookup"><span data-stu-id="b2ead-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="b2ead-117">Đặt tùy chọn để **ghi lại mật khẩu vào thư mục tại chỗ của bạn?** để **có**.</span><span class="sxs-lookup"><span data-stu-id="b2ead-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="b2ead-118">Đặt tùy chọn cho **phép người dùng mở khóa tài khoản mà không đặt lại mật khẩu của họ?** để **có**.</span><span class="sxs-lookup"><span data-stu-id="b2ead-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="b2ead-119">Khi đã sẵn sàng, hãy bấm **lưu**.</span><span class="sxs-lookup"><span data-stu-id="b2ead-119">When ready, click **Save**.</span></span>

<span data-ttu-id="b2ead-120">Để biết thêm thông tin, hãy xem [bật thiết đặt lại mật khẩu tự phục vụ Azure Active Directory với môi trường tại chỗ](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="b2ead-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="b2ead-121">Khi người quản trị đặt lại mật khẩu của người dùng trong cổng thông tin Azure, nếu người dùng đó được liên kết hoặc băm mật khẩu được đồng bộ hóa, thì mật khẩu sẽ được ghi lại tại chỗ.</span><span class="sxs-lookup"><span data-stu-id="b2ead-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="b2ead-122">Chức năng này đòi hỏi giấy phép Azure Premium (P1 hoặc P2) và hiện không được hỗ trợ trong cổng thông tin quản trị Office.</span><span class="sxs-lookup"><span data-stu-id="b2ead-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
