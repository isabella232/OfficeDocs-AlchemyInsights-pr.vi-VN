---
title: Lỗi đồng bộ hóa đăng ký thiết bị tự động của Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714970"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="60627-102">Lỗi đồng bộ hóa đăng ký thiết bị tự động của Apple</span><span class="sxs-lookup"><span data-stu-id="60627-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="60627-103">"Chúng tôi đã phát hiện rằng bạn có một hoặc nhiều thẻ ADE/DEP nằm trong trạng thái lỗi.</span><span class="sxs-lookup"><span data-stu-id="60627-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="60627-104">Cho đến khi trạng thái lỗi được giải quyết cho từng mã thông báo bị ảnh hưởng, hàm ADE sẽ không hoạt động cho cùng ".</span><span class="sxs-lookup"><span data-stu-id="60627-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="60627-105">Lỗi này có thể hiển thị trong một số cách bao gồm:</span><span class="sxs-lookup"><span data-stu-id="60627-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="60627-106">Các thiết bị có thể không đồng bộ từ ABM/ASM vào InTune</span><span class="sxs-lookup"><span data-stu-id="60627-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="60627-107">Các bài tập hồ sơ đăng ký có thể không</span><span class="sxs-lookup"><span data-stu-id="60627-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="60627-108">Thiết bị có thể không hoàn tất việc đăng ký ADE thành công</span><span class="sxs-lookup"><span data-stu-id="60627-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="60627-109">Kiểm tra lỗi đồng bộ được báo cáo trong bảng điều khiển InTune bên dưới **thiết bị > đăng ký thiết bị > các thẻ chương trình** ghi danh > và xem lại các tài liệu hướng dẫn sau đây để xem bất kỳ việc khắc phục tiềm ẩn nào:</span><span class="sxs-lookup"><span data-stu-id="60627-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="60627-110">Lỗi đồng bộ ABM/ASM cho iOS/iPadOS và thẻ đăng ký thiết bị tự động macOS</span><span class="sxs-lookup"><span data-stu-id="60627-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
