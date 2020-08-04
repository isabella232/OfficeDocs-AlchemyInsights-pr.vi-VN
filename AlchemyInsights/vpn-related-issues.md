---
title: Các vấn đề liên quan đến VPN
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555740"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="24b42-102">Các vấn đề liên quan đến VPN</span><span class="sxs-lookup"><span data-stu-id="24b42-102">VPN related issues</span></span>

<span data-ttu-id="24b42-103">Thực hiện thành công kết nối VPN cho khách hàng MDM phụ thuộc vào hồ sơ triển khai đúng phản ánh các yêu cầu của cơ sở hạ tầng VPN.</span><span class="sxs-lookup"><span data-stu-id="24b42-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="24b42-104">Đối với các thiết đặt thích hợp cho các nền tảng máy khách mà bạn đang điều tra, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="24b42-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="24b42-105">Cài đặt thiết bị Windows 10 và Windows Holographic để thêm các kết nối VPN bằng InTune</span><span class="sxs-lookup"><span data-stu-id="24b42-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="24b42-106">Thêm cài đặt VPN trên các thiết bị iOS và iPadOS trong Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="24b42-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="24b42-107">Cài đặt thiết bị Android để cấu hình VPN trong InTune</span><span class="sxs-lookup"><span data-stu-id="24b42-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="24b42-108">Thêm cài đặt VPN trên các thiết bị macOS trong Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="24b42-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="24b42-109">Nếu cấu hình VPN của bạn sử dụng xác thực dựa trên chứng chỉ, hãy đảm bảo rằng chứng chỉ gốc và hồ sơ chứng chỉ xác thực máy khách được liên kết đến cấu hình VPN đang triển khai thành công.</span><span class="sxs-lookup"><span data-stu-id="24b42-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="24b42-110">**Các vấn đề thường gặp**</span><span class="sxs-lookup"><span data-stu-id="24b42-110">**Common Issues**</span></span>

<span data-ttu-id="24b42-111">**Tôi đã triển khai một cấu hình VPN đến một thiết bị. InTune Hiển thị rằng nó đã thành công, nhưng thiết bị không kết nối với VPN.**</span><span class="sxs-lookup"><span data-stu-id="24b42-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="24b42-112">Trạng thái thành công có nghĩa là InTune đã triển khai thành công hồ sơ dưới dạng cấu hình.</span><span class="sxs-lookup"><span data-stu-id="24b42-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="24b42-113">Tuy nhiên, các cấu hình có thể không phù hợp với mạng của bạn và/hoặc yêu cầu xác thực.</span><span class="sxs-lookup"><span data-stu-id="24b42-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="24b42-114">Đánh giá Nhật ký trong cơ sở hạ tầng và dịch vụ xác thực (trên máy chủ VPN và máy chủ NPS/Radius) để biết thêm chi tiết về kết nối cố gắng.</span><span class="sxs-lookup"><span data-stu-id="24b42-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="24b42-115">Bạn có thể cần phải làm việc với nhóm cơ sở hạ tầng mạng của mình hoặc nhà cung cấp VPN bên thứ ba để thu thập và đánh giá các bản ghi.</span><span class="sxs-lookup"><span data-stu-id="24b42-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="24b42-116">**Khi tôi đặt cấu hình VPN tùy chỉnh cho iOS, tính năng VPN cho mỗi ứng dụng không có sẵn.**</span><span class="sxs-lookup"><span data-stu-id="24b42-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="24b42-117">Mỗi ứng dụng VPN cho các thiết bị iOS trong InTune hiện có sẵn cho một danh sách cụ thể của các nhà cung cấp và đối tác, những người cũng phải đáp ứng các điều kiện tiên quyết của chứng chỉ trước khi cấu hình một VPN cho mỗi ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="24b42-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="24b42-118">Để biết thêm thông tin, xem [thiết lập một ứng dụng Virtual Private Network (VPN) cho các thiết bị iOS/iPadOS trong InTune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="24b42-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="24b42-119">Để biết thêm thông tin về tất cả các loại kết nối VPN trong InTune, xem [tạo cấu hình VPN để kết nối với các máy chủ VPN trong InTune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="24b42-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="24b42-120">**VPN theo yêu cầu iOS không kích hoạt khi truy cập một miền được cấu hình**</span><span class="sxs-lookup"><span data-stu-id="24b42-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="24b42-121">Để kiểm tra cài đặt VPN tự động, hãy đặt các giá trị sau:</span><span class="sxs-lookup"><span data-stu-id="24b42-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="24b42-122">Tôi muốn làm như sau: đánh **giá từng nỗ lực kết nối**</span><span class="sxs-lookup"><span data-stu-id="24b42-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="24b42-123">Chọn có kết nối hay không: **kết nối nếu cần**</span><span class="sxs-lookup"><span data-stu-id="24b42-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="24b42-124">Khi người dùng truy cập vào các miền này: *tên miền* **đích**</span><span class="sxs-lookup"><span data-stu-id="24b42-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="24b42-125">Nếu cấu hình trên không thành công, thêm các yếu tố sau:</span><span class="sxs-lookup"><span data-stu-id="24b42-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="24b42-126">Khi URL này không thể truy cập, buộc kết nối VPN: **Badurl**</span><span class="sxs-lookup"><span data-stu-id="24b42-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>