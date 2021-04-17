---
title: Trung tâm quản trị nhóm
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826401"
---
# <a name="teams-admin-center"></a><span data-ttu-id="b6f89-102">Trung tâm quản trị nhóm</span><span class="sxs-lookup"><span data-stu-id="b6f89-102">Teams Admin Center</span></span>

<span data-ttu-id="b6f89-103">Tìm hiểu về quản lý nhóm với [Trung tâm quản trị nhóm](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="b6f89-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="b6f89-104">Nếu bạn không thể truy nhập vào Trung tâm quản trị nhóm, vui lòng kiểm tra các mục sau đây:</span><span class="sxs-lookup"><span data-stu-id="b6f89-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="b6f89-105">Xác nhận rằng bạn đã cho phép các [địa chỉ IP của Office 365 và URL](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) phù hợp trên mọi thiết bị chu vi (tường lửa, v.v.) hoặc trong các quy tắc tường lửa trên máy cục bộ của bạn.</span><span class="sxs-lookup"><span data-stu-id="b6f89-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="b6f89-106">Xác nhận rằng bạn đang sử dụng đăng nhập để truy nhập vào cổng thông tin quản trị nhóm khớp với tên người dùng của bạn được liệt kê trong [cổng thông tin quản trị Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="b6f89-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="b6f89-107">Nếu người dùng không xuất hiện trong Trung tâm quản trị nhóm, vui lòng kiểm tra như sau:</span><span class="sxs-lookup"><span data-stu-id="b6f89-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="b6f89-108">Bạn đã tạo người dùng hoặc giấy phép đã gán trong 24 giờ qua không?</span><span class="sxs-lookup"><span data-stu-id="b6f89-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="b6f89-109">Vui lòng đảm bảo bạn chờ ít nhất 24 giờ trước khi mở một vé hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="b6f89-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="b6f89-110">Xác minh bạn đã gán giấy phép thích hợp?</span><span class="sxs-lookup"><span data-stu-id="b6f89-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="b6f89-111">Nếu bạn có một Active Directory tại chỗ, hãy xác minh rằng [giá trị của Msrtcpc-PrimaryUserAddress hoặc địa chỉ SIP trong trường ProxyAddresses trong Active Directory địa phương của bạn là duy nhất và định dạng khớp với](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) SIP:**tên** người dùng từ [trung tâm quản trị Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="b6f89-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="b6f89-112">Nếu bạn dự định giữ lại triển khai Skype for Business Server và có người dùng lưu trữ tại cơ sở và trực tuyến: Hãy làm theo các **nhóm "thiết lập kết hợp với nhóm và Skype for Business Online"** trong Pa-nen điều khiển máy chủ Skype for Business của bạn và di chuyển người dùng trực tuyến.</span><span class="sxs-lookup"><span data-stu-id="b6f89-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
