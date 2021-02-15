---
title: Writeback mật khẩu không hoạt động
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243733"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="9eb66-102">Writeback mật khẩu không hoạt động</span><span class="sxs-lookup"><span data-stu-id="9eb66-102">Password Writeback is not working</span></span>

<span data-ttu-id="9eb66-103">**Tôi đang gặp sự cố về cấu hình writeback mật khẩu**</span><span class="sxs-lookup"><span data-stu-id="9eb66-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="9eb66-104">Trả về mật khẩu là một tính năng Premium.</span><span class="sxs-lookup"><span data-stu-id="9eb66-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="9eb66-105">Hãy đảm bảo rằng bạn hiểu được các yêu cầu cấp phép:</span><span class="sxs-lookup"><span data-stu-id="9eb66-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="9eb66-106">Bạn phải có ít nhất một giấy phép được gán trong tổ chức của bạn</span><span class="sxs-lookup"><span data-stu-id="9eb66-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="9eb66-107">**Đám mây chỉ người dùng** -bất kỳ Office 365 (O365) được trả về SKU hoặc Azure AD BASIC</span><span class="sxs-lookup"><span data-stu-id="9eb66-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="9eb66-108">Nền tảng điện **toán đám mây và/hoặc người dùng tại cơ sở** -Azure AD Premium P1 hoặc P2, doanh nghiệp Mobility + Security (EMS), hoặc doanh nghiệp hiệu quả bảo mật (SPE)</span><span class="sxs-lookup"><span data-stu-id="9eb66-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="9eb66-109">Để tìm hiểu thêm về các yêu cầu cấp phép, hãy xem mục [yêu cầu cấp phép cho AZURE AD self-đặt lại mật khẩu](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="9eb66-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="9eb66-110">Bạn có ít nhất một tài khoản người quản trị và một tài khoản người dùng kiểm tra với một trong số giấy phép thích hợp.</span><span class="sxs-lookup"><span data-stu-id="9eb66-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="9eb66-111">Bạn phải kết nối Azure AD kết nối với trình giả lập bộ điều khiển tên miền chính để làm việc với mật khẩu.</span><span class="sxs-lookup"><span data-stu-id="9eb66-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="9eb66-112">Bạn có thể cấu hình Azure AD Connect để dùng bộ điều khiển tên miền chính bằng cách bấm chuột phải vào **thuộc tính** của đường kết nối đồng bộ hóa Active Directory, sau đó chọn **cấu hình phân vùng thư mục**.</span><span class="sxs-lookup"><span data-stu-id="9eb66-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="9eb66-113">Từ đó, hãy tìm phần **thiết đặt kết nối bộ điều khiển tên miền** và chọn hộp chỉ có tiêu đề dùng bộ kiểm **soát miền ưu tiên**.</span><span class="sxs-lookup"><span data-stu-id="9eb66-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="9eb66-114">Nếu các DC ưu tiên không phải là giả lập PDC, Azure AD Connect sẽ vẫn tiếp cận với PDC để bật lại mật khẩu.</span><span class="sxs-lookup"><span data-stu-id="9eb66-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="9eb66-115">Đặt lại mật khẩu đã được cấu hình và được kích hoạt trong đối tượng thuê của bạn.</span><span class="sxs-lookup"><span data-stu-id="9eb66-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="9eb66-116">Để biết thêm thông tin, hãy xem cho [phép người dùng đặt lại mật khẩu AZURE AD của họ](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span><span class="sxs-lookup"><span data-stu-id="9eb66-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="9eb66-117">Hãy đảm bảo rằng tài khoản người quản trị đang được sử dụng để bật lại mật khẩu là tài khoản người quản trị đám mây (được tạo trong Azure AD không tại cơ sở tại chỗ)</span><span class="sxs-lookup"><span data-stu-id="9eb66-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="9eb66-118">Bạn có triển khai tại cơ sở đơn hoặc nhiều rừng chạy Windows Server 2008 R2, Windows Server 2012 hoặc Windows Server 2012 R2 với các gói dịch vụ mới nhất được cài đặt</span><span class="sxs-lookup"><span data-stu-id="9eb66-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="9eb66-119">Bạn đã cài đặt công cụ kết nối Azure AD và bạn đã chuẩn bị môi trường quảng cáo của mình để đồng bộ trên điện toán đám mây.</span><span class="sxs-lookup"><span data-stu-id="9eb66-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="9eb66-120">Trước khi kiểm tra lại mật khẩu, hãy đảm bảo rằng trước tiên bạn hoàn thành nhập đầy đủ và đồng bộ đầy đủ từ cả quảng cáo và Azure AD trong Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="9eb66-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="9eb66-121">Để tìm hiểu thêm, hãy xem làm thế nào để thực hiện [đồng bộ đầy đủ và nhập đầy đủ trong AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="9eb66-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="9eb66-122">**Tôi đang gặp sự cố với kết nối writeback mật khẩu**</span><span class="sxs-lookup"><span data-stu-id="9eb66-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="9eb66-123">Tải xuống và bật Phiên bản mới nhất của [AZURE AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="9eb66-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="9eb66-124">Cấu hình tường lửa: công cụ Azure AD Connect (1.1.443 trở lên) sẽ cần truy nhập **https ra ngoài** vào:</span><span class="sxs-lookup"><span data-stu-id="9eb66-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="9eb66-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="9eb66-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="9eb66-126">servicebus. Windows. Networks</span><span class="sxs-lookup"><span data-stu-id="9eb66-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="9eb66-127">Cho phép các kết nối nhàn rỗi tồn tại trong ít nhất 2-3 phút</span><span class="sxs-lookup"><span data-stu-id="9eb66-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="9eb66-128">**Tôi vẫn gặp sự cố với writeback mật khẩu**</span><span class="sxs-lookup"><span data-stu-id="9eb66-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="9eb66-129">Nếu bạn vẫn gặp khó khăn, hãy thử tắt và bật lại dịch vụ trả về mật khẩu trong công cụ Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="9eb66-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="9eb66-130">Để tìm hiểu thêm, hãy xem làm thế nào để [vô hiệu hóa và bật lại tính năng bật lại mật khẩu](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="9eb66-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
