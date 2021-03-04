---
title: Lỗi đồng bộ hóa đăng ký thiết bị tự động của Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448944"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="facc3-102">Lỗi đồng bộ hóa đăng ký thiết bị tự động của Apple</span><span class="sxs-lookup"><span data-stu-id="facc3-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="facc3-103">"Chúng tôi đã phát hiện rằng bạn có một hoặc nhiều thẻ ADE/DEP nằm trong trạng thái lỗi.</span><span class="sxs-lookup"><span data-stu-id="facc3-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="facc3-104">Cho đến khi trạng thái lỗi được giải quyết cho từng mã thông báo bị ảnh hưởng, chức năng ADE sẽ không hoạt động như mong đợi. ".</span><span class="sxs-lookup"><span data-stu-id="facc3-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="facc3-105">Lỗi này có thể hiển thị trong một số cách bao gồm:</span><span class="sxs-lookup"><span data-stu-id="facc3-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="facc3-106">Các thiết bị có thể không đồng bộ từ ABM/ASM vào InTune</span><span class="sxs-lookup"><span data-stu-id="facc3-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="facc3-107">Các bài tập hồ sơ đăng ký có thể không</span><span class="sxs-lookup"><span data-stu-id="facc3-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="facc3-108">Thiết bị có thể không hoàn tất việc đăng ký ADE thành công</span><span class="sxs-lookup"><span data-stu-id="facc3-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="facc3-109">Kiểm tra lỗi đồng bộ được báo cáo trong bảng điều khiển InTune bên dưới **thiết bị > đăng ký thiết bị > các thẻ chương trình đăng ký > của Apple**.</span><span class="sxs-lookup"><span data-stu-id="facc3-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="facc3-110">Một trong những nguyên nhân phổ biến nhất của lỗi đồng bộ là hết hạn của mã thông báo hiện tại.</span><span class="sxs-lookup"><span data-stu-id="facc3-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="facc3-111">Trong nhiều trường hợp, việc gia hạn mã thông báo bị ảnh hưởng sẽ giải quyết được sự cố.</span><span class="sxs-lookup"><span data-stu-id="facc3-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="facc3-112">Nếu một hoặc nhiều thẻ của bạn đã hết hạn, hãy xem tài liệu sau đây để giúp bạn gia hạn chúng là phù hợp:</span><span class="sxs-lookup"><span data-stu-id="facc3-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="facc3-113">Gia hạn mã thông báo đăng ký thiết bị tự động</span><span class="sxs-lookup"><span data-stu-id="facc3-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="facc3-114">Ngoài ra, bạn có thể thấy các tài liệu sau đây để xem những điều chỉnh sửa tiềm ẩn cho các lỗi khác khiến đồng bộ hóa mã lỗi:</span><span class="sxs-lookup"><span data-stu-id="facc3-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="facc3-115">Lỗi đồng bộ ABM/ASM cho iOS/iPadOS và thẻ đăng ký thiết bị tự động macOS</span><span class="sxs-lookup"><span data-stu-id="facc3-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="facc3-116">Lỗi đồng bộ ABM/ASM cho iOS/iPadOS và thẻ đăng ký thiết bị tự động macOS</span><span class="sxs-lookup"><span data-stu-id="facc3-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
