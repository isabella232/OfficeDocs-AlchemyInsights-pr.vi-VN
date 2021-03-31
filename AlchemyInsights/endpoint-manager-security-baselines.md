---
title: Trình quản lý điểm cuối-đường cơ sở bảo mật
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440915"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="f6c17-102">Trình quản lý điểm cuối-đường cơ sở bảo mật</span><span class="sxs-lookup"><span data-stu-id="f6c17-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="f6c17-103">Các cấu hình bảo mật được các nhóm thiết đặt sẵn của Windows giúp bạn áp dụng các thiết đặt bảo mật được đề xuất bởi nhóm bảo mật liên quan.</span><span class="sxs-lookup"><span data-stu-id="f6c17-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="f6c17-104">Những đường kết nối này có thể được tùy chỉnh để chỉ cung cấp các thiết đặt và giá trị mong muốn.</span><span class="sxs-lookup"><span data-stu-id="f6c17-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="f6c17-105">Để biết thêm thông tin về cấu hình bảo mật, hãy xem sử dụng các máy tính [bảo mật để cấu hình thiết bị chạy Windows 10 trong InTune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="f6c17-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="f6c17-106">Hiện tại có những đường cơ sở cho những sản phẩm này:</span><span class="sxs-lookup"><span data-stu-id="f6c17-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="f6c17-107">Thiết đặt bảo mật Windows MDM</span><span class="sxs-lookup"><span data-stu-id="f6c17-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="f6c17-108">Microsoft Defender cho bảo mật điểm cuối</span><span class="sxs-lookup"><span data-stu-id="f6c17-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="f6c17-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="f6c17-109">Microsoft Edge</span></span>

<span data-ttu-id="f6c17-110">Mỗi đường cơ sở được Cập Nhật theo định kỳ và được phát hành trong các phiên bản gia tăng.</span><span class="sxs-lookup"><span data-stu-id="f6c17-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="f6c17-111">Mỗi phiên bản thêm và loại bỏ các thiết đặt từ phiên bản trước đó để đảm bảo rằng đường cơ sở gặp phải hướng dẫn hiện tại.</span><span class="sxs-lookup"><span data-stu-id="f6c17-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="f6c17-112">Giao diện người dùng bảo mật trong Endpoint Security cho phép các phiên bản khác nhau được so sánh bằng cách thực hiện các thay đổi từ phiên bản sang phiên bản Hiển thị.</span><span class="sxs-lookup"><span data-stu-id="f6c17-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="f6c17-113">Để biết hướng dẫn về cách thay đổi hiệu quả nhất mà phiên bản của đường cơ sở được triển khai, hãy xem [quản lý hồ sơ đường cơ sở bảo mật trong Microsoft InTune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="f6c17-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="f6c17-114">Sau khi triển khai một đường cơ sở bảo mật, bạn có thể theo dõi các thiết đặt trạng thái triển khai và xem lại trên cơ sở thiết bị theo từng thiết bị.</span><span class="sxs-lookup"><span data-stu-id="f6c17-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="f6c17-115">**Lưu ý:** Dữ liệu báo cáo cho các máy tính có thể mất tối đa 24 giờ để xuất hiện từ triển khai ban đầu cho một thiết bị và tối đa 6 giờ để biết thêm các bản Cập Nhật.</span><span class="sxs-lookup"><span data-stu-id="f6c17-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="f6c17-116">Nguyên nhân phổ biến nhất của một thiết đặt đường cơ sở không áp dụng được vì cùng một thiết đặt đang được dùng trong một hồ sơ khác.</span><span class="sxs-lookup"><span data-stu-id="f6c17-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="f6c17-117">Tình huống này có thể được điều tra cho thiết bị cụ thể bằng cách chọn thiết bị đó từ bên trong nút trạng thái thiết bị của hồ sơ cơ sở bảo mật.</span><span class="sxs-lookup"><span data-stu-id="f6c17-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="f6c17-118">Để biết chi tiết, hãy xem [giải quyết xung đột cho](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)các đường cơ sở bảo mật.</span><span class="sxs-lookup"><span data-stu-id="f6c17-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>