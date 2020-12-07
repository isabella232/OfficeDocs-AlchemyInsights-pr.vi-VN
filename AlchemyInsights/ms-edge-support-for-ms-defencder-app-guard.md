---
title: Hỗ trợ của Microsoft Edge cho bảo vệ ứng dụng Microsoft Defender
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584177"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="98e5c-102">Hỗ trợ của Microsoft Edge cho bảo vệ ứng dụng Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="98e5c-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="98e5c-103">Được thiết kế dành cho Windows 10 và Microsoft Edge, ứng dụng guard dùng phương pháp phân cách phần cứng cho phép người dùng dẫn hướng một site không đáng tin cậy từ bên trong bộ chứa siêu bị cô lập, Hyper-V – đã được phân tách khỏi hệ điều hành máy chủ lưu trữ.</span><span class="sxs-lookup"><span data-stu-id="98e5c-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="98e5c-104">Người quản trị doanh nghiệp xác định danh sách các website đáng tin cậy, tài nguyên điện toán đám mây và các mạng nội bộ.</span><span class="sxs-lookup"><span data-stu-id="98e5c-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="98e5c-105">Khi người dùng truy nhập vào một site không có trong danh sách, Microsoft Edge sẽ mở site đó trong bộ chứa.</span><span class="sxs-lookup"><span data-stu-id="98e5c-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="98e5c-106">Điều này có nghĩa là nếu site đó trở thành độc hại, máy tính lưu trữ sẽ vẫn được bảo vệ và kẻ tấn công sẽ không nhận được dữ liệu doanh nghiệp.</span><span class="sxs-lookup"><span data-stu-id="98e5c-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="98e5c-107">Việc cài đặt các phần mở rộng trong bộ chứa được hỗ trợ dưới dạng Microsoft Edge Phiên bản 81 và có thể điều khiển thông qua chính sách.</span><span class="sxs-lookup"><span data-stu-id="98e5c-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="98e5c-108">Địa chỉ updateURL được dùng trong chính sách ExtensionInstallForcelist sẽ được thêm vào như một nguồn tài nguyên trung lập trong các chính sách phân cách mạng được sử dụng bởi bộ bảo vệ ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="98e5c-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="98e5c-109">Để biết thêm thông tin, hãy xem [hỗ trợ Microsoft Edge cho bộ bảo vệ ứng dụng bảo vệ Microsoft](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="98e5c-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
