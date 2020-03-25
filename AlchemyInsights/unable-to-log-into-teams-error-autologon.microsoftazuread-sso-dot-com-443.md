---
title: Không thể đăng nhập vào teams do lỗi autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932283"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="7d4b5-102">Không thể đăng nhập vào nhóm do lỗi tự động đăng nhập. microsoftazuread-SSO dot com: 443</span><span class="sxs-lookup"><span data-stu-id="7d4b5-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="7d4b5-103">Nếu liền mạch SSO được kích hoạt như xác thực O365, URL "autologon.microsoftazuread-sso.com" có thể cần phải được thêm vào trang web intranet.</span><span class="sxs-lookup"><span data-stu-id="7d4b5-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="7d4b5-104">Nếu nó đã được thêm vào site tin cậy và liền mạch SSO đang được sử dụng, nó sẽ bị xoá khỏi site tin cậy.</span><span class="sxs-lookup"><span data-stu-id="7d4b5-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="7d4b5-105">Vui lòng đánh giá [danh sách kiểm tra khắc phục sự cố SSO liền mạch](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="7d4b5-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="7d4b5-106">Hãy làm theo các bước sau để thêm URL vào danh sách site intranet:</span><span class="sxs-lookup"><span data-stu-id="7d4b5-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="7d4b5-107">Mở Internet Explorer bằng cách bấm vào nút **bắt đầu** .</span><span class="sxs-lookup"><span data-stu-id="7d4b5-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="7d4b5-108">Trong hộp tìm kiếm, nhập Internet Explorer, sau đó, trong danh sách kết quả, bấm **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="7d4b5-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="7d4b5-109">Bấm **công cụ**, và sau đó bấm **tùy chọn Internet**.</span><span class="sxs-lookup"><span data-stu-id="7d4b5-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="7d4b5-110">Nhấp vào tab **bảo mật** .</span><span class="sxs-lookup"><span data-stu-id="7d4b5-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="7d4b5-111">Bây giờ bấm vào các **trang web Intranet Nội bộ** và sau đó bấm vào nút các **trang web** và sau đó **nâng cao** nút.</span><span class="sxs-lookup"><span data-stu-id="7d4b5-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="7d4b5-112">Nhập URL trang web và nhấp vào **Thêm**.</span><span class="sxs-lookup"><span data-stu-id="7d4b5-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="7d4b5-113">Khi bạn hoàn tất, bấm **đóng**.</span><span class="sxs-lookup"><span data-stu-id="7d4b5-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="7d4b5-114">Để biết thêm thông tin, xem [tài liệu để triển khai liền mạch SSO cho O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (bao gồm quy trình dựa trên chính sách để thêm URL vào trang web intranet trong bước 3).</span><span class="sxs-lookup"><span data-stu-id="7d4b5-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
