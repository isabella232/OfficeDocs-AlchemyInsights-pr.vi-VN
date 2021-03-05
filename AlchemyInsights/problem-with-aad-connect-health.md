---
title: Vấn đề với thiết bị cảm ứng của Bad Connect
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483125"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="acc85-102">Vấn đề với thiết bị cảm ứng của Bad Connect</span><span class="sxs-lookup"><span data-stu-id="acc85-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="acc85-103">Đảm bảo rằng bạn được phép thực hiện thao tác này.</span><span class="sxs-lookup"><span data-stu-id="acc85-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="acc85-104">Người quản trị toàn cầu có quyền truy nhập theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="acc85-104">Global Admins have access by default.</span></span> <span data-ttu-id="acc85-105">Ngoài ra, bạn có thể sử dụng [điều khiển truy nhập dựa trên vai trò](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) để cho phép người đóng góp đăng ký.</span><span class="sxs-lookup"><span data-stu-id="acc85-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="acc85-106">Đảm bảo các điểm cuối bắt buộc được kích hoạt và không bị chặn do tường lửa.</span><span class="sxs-lookup"><span data-stu-id="acc85-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="acc85-107">Để biết chi tiết, hãy xem mục [yêu cầu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="acc85-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="acc85-108">Đăng ký có thể không thành công vì giao tiếp đi là phải chịu việc kiểm tra SSL bằng tầng mạng.</span><span class="sxs-lookup"><span data-stu-id="acc85-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="acc85-109">Đảm bảo rằng bạn đã xác minh cài đặt thông báo cho Azure AD Connect Health.</span><span class="sxs-lookup"><span data-stu-id="acc85-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="acc85-110">Vui lòng xem lại thiết đặt của bạn.</span><span class="sxs-lookup"><span data-stu-id="acc85-110">Please review your setting.</span></span> <span data-ttu-id="acc85-111">[Hướng dẫn](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) này có thể giúp bạn hiểu cách cấu hình các thiết đặt thông báo cho Azure AD Connect Health Notifications.</span><span class="sxs-lookup"><span data-stu-id="acc85-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="acc85-112">Để tìm hiểu thêm về báo cáo đồng bộ hóa trạng thái kết nối và cách tải xuống, hãy xem [báo cáo đồng bộ hóa mức đối tượng](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="acc85-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="acc85-113">Để khắc phục sự cố về cảnh báo trạng thái kết nối, hãy làm theo [các hướng dẫn khắc phục sự cố cho các cảnh báo tự động kết nối dữ liệu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) và cho các câu hỏi thường gặp, hãy xem các [câu hỏi cài đặt kết nối thông thường](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)của cộng đồng.</span><span class="sxs-lookup"><span data-stu-id="acc85-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
