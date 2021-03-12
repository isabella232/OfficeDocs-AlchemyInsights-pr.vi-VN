---
title: Không thể gửi/nhận email đến/từ Office 365 vì của TLS 1,0 và TLS 1,1 đã ngừng phân tích
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747111"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="27a0a-102">Không thể gửi/nhận email đến/từ Office 365 vì của TLS 1,0 và TLS 1,1 đã ngừng phân tích</span><span class="sxs-lookup"><span data-stu-id="27a0a-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="27a0a-103">Khi được xác nhận bởi Trung tâm thông báo Post MC229914, TLS 1,0 và TLS 1,1 việc phản đối bắt đầu thực thi các điểm cuối dòng thư Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="27a0a-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="27a0a-104">Soon Office 365 sẽ không còn chấp nhận kết nối email TLS 1,0 và TLS 1,1 từ các nguồn bên ngoài.</span><span class="sxs-lookup"><span data-stu-id="27a0a-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="27a0a-105">Ngoài ra, Exchange Online sẽ không bao giờ sử dụng TLS 1,0 hoặc 1,1 để gửi email đi.</span><span class="sxs-lookup"><span data-stu-id="27a0a-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="27a0a-106">Nếu bạn đang gặp phải sự cố vì 1,0 hoặc 1,1 không phân hủy, bạn có thể gặp một trong các lỗi sau đây-</span><span class="sxs-lookup"><span data-stu-id="27a0a-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="27a0a-107">Người gửi đang nhận được NDR Bounce Back-' 421 kết nối 4.4.2 bị bỏ do SocketError '</span><span class="sxs-lookup"><span data-stu-id="27a0a-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="27a0a-108">Lỗi trong trình xem xếp hàng của máy chủ tại chỗ đang gửi email đến sĩ quan 365-' 421 4.4.2 kết nối bị bỏ do SocketError '</span><span class="sxs-lookup"><span data-stu-id="27a0a-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="27a0a-109">Lỗi trong gửi [Nhật ký giao thức](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) đường kết nối trên máy chủ gửi email đến Office 365-TLS không thành công với SocketError lỗi</span><span class="sxs-lookup"><span data-stu-id="27a0a-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="27a0a-110">Lỗi trong Nhật ký gửi hoặc nhận giao thức đường kết nối-' 451 5.7.3 phải phát hành lệnh STARTTLS đầu tiên '</span><span class="sxs-lookup"><span data-stu-id="27a0a-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="27a0a-111">Nếu bạn gặp bất kỳ lỗi nào ở trên, hãy đảm bảo rằng máy chủ đang gửi hoặc nhận email đã bật TLS 1,2 bằng cách kiểm tra các khóa đăng ký sau đây-</span><span class="sxs-lookup"><span data-stu-id="27a0a-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="27a0a-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2 \ máy khách] **"DisabledByDefault" = DWORD: 00000000 "bật" = DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2 \ máy chủ] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001**</span><span class="sxs-lookup"><span data-stu-id="27a0a-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="27a0a-113">Nếu bạn thực hiện bất kỳ thay đổi nào trong các phím đăng ký ở trên để bật TLS 1,2, hãy khởi động lại máy chủ để các thay đổi có hiệu lực.</span><span class="sxs-lookup"><span data-stu-id="27a0a-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="27a0a-114">Ngoài ra, hãy đảm bảo bạn đã cài đặt các bản cập nhật Windows và Exchange mới nhất.</span><span class="sxs-lookup"><span data-stu-id="27a0a-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="27a0a-115">Để biết thêm thông tin, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="27a0a-115">For more information, see:</span></span>

- [<span data-ttu-id="27a0a-116">Hướng dẫn về Exchange Server TLS, phần 1: chuẩn bị sẵn sàng cho TLS 1,2-cộng đồng kỹ thuật của Microsoft</span><span class="sxs-lookup"><span data-stu-id="27a0a-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="27a0a-117">Phần hướng dẫn của Exchange Server TLS 2: bật TLS 1,2 và xác định khách hàng không sử dụng CNTT-cộng đồng kỹ thuật của Microsoft</span><span class="sxs-lookup"><span data-stu-id="27a0a-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="27a0a-118">Hiểu rõ tình huống email nếu không thể thỏa thuận Phiên bản TLS với Exchange Online-Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="27a0a-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
