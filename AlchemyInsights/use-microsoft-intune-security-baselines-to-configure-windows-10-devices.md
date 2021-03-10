---
title: Sử dụng trình nền bảo mật InTune của Microsoft để cấu hình thiết bị chạy Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696387"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="fea46-102">Sử dụng trình nền bảo mật InTune của Microsoft để cấu hình các thiết bị chạy Windows 10</span><span class="sxs-lookup"><span data-stu-id="fea46-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="fea46-103">InTune bảo mật, giúp bảo vệ người dùng và thiết bị.</span><span class="sxs-lookup"><span data-stu-id="fea46-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="fea46-104">Cấu hình bảo mật là các nhóm thiết đặt sẵn của Windows được dùng để áp dụng một nhóm thiết đặt đã biết và các giá trị mặc định được đề xuất bởi nhóm bảo mật liên quan.</span><span class="sxs-lookup"><span data-stu-id="fea46-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="fea46-105">Bằng cách tạo hồ sơ đường cơ sở bảo mật trong InTune, bạn tạo một mẫu bao gồm nhiều hồ sơ cấu hình thiết bị.</span><span class="sxs-lookup"><span data-stu-id="fea46-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="fea46-106">Khi bạn triển khai các cấu hình bảo mật cho các nhóm người dùng hoặc thiết bị, các thiết đặt sẽ được áp dụng cho các thiết bị chạy trên Windows 10 hoặc các phiên bản mới hơn.</span><span class="sxs-lookup"><span data-stu-id="fea46-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="fea46-107">Ví dụ: cơ sở tự động bảo mật quản lý thiết bị di động (MDM) của Microsoft (1) cho phép BitLocker cho ổ đĩa rời, (2) yêu cầu mật khẩu để mở khóa thiết bị và (3) vô hiệu hóa xác thực cơ bản.</span><span class="sxs-lookup"><span data-stu-id="fea46-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="fea46-108">Khi một giá trị mặc định không hoạt động cho môi trường của bạn, bạn có thể tùy chỉnh đường cơ sở để áp dụng các thiết đặt mà bạn cần.</span><span class="sxs-lookup"><span data-stu-id="fea46-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="fea46-109">Các đường căn bảo an cũng giúp thiết lập một dòng công việc bảo mật end-to-end trong Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="fea46-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="fea46-110">Sau đây là một số lợi ích của chức năng này:</span><span class="sxs-lookup"><span data-stu-id="fea46-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="fea46-111">Một đường cơ sở bảo mật bao gồm các biện pháp và đề xuất tốt nhất cho các thiết đặt ảnh hưởng đến bảo mật.</span><span class="sxs-lookup"><span data-stu-id="fea46-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="fea46-112">Vì InTune đối tác với nhóm bảo mật Windows tạo ra các đường lưới cho các chính sách nhóm, các khuyến nghị này dựa trên hướng dẫn vững chắc và trải nghiệm rộng rãi.</span><span class="sxs-lookup"><span data-stu-id="fea46-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="fea46-113">Nếu bạn mới dùng InTune và không chắc chắn bắt đầu từ đâu, sau đó sẽ giúp bạn nhanh chóng tạo và triển khai hồ sơ bảo mật.</span><span class="sxs-lookup"><span data-stu-id="fea46-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="fea46-114">Nếu bạn hiện đang sử dụng chính sách nhóm, sau đó di chuyển đến InTune cho các mục đích quản lý sẽ dễ dàng hơn nhiều so với các đường kết hợp bảo mật, bởi vì các đường cơ sở bảo mật này được tích hợp vào InTune và bao gồm các khả năng cắt cạnh để quản lý.</span><span class="sxs-lookup"><span data-stu-id="fea46-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="fea46-115">Để biết thêm thông tin, hãy xem bộ [phận bảo mật của Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) và [quản lý thiết bị di động](https://docs.microsoft.com/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="fea46-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>