---
title: Các hồ sơ Wi-Fi InTune
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
- "1548"
- "9000076"
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696283"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="e34f8-102">Các hồ sơ Wi-Fi InTune</span><span class="sxs-lookup"><span data-stu-id="e34f8-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="e34f8-103">Việc thực hiện thành công kết nối Wi-Fi cho máy khách MDM tùy thuộc vào một hồ sơ được triển khai chính xác phản ánh các yêu cầu của cơ sở hạ tầng Wi-Fi của công ty.</span><span class="sxs-lookup"><span data-stu-id="e34f8-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="e34f8-104">Để xem lại các thiết đặt phù hợp cho nền tảng máy khách mà bạn đang điều tra, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="e34f8-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="e34f8-105">Thêm thiết đặt Wi-Fi cho các thiết bị chạy Android trong Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="e34f8-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="e34f8-106">Thêm các thiết đặt Wi-Fi cho thiết bị Android dành riêng và được quản lý đầy đủ trong Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="e34f8-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="e34f8-107">Thêm thiết đặt Wi-Fi cho các thiết bị iOS và iPadOS trong Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="e34f8-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="e34f8-108">Thêm thiết đặt Wi-Fi cho Windows 10 và các thiết bị sau này trong InTune</span><span class="sxs-lookup"><span data-stu-id="e34f8-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="e34f8-109">Nhập thiết đặt Wi-Fi cho thiết bị Windows trong InTune</span><span class="sxs-lookup"><span data-stu-id="e34f8-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="e34f8-110">**Các sự cố phổ biến**</span><span class="sxs-lookup"><span data-stu-id="e34f8-110">**Common Issues**</span></span>

<span data-ttu-id="e34f8-111">**Tôi đang triển khai hồ sơ Wi-Fi phụ thuộc vào chứng chỉ được triển khai được xác định trong hồ sơ Wi-Fi. Tuy nhiên, Hồ sơ cấu hình sẽ hiển thị trạng thái lỗi.**</span><span class="sxs-lookup"><span data-stu-id="e34f8-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="e34f8-112">Kiểm tra xem thiết bị của bạn đã nhận được chứng chỉ không.</span><span class="sxs-lookup"><span data-stu-id="e34f8-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="e34f8-113">Trong InTune, đi tới **tất cả các thiết bị** và chọn thiết bị > **cấu hình thiết bị**.</span><span class="sxs-lookup"><span data-stu-id="e34f8-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="e34f8-114">Kiểm tra xem tất cả hồ sơ dự kiến đều được liệt kê và trong trạng thái thành công.</span><span class="sxs-lookup"><span data-stu-id="e34f8-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="e34f8-115">Đối với một hồ sơ Android, nếu bạn có chứng chỉ trung bình trong Chuỗi chứng chỉ, hãy đảm bảo rằng chúng được triển khai cho các thiết bị chạy Android.</span><span class="sxs-lookup"><span data-stu-id="e34f8-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="e34f8-116">Để kiểm tra trạng thái chứng chỉ, đi tới hồ sơ **cấu hình thiết bị**  >  **Profiles**  >  **Android Trung**bình  >  **tài sản**được  >  **chứng nhận tin cậy**.</span><span class="sxs-lookup"><span data-stu-id="e34f8-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="e34f8-117">Nếu bạn tiếp tục thấy lỗi, hãy xem lại các thủ tục và các phần khắc phục sự cố.</span><span class="sxs-lookup"><span data-stu-id="e34f8-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="e34f8-118">Để biết thêm thông tin, hãy xem [tổng quan về khắc phục sự cố các hồ sơ chứng chỉ SCEP với Microsoft InTune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="e34f8-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="e34f8-119">**Tôi đã triển khai hồ sơ Wi-Fi vào một thiết bị. InTune Hiển thị rằng nó đã thành công nhưng thiết bị không được kết nối với Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="e34f8-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="e34f8-120">Trạng thái thành công nghĩa là InTune đã triển khai thành công hồ sơ như được cấu hình.</span><span class="sxs-lookup"><span data-stu-id="e34f8-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="e34f8-121">Tuy nhiên, các cấu hình này có thể không khớp với mạng của bạn và/hoặc các yêu cầu xác thực.</span><span class="sxs-lookup"><span data-stu-id="e34f8-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="e34f8-122">Để biết thêm chi tiết về kết nối đã thử, hãy xem lại Nhật ký trong cơ sở hạ tầng và dịch vụ xác thực (trên bộ điều khiển điểm truy nhập Wi-Fi và máy chủ NPS/Radius).</span><span class="sxs-lookup"><span data-stu-id="e34f8-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="e34f8-123">Bạn có thể phải làm việc với nhóm cơ sở hạ tầng mạng của bạn hoặc nhà cung cấp Wi-Fi bên thứ ba, để thu thập và xem lại Nhật ký.</span><span class="sxs-lookup"><span data-stu-id="e34f8-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>