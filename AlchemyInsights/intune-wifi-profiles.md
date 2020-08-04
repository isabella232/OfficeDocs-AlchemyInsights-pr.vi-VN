---
title: Cấu hình Wi-Fi InTune
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555819"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="54517-102">Cấu hình Wi-Fi InTune</span><span class="sxs-lookup"><span data-stu-id="54517-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="54517-103">Thực hiện thành công kết nối Wi-Fi cho MDM khách hàng phụ thuộc vào một chính xác triển khai hồ sơ phản ánh các yêu cầu của cơ sở hạ tầng Wi-Fi công ty.</span><span class="sxs-lookup"><span data-stu-id="54517-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="54517-104">Để xem lại các cài đặt thích hợp cho các nền tảng máy khách mà bạn đang điều tra:</span><span class="sxs-lookup"><span data-stu-id="54517-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="54517-105">Thêm cài đặt Wi-Fi cho các thiết bị chạy Android trong Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="54517-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="54517-106">Thêm cài đặt Wi-Fi cho Android Enterprise chuyên dụng và quản lý toàn bộ thiết bị trong Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="54517-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="54517-107">Thêm cài đặt Wi-Fi cho các thiết bị iOS và iPadOS trong Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="54517-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="54517-108">Thêm cài đặt Wi-Fi cho Windows 10 và các thiết bị sau trong InTune</span><span class="sxs-lookup"><span data-stu-id="54517-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="54517-109">Nhập cài đặt Wi-Fi cho các thiết bị Windows trong InTune</span><span class="sxs-lookup"><span data-stu-id="54517-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="54517-110">**Các vấn đề thường gặp**</span><span class="sxs-lookup"><span data-stu-id="54517-110">**Common Issues**</span></span>

<span data-ttu-id="54517-111">**Tôi đang triển khai hồ sơ Wi-Fi phụ thuộc vào chứng chỉ đã triển khai được chỉ định trong hồ sơ Wi-Fi. Tuy nhiên, Hồ sơ cấu hình đang hiển thị trạng thái lỗi.**</span><span class="sxs-lookup"><span data-stu-id="54517-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="54517-112">Kiểm tra xem thiết bị của bạn có nhận chứng chỉ hay không.</span><span class="sxs-lookup"><span data-stu-id="54517-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="54517-113">Trong InTune, đi tới **tất cả thiết bị** và chọn **cấu hình**thiết bị > thiết bị.</span><span class="sxs-lookup"><span data-stu-id="54517-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="54517-114">Kiểm tra tất cả các cấu hình dự kiến được liệt kê và ở trạng thái thành công.</span><span class="sxs-lookup"><span data-stu-id="54517-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="54517-115">Đối với hồ sơ Android, nếu bạn có chứng chỉ trung gian trong Chuỗi chứng chỉ của mình, hãy đảm bảo chúng được triển khai cho các thiết bị Android.</span><span class="sxs-lookup"><span data-stu-id="54517-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="54517-116">Để kiểm tra trạng thái chứng chỉ, hãy đi tới **cấu hình thiết bị**  >  **Profiles**  >  **Android trung gian ca**thuộc  >  **tính**  >  **tin cậy chứng chỉ**.</span><span class="sxs-lookup"><span data-stu-id="54517-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="54517-117">Nếu bạn tiếp tục thấy lỗi, hãy xem lại các quy trình và các phần khắc phục sự cố.</span><span class="sxs-lookup"><span data-stu-id="54517-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="54517-118">Để biết thêm thông tin, xem [tổng quan về khắc phục sự cố cấu hình chứng chỉ SCEP với Microsoft InTune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="54517-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="54517-119">**Tôi đã triển khai một cấu hình Wi-Fi cho một thiết bị. InTune Hiển thị rằng nó đã thành công, nhưng thiết bị không kết nối với Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="54517-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="54517-120">Trạng thái thành công có nghĩa là InTune đã triển khai thành công hồ sơ dưới dạng cấu hình.</span><span class="sxs-lookup"><span data-stu-id="54517-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="54517-121">Tuy nhiên, các cấu hình có thể không phù hợp với mạng của bạn và/hoặc yêu cầu xác thực.</span><span class="sxs-lookup"><span data-stu-id="54517-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="54517-122">Để biết thêm chi tiết về kết nối cố gắng, kiểm lại Nhật ký trong cơ sở hạ tầng và dịch vụ xác thực (trên bộ điều khiển điểm truy cập Wi-Fi và máy chủ NPS/Radius).</span><span class="sxs-lookup"><span data-stu-id="54517-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="54517-123">Bạn có thể phải làm việc với nhóm cơ sở hạ tầng mạng của mình hoặc nhà cung cấp Wi-Fi của bên thứ ba để thu thập và đánh giá Nhật ký.</span><span class="sxs-lookup"><span data-stu-id="54517-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>