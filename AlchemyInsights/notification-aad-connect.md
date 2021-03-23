---
title: Thông báo kết nối với Bad
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037231"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="7a546-102">Thông báo kết nối với Bad</span><span class="sxs-lookup"><span data-stu-id="7a546-102">Notification AAD Connect</span></span>

- <span data-ttu-id="7a546-103">Đảm bảo rằng bạn được phép thực hiện thao tác này.</span><span class="sxs-lookup"><span data-stu-id="7a546-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="7a546-104">Người quản trị toàn cầu có quyền truy nhập theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="7a546-104">Global Admins have access by default.</span></span> <span data-ttu-id="7a546-105">Ngoài ra, bạn có thể sử dụng [điều khiển truy nhập dựa trên vai trò](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) để cho phép người đóng góp đăng ký.</span><span class="sxs-lookup"><span data-stu-id="7a546-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="7a546-106">Đảm bảo các điểm cuối bắt buộc được kích hoạt và không bị chặn do tường lửa.</span><span class="sxs-lookup"><span data-stu-id="7a546-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="7a546-107">Để biết chi tiết, hãy xem mục [yêu cầu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="7a546-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="7a546-108">Đăng ký có thể không thành công vì giao tiếp đi là phải chịu việc kiểm tra SSL bằng tầng mạng.</span><span class="sxs-lookup"><span data-stu-id="7a546-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="7a546-109">Đảm bảo rằng bạn đã xác minh cài đặt thông báo cho Azure AD Connect Health và xem lại thiết đặt của bạn.</span><span class="sxs-lookup"><span data-stu-id="7a546-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="7a546-110">Để tìm hiểu cách đặt cấu hình các thiết đặt thông báo cho các thông báo trạng thái kết nối Azure AD, hãy xem [hướng dẫn](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)này.</span><span class="sxs-lookup"><span data-stu-id="7a546-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="7a546-111">Để tìm hiểu thêm về báo cáo đồng bộ hóa trạng thái kết nối và cách tải xuống, hãy xem [báo cáo đồng bộ hóa mức đối tượng](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="7a546-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="7a546-112">Để khắc phục sự cố về cảnh báo tình trạng thông tin kết nối, hãy làm theo [hướng dẫn khắc phục sự cố cho các](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) câu hỏi thường gặp về dữ liệu tự động kết nối, hãy xem các [câu hỏi thường gặp về cài đặt](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="7a546-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
