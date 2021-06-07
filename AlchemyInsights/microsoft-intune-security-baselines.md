---
title: Sử dụng Microsoft Intune cơ sở bảo mật để đặt cấu hình cho các Windows 10 thiết bị
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794125"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="0d3ab-102">Sử dụng Microsoft Intune cơ sở bảo mật để đặt cấu hình cho các Windows 10 thiết bị</span><span class="sxs-lookup"><span data-stu-id="0d3ab-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="0d3ab-103">Đường cơ sở bảo mật intune giúp bảo vệ người dùng và thiết bị.</span><span class="sxs-lookup"><span data-stu-id="0d3ab-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="0d3ab-104">Đường cơ sở bảo mật là Windows đặt sẵn được dùng để áp dụng một nhóm thiết đặt đã biết và các giá trị mặc định do các nhóm bảo mật liên quan đề xuất.</span><span class="sxs-lookup"><span data-stu-id="0d3ab-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="0d3ab-105">Bằng cách tạo hồ sơ đường cơ sở bảo mật trong Intune, bạn tạo một mẫu bao gồm nhiều hồ sơ cấu hình thiết bị.</span><span class="sxs-lookup"><span data-stu-id="0d3ab-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="0d3ab-106">Khi bạn triển khai đường cơ sở bảo mật cho các nhóm người dùng hoặc thiết bị, thiết đặt được áp dụng cho các thiết bị chạy trên Windows 10 trở lên.</span><span class="sxs-lookup"><span data-stu-id="0d3ab-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="0d3ab-107">Ví dụ, đường cơ sở bảo mật quản lý thiết bị di động (MDM) của Microsoft tự động bật tính năng BitLocker cho ổ đĩa di động, yêu cầu mật khẩu để mở khóa thiết bị và tắt xác thực cơ bản.</span><span class="sxs-lookup"><span data-stu-id="0d3ab-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="0d3ab-108">Khi một giá trị mặc định không hoạt động đối với môi trường của bạn, bạn có thể tùy chỉnh đường cơ sở để áp dụng các thiết đặt mà bạn cần.</span><span class="sxs-lookup"><span data-stu-id="0d3ab-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="0d3ab-109">Đường cơ sở bảo mật cũng giúp thiết lập một dòng công việc bảo mật đầu cuối trong Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0d3ab-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="0d3ab-110">Đường cơ sở bảo mật bao gồm các phương pháp và đề xuất tốt nhất cho các cài đặt ảnh hưởng đến bảo mật.</span><span class="sxs-lookup"><span data-stu-id="0d3ab-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="0d3ab-111">Intune hợp tác với nhóm bảo mật Windows tạo đường cơ sở cho các chính sách nhóm, do đó, các đề xuất này dựa trên hướng dẫn đặc biệt và trải nghiệm chuyên sâu.</span><span class="sxs-lookup"><span data-stu-id="0d3ab-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="0d3ab-112">Nếu bạn mới sử dụng Intune và không chắc nên bắt đầu từ đâu, đường cơ sở bảo mật sẽ giúp bạn nhanh chóng tạo và triển khai hồ sơ bảo mật.</span><span class="sxs-lookup"><span data-stu-id="0d3ab-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="0d3ab-113">Nếu bạn hiện đang sử dụng chính sách nhóm, việc di chuyển sang Intune cho mục đích quản lý sẽ dễ dàng hơn nhiều với đường cơ sở bảo mật vì chúng được tích hợp vào Intune và bao gồm các chức năng quản lý tiên tiến.</span><span class="sxs-lookup"><span data-stu-id="0d3ab-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="0d3ab-114">Để tìm hiểu thêm, hãy xem [Windows cơ sở bảo mật và](/windows/security/threat-protection/windows-security-baselines) Quản lý thiết bị di [động](/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="0d3ab-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

