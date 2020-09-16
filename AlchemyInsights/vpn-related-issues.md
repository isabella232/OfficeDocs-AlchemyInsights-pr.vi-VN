---
title: Các vấn đề liên quan đến VPN
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
- "1545"
- "9000076"
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726135"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="51823-102">Các vấn đề liên quan đến VPN</span><span class="sxs-lookup"><span data-stu-id="51823-102">VPN related issues</span></span>

<span data-ttu-id="51823-103">Việc thực hiện thành công các kết nối VPN cho máy khách MDM tùy thuộc vào một hồ sơ đã triển khai phản ánh chính xác các yêu cầu của cơ sở hạ tầng VPN.</span><span class="sxs-lookup"><span data-stu-id="51823-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="51823-104">Đối với các cài đặt phù hợp cho nền tảng máy khách mà bạn đang điều tra, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="51823-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="51823-105">Thiết đặt thiết bị trong Windows 10 và Windows Holographic để thêm kết nối VPN bằng cách dùng InTune</span><span class="sxs-lookup"><span data-stu-id="51823-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="51823-106">Thêm các thiết đặt VPN trên các thiết bị iOS và iPadOS trong Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="51823-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="51823-107">Thiết đặt thiết bị Android để cấu hình VPN trong InTune</span><span class="sxs-lookup"><span data-stu-id="51823-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="51823-108">Thêm các thiết đặt VPN trên thiết bị macOS trong Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="51823-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="51823-109">Nếu hồ sơ VPN của bạn sử dụng xác thực dựa trên chứng chỉ, hãy đảm bảo rằng các hồ sơ chứng nhận chứng chỉ gốc và xác thực máy khách được nối kết với hồ sơ VPN được triển khai thành công.</span><span class="sxs-lookup"><span data-stu-id="51823-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="51823-110">**Các sự cố phổ biến**</span><span class="sxs-lookup"><span data-stu-id="51823-110">**Common Issues**</span></span>

<span data-ttu-id="51823-111">**Tôi đã triển khai hồ sơ VPN vào một thiết bị. InTune Hiển thị rằng nó đã thành công, nhưng thiết bị không được kết nối với VPN.**</span><span class="sxs-lookup"><span data-stu-id="51823-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="51823-112">Trạng thái thành công nghĩa là InTune đã triển khai thành công hồ sơ như được cấu hình.</span><span class="sxs-lookup"><span data-stu-id="51823-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="51823-113">Tuy nhiên, các cấu hình này có thể không khớp với mạng của bạn và/hoặc các yêu cầu xác thực.</span><span class="sxs-lookup"><span data-stu-id="51823-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="51823-114">Xem lại Nhật ký trong cơ sở hạ tầng và dịch vụ xác thực (trên máy chủ VPN và NPS/Radius) để biết thêm chi tiết về kết nối đã thử.</span><span class="sxs-lookup"><span data-stu-id="51823-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="51823-115">Bạn có thể cần làm việc với nhóm cơ sở hạ tầng mạng của bạn hoặc nhà cung cấp VPN bên thứ ba, để thu thập và xem lại Nhật ký.</span><span class="sxs-lookup"><span data-stu-id="51823-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="51823-116">**Khi tôi cấu hình một VPN tùy chỉnh cho iOS, tính năng trên mỗi ứng dụng VPN không được tạo sẵn.**</span><span class="sxs-lookup"><span data-stu-id="51823-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="51823-117">VPN mỗi ứng dụng dành cho thiết bị iOS trong InTune hiện sẵn dùng cho một danh sách các nhà cung cấp và đối tác cụ thể, những người cũng phải đáp ứng các điều kiện tiên quyết chứng chỉ trước khi cấu hình VPN cho mỗi ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="51823-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="51823-118">Để biết thêm thông tin, hãy xem [thiết lập mạng riêng ảo trên mỗi ứng dụng (VPN) cho các thiết bị iOS/iPadOS trong InTune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="51823-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="51823-119">Để biết thêm thông tin về tất cả các loại kết nối VPN trong InTune, hãy xem [tạo hồ sơ VPN để kết nối với các máy chủ VPN trong InTune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="51823-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="51823-120">**VPN on-Demand VPN không được kích hoạt khi tên miền được đặt cấu hình được truy nhập**</span><span class="sxs-lookup"><span data-stu-id="51823-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="51823-121">Để kiểm tra các thiết đặt VPN tự động, hãy đặt các giá trị sau đây:</span><span class="sxs-lookup"><span data-stu-id="51823-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="51823-122">Tôi muốn thực hiện các thao tác sau: **đánh giá mỗi lần thử kết nối**</span><span class="sxs-lookup"><span data-stu-id="51823-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="51823-123">Chọn xem có kết nối không: **kết nối nếu cần thiết**</span><span class="sxs-lookup"><span data-stu-id="51823-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="51823-124">Khi người dùng truy nhập các tên miền này: *tên miền* **đích**</span><span class="sxs-lookup"><span data-stu-id="51823-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="51823-125">Nếu cấu hình trên không thành công, hãy thêm thành phần sau đây:</span><span class="sxs-lookup"><span data-stu-id="51823-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="51823-126">Khi URL này không thể truy cập, lực lượng kết nối VPN: **Badurl**</span><span class="sxs-lookup"><span data-stu-id="51823-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>