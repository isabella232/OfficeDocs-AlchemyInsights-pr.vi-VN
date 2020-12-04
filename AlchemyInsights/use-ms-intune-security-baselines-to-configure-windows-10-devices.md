---
title: Sử dụng cấu hình bảo mật của Microsoft InTune để cấu hình thiết bị chạy Windows 10
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573783"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="90dd3-102">Sử dụng cấu hình bảo mật của Microsoft InTune để cấu hình thiết bị chạy Windows 10</span><span class="sxs-lookup"><span data-stu-id="90dd3-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="90dd3-103">InTune bảo mật, giúp bảo vệ người dùng và thiết bị.</span><span class="sxs-lookup"><span data-stu-id="90dd3-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="90dd3-104">Cấu hình bảo mật là các nhóm thiết đặt sẵn của Windows được dùng để áp dụng một nhóm thiết đặt đã biết và các giá trị mặc định được đề xuất bởi nhóm bảo mật liên quan.</span><span class="sxs-lookup"><span data-stu-id="90dd3-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="90dd3-105">Bằng cách tạo hồ sơ đường cơ sở bảo mật trong InTune, bạn tạo một mẫu bao gồm nhiều hồ sơ cấu hình thiết bị.</span><span class="sxs-lookup"><span data-stu-id="90dd3-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="90dd3-106">Khi bạn triển khai các cấu hình bảo mật cho các nhóm người dùng hoặc thiết bị, các thiết đặt sẽ được áp dụng cho các thiết bị chạy trên Windows 10 trở lên.</span><span class="sxs-lookup"><span data-stu-id="90dd3-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="90dd3-107">Ví dụ: MDM Security Baseline tự động (1) cho phép BitLocker cho ổ đĩa rời, (2) yêu cầu mật khẩu để mở khóa thiết bị và (3) vô hiệu hóa xác thực cơ bản.</span><span class="sxs-lookup"><span data-stu-id="90dd3-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="90dd3-108">Khi một giá trị mặc định không hoạt động cho môi trường của bạn, hãy tùy chỉnh đường cơ sở để áp dụng các thiết đặt mà bạn cần.</span><span class="sxs-lookup"><span data-stu-id="90dd3-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="90dd3-109">Các đường căn bảo an cũng giúp thiết lập một dòng công việc bảo mật end-to-end trong Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="90dd3-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="90dd3-110">Sau đây là một số lợi ích của việc này:</span><span class="sxs-lookup"><span data-stu-id="90dd3-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="90dd3-111">Một đường cơ sở bảo mật bao gồm các biện pháp và đề xuất tốt nhất cho các thiết đặt ảnh hưởng đến bảo mật.</span><span class="sxs-lookup"><span data-stu-id="90dd3-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="90dd3-112">Vì InTune đối tác với nhóm bảo mật Windows tạo ra các đường lưới cho các chính sách nhóm, các khuyến nghị này dựa trên hướng dẫn vững chắc và trải nghiệm rộng rãi.</span><span class="sxs-lookup"><span data-stu-id="90dd3-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="90dd3-113">Nếu bạn mới dùng InTune và không chắc chắn bắt đầu từ đâu, sau đó sẽ giúp bạn nhanh chóng tạo và triển khai hồ sơ bảo mật.</span><span class="sxs-lookup"><span data-stu-id="90dd3-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="90dd3-114">Nếu bạn hiện đang sử dụng chính sách nhóm, sau đó di chuyển đến InTune cho mục đích quản lý dễ dàng hơn nhiều so với các đường cơ bản, vì chúng được tích hợp vào InTune và bao gồm các khả năng cắt cạnh để quản lý.</span><span class="sxs-lookup"><span data-stu-id="90dd3-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="90dd3-115">Để tìm hiểu thêm, hãy xem các đường cơ sở [bảo mật của Windows](https://go.microsoft.com/fwlink/?linkid=2141503) và [quản lý thiết bị di động](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="90dd3-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>