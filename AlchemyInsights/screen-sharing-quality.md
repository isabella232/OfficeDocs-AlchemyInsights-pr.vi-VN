---
title: Chất lượng chia sẻ màn hình
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11061"
- "11062"
- "9002254"
- "9002536"
ms.openlocfilehash: 0832f886d3f5c0bfbfe138647403e4e215deaacb
ms.sourcegitcommit: d822377ec76adf9ef6d13bc761a16c9900a3e7cb
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/26/2021
ms.locfileid: "52125768"
---
# <a name="screen-sharing-quality"></a><span data-ttu-id="afa0e-102">Chất lượng chia sẻ màn hình</span><span class="sxs-lookup"><span data-stu-id="afa0e-102">Screen sharing quality</span></span>

<span data-ttu-id="afa0e-103">Trong hầu hết các trường hợp vấn đề về chất lượng với Chia sẻ Màn hình đi kèm đến băng thông hạn chế từ phía máy khách.</span><span class="sxs-lookup"><span data-stu-id="afa0e-103">In most cases quality issues with Screen Sharing comes down to limited bandwidth from the client side.</span></span>  <span data-ttu-id="afa0e-104">Khi băng thông không bị hạn chế, Teams sẽ tối ưu hóa chất lượng phương tiện, bao gồm độ phân giải video lên tới 1080p, lên tới 30fps cho video và 15fps cho nội dung và âm thanh có độ trung thực cao.</span><span class="sxs-lookup"><span data-stu-id="afa0e-104">Where bandwidth isn't limited, Teams optimizes media quality, including up to 1080p video resolution, up to 30fps for video and 15fps for content, and high-fidelity audio.</span></span>

<span data-ttu-id="afa0e-105">Teams nên luôn thận trọng khi sử dụng băng thông và có thể mang lại chất lượng video HD dưới 1,2Mbps.</span><span class="sxs-lookup"><span data-stu-id="afa0e-105">Teams is always conservative on bandwidth utilization and can deliver HD video quality in under 1.2Mbps.</span></span> <span data-ttu-id="afa0e-106">Mức tiêu thụ băng thông thực tế trong mỗi cuộc gọi âm thanh/video hoặc cuộc họp khác nhau dựa trên các yếu tố như bố trí video, độ phân giải video và khung video trên giây.</span><span class="sxs-lookup"><span data-stu-id="afa0e-106">The actual bandwidth consumption in each audio/video call or meeting vary based on factors such as video layout, video resolution, and video frames per second.</span></span> <span data-ttu-id="afa0e-107">Khi có nhiều băng thông hơn, chất lượng và mức sử dụng sẽ tăng để cung cấp trải nghiệm tốt nhất.</span><span class="sxs-lookup"><span data-stu-id="afa0e-107">When more bandwidth is available, quality and usage increase to deliver the best experience.</span></span> <span data-ttu-id="afa0e-108">Bảng này mô tả cách thức Teams băng thông:</span><span class="sxs-lookup"><span data-stu-id="afa0e-108">This table describes how Teams uses bandwidth:</span></span>

<span data-ttu-id="afa0e-109">**Kịch bản (lên/xuống) Băng thông**</span><span class="sxs-lookup"><span data-stu-id="afa0e-109">**Bandwidth(up/down) Scenarios**</span></span>

- <span data-ttu-id="afa0e-110">Cuộc gọi âm thanh ngang hàng 30 kbps</span><span class="sxs-lookup"><span data-stu-id="afa0e-110">30 kbps Peer-to-peer audio calling</span></span>

- <span data-ttu-id="afa0e-111">130 kbps Cuộc gọi thoại ngang hàng và chia sẻ màn hình</span><span class="sxs-lookup"><span data-stu-id="afa0e-111">130 kbps Peer-to-peer audio calling and screen sharing</span></span>

- <span data-ttu-id="afa0e-112">Cuộc gọi video chất lượng ngang hàng 360p 500 kbps tại 30fps</span><span class="sxs-lookup"><span data-stu-id="afa0e-112">500 kbps Peer-to-peer quality video calling 360p at 30fps</span></span>

- <span data-ttu-id="afa0e-113">Gọi video chất lượng HD ngang hàng 1,2 Mbps với độ phân giải HD 720p ở 30fps</span><span class="sxs-lookup"><span data-stu-id="afa0e-113">1.2 Mbps Peer-to-peer HD quality video calling with resolution of HD 720p at 30fps</span></span>

- <span data-ttu-id="afa0e-114">Gọi video chất lượng HD ngang hàng 1,5 Mbps với độ phân giải HD 1080p ở 30fps</span><span class="sxs-lookup"><span data-stu-id="afa0e-114">1.5 Mbps Peer-to-peer HD quality video calling with resolution of HD 1080p at 30fps</span></span>

- <span data-ttu-id="afa0e-115">Cuộc gọi video nhóm 500kbps/1Mbps</span><span class="sxs-lookup"><span data-stu-id="afa0e-115">500kbps/1Mbps Group Video calling</span></span>

- <span data-ttu-id="afa0e-116">Cuộc gọi video Nhóm HD 1Mbps/2Mbps (video 540p trên màn hình 1080p)</span><span class="sxs-lookup"><span data-stu-id="afa0e-116">1Mbps/2Mbps HD Group video calling (540p videos on 1080p screen)</span></span>

<span data-ttu-id="afa0e-117">Để biết thêm thông tin, [xem mục Chuẩn bị mạng cho tổ chức của bạn để Microsoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)</span><span class="sxs-lookup"><span data-stu-id="afa0e-117">For more information, see [Prepare your organization's network for Microsoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)</span></span>