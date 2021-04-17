---
title: Biểu tượng lịch không hiển thị trong máy khách nhóm
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819975"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="345c2-102">Biểu tượng lịch không hiển thị trong máy khách nhóm</span><span class="sxs-lookup"><span data-stu-id="345c2-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="345c2-103">Tab lịch trong nhóm yêu cầu quyền truy nhập vào hộp thư Exchange thông qua dịch vụ Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="345c2-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="345c2-104">Hộp thư Exchange có thể trực tuyến hoặc tại cơ sở.</span><span class="sxs-lookup"><span data-stu-id="345c2-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="345c2-105">Đối với những người dùng trực tuyến không nhìn thấy tab lịch, hãy đảm bảo rằng chúng [được cấp phép cho hộp thư Exchange Online và hộp thư được bật](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="345c2-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="345c2-106">Nếu người dùng có một hộp thư hợp lệ trong Exchange Online, nhưng vẫn không nhìn thấy tab lịch, bạn có thể gặp phải sự cố mạng.</span><span class="sxs-lookup"><span data-stu-id="345c2-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="345c2-107">Sử dụng trình phân [tích kết nối từ xa của Microsoft](https://testconnectivity.microsoft.com/) và chạy các **kiểm tra kết nối dịch vụ web của Microsoft Exchange** cho người dùng bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="345c2-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="345c2-108">Cuối cùng, hãy kiểm tra các [ứng dụng nhóm – chính sách thiết lập ứng dụng](https://admin.teams.microsoft.com/policies/app-setup) để đảm bảo rằng ứng dụng lịch chưa được loại bỏ khỏi chính sách được áp dụng cho người dùng (có thể là **mặc định toàn cầu (toàn** bộ tổ chức).</span><span class="sxs-lookup"><span data-stu-id="345c2-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="345c2-109">Nếu người dùng của bạn được sắp đặt tại cơ sở, bạn cần phải xác nhận cấu hình hỗn hợp của bạn được khỏe mạnh.</span><span class="sxs-lookup"><span data-stu-id="345c2-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="345c2-110">Sử dụng trình [hướng dẫn cấu hình hỗn](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) hợp để khắc phục sự cố.</span><span class="sxs-lookup"><span data-stu-id="345c2-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="345c2-111">Lưu ý rằng các [nhóm yêu cầu Exchange 2016 CU3 hoặc cao hơn](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="345c2-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
