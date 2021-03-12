---
title: Tạo các chính sách và hồ sơ InTune
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: af8f1a3dfaccaca52f187f387274d63b22631b2d
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704664"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="d8941-102">Tạo chính sách và hồ sơ InTune</span><span class="sxs-lookup"><span data-stu-id="d8941-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="d8941-103">Trong InTune, bạn có thể tạo các chính sách và hồ sơ làm những việc khác nhau.</span><span class="sxs-lookup"><span data-stu-id="d8941-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="d8941-104">**Hồ sơ đăng** ký: preconfigure thiết bị của bạn theo nền tảng, cho phép người dùng quan hệ, sử dụng xác thực đa yếu tố và nhiều hơn nữa.</span><span class="sxs-lookup"><span data-stu-id="d8941-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="d8941-105">[Đăng ký thiết bị là gì](https://docs.microsoft.com/intune/device-enrollment)và tạo hồ sơ đăng ký cho [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll)và [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) là các nguồn tài nguyên tốt.</span><span class="sxs-lookup"><span data-stu-id="d8941-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="d8941-106">**Chính sách tuân thủ**: xác định quy tắc và cài đặt các thiết bị mà phải tuân theo để phù hợp.</span><span class="sxs-lookup"><span data-stu-id="d8941-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="d8941-107">Bạn cũng có thể sử dụng chính sách tuân thủ để giám sát thiết bị và thông báo cho người dùng không tuân thủ.</span><span class="sxs-lookup"><span data-stu-id="d8941-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="d8941-108">Bắt đầu với [chính sách tuân thủ thiết bị](https://docs.microsoft.com/intune/device-compliance-get-started).</span><span class="sxs-lookup"><span data-stu-id="d8941-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="d8941-109">**Chính sách truy nhập** có điều kiện: giúp bảo mật tài nguyên tổ chức, tùy thuộc vào các điều kiện bạn nhập.</span><span class="sxs-lookup"><span data-stu-id="d8941-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="d8941-110">Ví dụ: đối với các thiết bị không tuân thủ, hãy sử dụng quyền truy nhập có điều kiện để hạn chế quyền truy nhập vào email và SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d8941-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="d8941-111">[Truy nhập có điều kiện](https://docs.microsoft.com/intune/conditional-access) và những [cách phổ biến để sử dụng quyền truy nhập](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) có điều kiện là các nguồn tài nguyên tốt để bắt đầu.</span><span class="sxs-lookup"><span data-stu-id="d8941-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="d8941-112">**Cấu hình hồ sơ**: quản lý các tính năng và thiết đặt trên thiết bị, bao gồm các thiết đặt email, thêm một mạng WiFi, sử dụng các mẫu dựng sẵn, điều khiển iOS và các tính năng thiết bị macOS và nhiều hơn nữa.</span><span class="sxs-lookup"><span data-stu-id="d8941-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="d8941-113">Bắt đầu tại [hồ sơ cấu hình thiết bị](https://docs.microsoft.com/intune/device-profiles).</span><span class="sxs-lookup"><span data-stu-id="d8941-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="d8941-114">Liên kết hữu ích:</span><span class="sxs-lookup"><span data-stu-id="d8941-114">Helpful links:</span></span>

- [<span data-ttu-id="d8941-115">Các câu hỏi thường gặp, sự cố và độ phân giải với chính sách và hồ sơ của thiết bị trong InTune</span><span class="sxs-lookup"><span data-stu-id="d8941-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="d8941-116">Khắc phục sự cố các chính sách và hồ sơ trong InTune</span><span class="sxs-lookup"><span data-stu-id="d8941-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)
