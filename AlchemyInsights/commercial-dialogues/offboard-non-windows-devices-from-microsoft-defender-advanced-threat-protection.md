---
title: Các thiết bị không phải Windows không có từ bộ bảo vệ mối đe dọa nâng cao của Microsoft Defender (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748488"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="39e89-102">Các thiết bị không phải Windows không có từ bộ bảo vệ mối đe dọa nâng cao của Microsoft Defender (ATP)</span><span class="sxs-lookup"><span data-stu-id="39e89-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="39e89-103">Dưới đây là cách thực hiện:</span><span class="sxs-lookup"><span data-stu-id="39e89-103">Here's how:</span></span>

1. <span data-ttu-id="39e89-104">Hãy làm theo các tài liệu hướng dẫn bên thứ ba để ngắt kết nối giải pháp bên thứ ba từ Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="39e89-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="39e89-105">Từ đối tượng thuê Azure Active Directory của bạn, hãy loại bỏ quyền cho giải pháp của bên thứ ba:</span><span class="sxs-lookup"><span data-stu-id="39e89-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="39e89-106">Đăng nhập vào [cổng thông tin Azure](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="39e89-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="39e89-107">Chọn **tất cả**  >  các ứng dụng dịch vụ **Azure Active Directory**  >  **Enterprise**.</span><span class="sxs-lookup"><span data-stu-id="39e89-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="39e89-108">Chọn ứng dụng bạn muốn offboard.</span><span class="sxs-lookup"><span data-stu-id="39e89-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="39e89-109">Chọn **xóa**.</span><span class="sxs-lookup"><span data-stu-id="39e89-109">Select **Delete**.</span></span>

<span data-ttu-id="39e89-110">Để tìm hiểu thêm, hãy xem các [thiết bị không](https://go.microsoft.com/fwlink/?linkid=2143630)phải của Windows.</span><span class="sxs-lookup"><span data-stu-id="39e89-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
