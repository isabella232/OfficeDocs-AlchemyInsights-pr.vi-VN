---
title: Không thể đăng nhập vào các nhóm do lỗi autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 649124db135805d8101b43dbead63860d36853ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799982"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="57558-102">Không thể đăng nhập vào các nhóm do lỗi tự động đăng nhập. microsoftazuread-SSO dot com: 443</span><span class="sxs-lookup"><span data-stu-id="57558-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="57558-103">Nếu SSO seamless được bật là xác thực O365, URL "autologon.microsoftazuread-sso.com" có thể cần phải được thêm vào site intranet.</span><span class="sxs-lookup"><span data-stu-id="57558-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="57558-104">Nếu trước đó đã được thêm vào các site tin cậy và SSO được dàn lại đang được sử dụng, nó sẽ được loại bỏ khỏi các trang tin cậy.</span><span class="sxs-lookup"><span data-stu-id="57558-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="57558-105">Vui lòng xem xét [danh sách khắc phục sự cố SSO liền mạch](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="57558-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="57558-106">Làm theo các bước sau để thêm URL vào danh sách site intranet:</span><span class="sxs-lookup"><span data-stu-id="57558-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="57558-107">Mở Internet Explorer bằng cách bấm vào nút **bắt đầu** .</span><span class="sxs-lookup"><span data-stu-id="57558-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="57558-108">Trong hộp tìm kiếm, nhập Internet Explorer, sau đó trong danh sách kết quả, hãy bấm **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="57558-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="57558-109">Bấm vào **công cụ**, rồi bấm **tùy chọn Internet**.</span><span class="sxs-lookup"><span data-stu-id="57558-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="57558-110">Bấm vào tab **bảo mật** .</span><span class="sxs-lookup"><span data-stu-id="57558-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="57558-111">Bây giờ, hãy bấm vào **site intranet Cục bộ** , rồi bấm vào nút **site** rồi **nâng cao** .</span><span class="sxs-lookup"><span data-stu-id="57558-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="57558-112">Nhập URL của trang web, rồi bấm vào **Thêm**.</span><span class="sxs-lookup"><span data-stu-id="57558-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="57558-113">Khi bạn đã hoàn tất, hãy bấm **đóng**.</span><span class="sxs-lookup"><span data-stu-id="57558-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="57558-114">Để biết thêm thông tin, hãy xem [tài liệu về việc triển khai SSO trong suốt cho O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (bao gồm quy trình dựa trên chính sách để thêm URL vào site intranet trong bước 3).</span><span class="sxs-lookup"><span data-stu-id="57558-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
