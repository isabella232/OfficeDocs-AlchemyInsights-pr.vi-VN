---
title: Khắc phục sự cố triển khai chứng chỉ xác thực máy khách
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555804"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="6d329-102">Khắc phục sự cố triển khai chứng chỉ xác thực máy khách</span><span class="sxs-lookup"><span data-stu-id="6d329-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="6d329-103">InTune NDES/SCEP và PKCS/PFX hồ sơ chứng chỉ máy khách thường được sử dụng kết hợp với các loại hồ sơ khác như WiFi, VPN và email cho phép người dùng xác thực với tài nguyên của công ty.</span><span class="sxs-lookup"><span data-stu-id="6d329-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="6d329-104">Khi các loại hồ sơ được liên kết với hồ sơ chứng chỉ máy khách phụ thuộc vào việc triển khai thành công hồ sơ đó.</span><span class="sxs-lookup"><span data-stu-id="6d329-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="6d329-105">Thiết lập cơ sở hạ tầng ban đầu và cấu hình liên quan của hồ sơ chứng chỉ máy khách thường yêu cầu khắc phục sự cố.</span><span class="sxs-lookup"><span data-stu-id="6d329-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="6d329-106">Để có hướng dẫn từng bước để thiết lập thành công kết nối NDES và khắc phục sự cố hướng dẫn để tách các vấn đề với triển khai chứng chỉ, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="6d329-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="6d329-107">Cấu hình cơ sở hạ tầng để hỗ trợ SCEP với InTune</span><span class="sxs-lookup"><span data-stu-id="6d329-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="6d329-108">Tổng quan về khắc phục sự cố cấu hình chứng chỉ SCEP với Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="6d329-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="6d329-109">Sử dụng tập lệnh PowerShell tham chiếu để giúp xác minh cấu hình của bạn.</span><span class="sxs-lookup"><span data-stu-id="6d329-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="6d329-110">Để biết thêm thông tin, xem [tập lệnh xác minh kết nối chứng chỉ InTune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="6d329-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="6d329-111">**Các vấn đề thường gặp khác**</span><span class="sxs-lookup"><span data-stu-id="6d329-111">**Other common issues**</span></span>

<span data-ttu-id="6d329-112">**Khi tôi cố gắng cài đặt kết nối InTune chứng chỉ trên máy chủ kết nối NDES, tôi nhận được thông báo "mật khẩu trong yêu cầu chứng chỉ không được xác minh. Nó có thể đã được sử dụng rồi. Lấy mật khẩu mới để gửi với yêu cầu này. "**</span><span class="sxs-lookup"><span data-stu-id="6d329-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="6d329-113">Thông báo này có nghĩa là bạn cần chạy cài đặt kết nối chứng chỉ là quản trị viên.</span><span class="sxs-lookup"><span data-stu-id="6d329-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="6d329-114">Trong một số môi trường, các máy chủ có chạy chứng chỉ InTune phải sử dụng máy chủ proxy để kết nối với InTune, và để kết nối chứng chỉ phải sử dụng proxy.</span><span class="sxs-lookup"><span data-stu-id="6d329-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="6d329-115">Trong một số trường hợp, kết nối NDES bỏ qua cài đặt proxy được cấu hình và có thể cần thiết để cấu hình thiết đặt ủy quyền trong khi chạy trong ngữ cảnh bảo mật của LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="6d329-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="6d329-116">Giải pháp là để chạy Internet Explorer như hệ thống và cấu hình một proxy trong IE.</span><span class="sxs-lookup"><span data-stu-id="6d329-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="6d329-117">Sau khi khởi động lại dịch vụ InTune Connector, kết nối NDES kết nối với InTune.</span><span class="sxs-lookup"><span data-stu-id="6d329-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="6d329-118">**Thiết bị người dùng không còn nhận được chứng chỉ SCEP từ NDES.**</span><span class="sxs-lookup"><span data-stu-id="6d329-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="6d329-119">Có thể chứng chỉ xác thực máy khách phát hành cho máy chủ NDES và được chỉ định trong quá trình cài đặt kết nối NDES, đã hết hạn hoặc bị thiếu.</span><span class="sxs-lookup"><span data-stu-id="6d329-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="6d329-120">Để giải quyết:</span><span class="sxs-lookup"><span data-stu-id="6d329-120">To resolve:</span></span> 
 
1. <span data-ttu-id="6d329-121">Dỡ cài đặt kết nối NDES.</span><span class="sxs-lookup"><span data-stu-id="6d329-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="6d329-122">Sử dụng các chi tiết để yêu cầu xác thực máy khách mới hoặc chứng chỉ xác thực máy chủ:</span><span class="sxs-lookup"><span data-stu-id="6d329-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="6d329-123">Tên chủ đề: CN = FQDN bên ngoài</span><span class="sxs-lookup"><span data-stu-id="6d329-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="6d329-124">Tên thay thế tiêu đề (cả hai đều bắt buộc): DNS = FQDN bên ngoài, DNS = FQDN nội bộ</span><span class="sxs-lookup"><span data-stu-id="6d329-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="6d329-125">Cài đặt lại kết nối NDES với chứng chỉ mới.</span><span class="sxs-lookup"><span data-stu-id="6d329-125">Reinstall the NDES connector with the new certificate.</span></span>