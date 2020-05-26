---
title: Giải quyết các đội đăng nhập lỗi AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/20/2020
ms.locfileid: "44358364"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="7aedb-102">Giải quyết các đội đăng nhập lỗi AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="7aedb-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="7aedb-103">Khi đăng nhập vào Microsoft teams, bạn có thể nhận được lỗi: **xin lỗi, nhưng chúng tôi đang gặp sự cố khi đăng nhập bạn trong AADSTS9000411: yêu cầu không được định dạng đúng. Tham số "login_hint" được sao chép.**</span><span class="sxs-lookup"><span data-stu-id="7aedb-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="7aedb-104">Để giải quyết vấn đề này, hãy đảm bảo các khách hàng Microsoft teams của bạn được Cập Nhật.</span><span class="sxs-lookup"><span data-stu-id="7aedb-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="7aedb-105">Để biết thêm thông tin về Cập Nhật ứng dụng khách của bạn, hãy xem [Update Microsoft teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="7aedb-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="7aedb-106">Nếu bạn không thể Cập Nhật khách hàng của bạn cho một số lý do, đăng xuất khỏi máy khách sẽ xóa hầu hết các dữ liệu lưu trữ.</span><span class="sxs-lookup"><span data-stu-id="7aedb-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="7aedb-107">Tuy nhiên, nếu bạn vẫn gặp sự cố sau khi đăng xuất, thoát khỏi teams và vui lòng xóa bộ nhớ cache của khách hàng bằng làm như sau:</span><span class="sxs-lookup"><span data-stu-id="7aedb-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="7aedb-108">Đóng Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="7aedb-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="7aedb-109">Truy cập:%AppData%\microsoft\teams và xóa tất cả các tệp.</span><span class="sxs-lookup"><span data-stu-id="7aedb-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="7aedb-110">Mở Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="7aedb-110">Reopen Microsoft Teams.</span></span>
