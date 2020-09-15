---
title: Khắc phục sự cố triển khai chứng chỉ xác thực khách
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659008"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="d1597-102">Khắc phục sự cố triển khai chứng chỉ xác thực khách</span><span class="sxs-lookup"><span data-stu-id="d1597-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="d1597-103">InTune NDES/SCEP và PKCS/PFX Client, Hồ sơ chứng chỉ được sử dụng thường xuyên cùng với các kiểu hồ sơ khác chẳng hạn như WiFi, VPN và email để cho phép người dùng xác thực đối với tài nguyên của công ty.</span><span class="sxs-lookup"><span data-stu-id="d1597-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="d1597-104">Khi các kiểu hồ sơ này được nối kết với hồ sơ chứng chỉ máy khách sẽ phụ thuộc vào việc triển khai thành công hồ sơ đó.</span><span class="sxs-lookup"><span data-stu-id="d1597-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="d1597-105">Thiết lập cơ sở hạ tầng ban đầu và cấu hình liên kết của hồ sơ chứng chỉ máy khách thường bắt buộc khắc phục sự cố.</span><span class="sxs-lookup"><span data-stu-id="d1597-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="d1597-106">Để có hướng dẫn từng bước để thiết lập thành công của trình kết nối NDES và hướng dẫn khắc phục sự cố để tách biệt các vấn đề với triển khai chứng chỉ, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="d1597-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="d1597-107">Cấu hình cơ sở hạ tầng để hỗ trợ SCEP bằng InTune</span><span class="sxs-lookup"><span data-stu-id="d1597-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="d1597-108">Tổng quan về khắc phục sự cố các hồ sơ chứng chỉ SCEP với Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="d1597-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="d1597-109">Sử dụng các tập lệnh PowerShell được tham chiếu để giúp xác minh cấu hình của bạn.</span><span class="sxs-lookup"><span data-stu-id="d1597-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="d1597-110">Để biết thêm thông tin, hãy xem [script xác minh trình kết nối InTune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="d1597-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="d1597-111">**Các vấn đề phổ biến khác**</span><span class="sxs-lookup"><span data-stu-id="d1597-111">**Other common issues**</span></span>

<span data-ttu-id="d1597-112">**Khi tôi tìm cách cài đặt trình kết nối chứng chỉ InTune trên máy chủ kết nối NDES, tôi nhận được thông báo, "mật khẩu trong yêu cầu chứng chỉ không thể được xác nhận. Có thể nó đã được sử dụng. Lấy mật khẩu mới để gửi yêu cầu này. "**</span><span class="sxs-lookup"><span data-stu-id="d1597-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="d1597-113">Thông báo này có nghĩa là bạn cần chạy cài đặt trình kết nối chứng chỉ với tư cách là người quản trị.</span><span class="sxs-lookup"><span data-stu-id="d1597-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="d1597-114">Trong một số môi trường, các máy chủ có chứng chỉ InTune chạy phải sử dụng máy chủ proxy để kết nối với InTune, và vì vậy trình kết nối chứng chỉ phải sử dụng proxy.</span><span class="sxs-lookup"><span data-stu-id="d1597-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="d1597-115">Trong một số trường hợp, đường kết nối NDES bỏ qua thiết đặt proxy được cấu hình và có thể là cần thiết để cấu hình các thiết đặt proxy trong khi đang chạy trong ngữ cảnh bảo mật của LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="d1597-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="d1597-116">Giải pháp là chạy Internet Explorer dưới dạng hệ thống và đặt cấu hình proxy trong IE.</span><span class="sxs-lookup"><span data-stu-id="d1597-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="d1597-117">Sau khi khởi động lại dịch vụ kết nối InTune, đường kết nối NDES sẽ kết nối đến InTune.</span><span class="sxs-lookup"><span data-stu-id="d1597-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="d1597-118">**Thiết bị người dùng không còn nhận được chứng chỉ SCEP từ NDES.**</span><span class="sxs-lookup"><span data-stu-id="d1597-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="d1597-119">Có thể là chứng chỉ xác thực máy khách đã phát hành với máy chủ NDES và đã xác định trong quá trình cài đặt kết nối NDES, đã hết hạn hoặc bị thiếu.</span><span class="sxs-lookup"><span data-stu-id="d1597-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="d1597-120">Để giải quyết:</span><span class="sxs-lookup"><span data-stu-id="d1597-120">To resolve:</span></span> 
 
1. <span data-ttu-id="d1597-121">Gỡ cài đặt trình kết nối NDES.</span><span class="sxs-lookup"><span data-stu-id="d1597-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="d1597-122">Sử dụng các chi tiết này để yêu cầu chứng chỉ xác thực máy khách mới hoặc chứng thực máy chủ:</span><span class="sxs-lookup"><span data-stu-id="d1597-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="d1597-123">Tên chủ đề: CN = bên ngoài FQDN</span><span class="sxs-lookup"><span data-stu-id="d1597-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="d1597-124">Chủ đề tên thay thế (cả hai đều bắt buộc): DNS = bên ngoài FQDN, DNS = FQDN nội bộ</span><span class="sxs-lookup"><span data-stu-id="d1597-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="d1597-125">Cài đặt lại trình kết nối NDES với chứng chỉ mới.</span><span class="sxs-lookup"><span data-stu-id="d1597-125">Reinstall the NDES connector with the new certificate.</span></span>