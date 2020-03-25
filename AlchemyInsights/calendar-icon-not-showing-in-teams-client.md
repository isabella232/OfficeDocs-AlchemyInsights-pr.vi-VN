---
title: Biểu tượng lịch không hiển thị trong khách hàng teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932379"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="5ef4e-102">Biểu tượng lịch không hiển thị trong khách hàng teams</span><span class="sxs-lookup"><span data-stu-id="5ef4e-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="5ef4e-103">Tab lịch trong teams yêu cầu quyền truy cập vào hộp thư Exchange qua dịch vụ Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="5ef4e-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="5ef4e-104">Hộp thư Exchange có thể trực tuyến hoặc tại chỗ.</span><span class="sxs-lookup"><span data-stu-id="5ef4e-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="5ef4e-105">Đối với người dùng trực tuyến không thấy tab lịch, đảm bảo rằng chúng [được cấp phép cho hộp thư Exchange Online và hộp thư được kích hoạt](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="5ef4e-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="5ef4e-106">Nếu người dùng có một hộp thư hợp lệ trong Exchange Online, nhưng vẫn không thể xem tab lịch, bạn có thể gặp sự cố mạng.</span><span class="sxs-lookup"><span data-stu-id="5ef4e-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="5ef4e-107">Sử dụng [phân tích kết nối từ xa của Microsoft](https://testconnectivity.microsoft.com/) và chạy **kiểm tra kết nối dịch vụ web của Microsoft Exchange** cho người dùng bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="5ef4e-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="5ef4e-108">Cuối cùng kiểm tra các [ứng dụng teams-chính sách thiết lập ứng dụng](https://admin.teams.microsoft.com/policies/app-setup) để đảm bảo ứng dụng lịch không bị xóa khỏi chính sách được áp dụng cho người dùng (nhiều khả năng là **toàn cầu (mặc định**trong toàn bộ).</span><span class="sxs-lookup"><span data-stu-id="5ef4e-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="5ef4e-109">Nếu người dùng của bạn homed tại chỗ, bạn cần xác nhận cấu hình kết hợp của bạn là ổn định.</span><span class="sxs-lookup"><span data-stu-id="5ef4e-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="5ef4e-110">Sử dụng [thuật sĩ cấu hình kết](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) hợp để khắc phục sự cố.</span><span class="sxs-lookup"><span data-stu-id="5ef4e-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="5ef4e-111">Lưu ý rằng các [nhóm yêu cầu Exchange 2016 CU3 trở](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)lên.</span><span class="sxs-lookup"><span data-stu-id="5ef4e-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
