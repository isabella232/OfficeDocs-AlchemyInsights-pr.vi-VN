---
title: Giải quyết lỗi đăng nhập nhóm AADSTS9000411
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
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822009"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="87e5b-102">Giải quyết lỗi đăng nhập nhóm AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="87e5b-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="87e5b-103">Khi đăng nhập vào Microsoft nhóm, bạn có thể nhận được lỗi: **xin lỗi, nhưng chúng tôi đang gặp sự cố với việc đăng nhập vào AADSTS9000411: yêu cầu đó không được định dạng đúng. Tham số "login_hint" bị trùng lặp.**</span><span class="sxs-lookup"><span data-stu-id="87e5b-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="87e5b-104">Để giải quyết sự cố này, vui lòng đảm bảo rằng khách hàng Microsoft nhóm của bạn được Cập Nhật.</span><span class="sxs-lookup"><span data-stu-id="87e5b-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="87e5b-105">Để biết thêm thông tin về việc Cập Nhật máy khách của bạn, hãy xem [Cập nhật các nhóm Microsoft](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="87e5b-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="87e5b-106">Nếu bạn không thể cập nhật máy khách của mình vì lý do nào đó, hãy đăng xuất khỏi máy khách sẽ xóa hầu hết các dữ liệu được lưu trong bộ đệm ẩn.</span><span class="sxs-lookup"><span data-stu-id="87e5b-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="87e5b-107">Tuy nhiên, nếu bạn vẫn gặp sự cố sau khi đăng xuất/đăng nhập, hãy thoát khỏi nhóm và vui lòng xóa bộ đệm ẩn máy khách của bạn bằng cách thực hiện như sau:</span><span class="sxs-lookup"><span data-stu-id="87e5b-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="87e5b-108">Đóng nhóm Microsoft.</span><span class="sxs-lookup"><span data-stu-id="87e5b-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="87e5b-109">Đi đến:%AppData%\microsoft\nhóm và xóa tất cả các tệp.</span><span class="sxs-lookup"><span data-stu-id="87e5b-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="87e5b-110">Mở lại nhóm Microsoft.</span><span class="sxs-lookup"><span data-stu-id="87e5b-110">Reopen Microsoft Teams.</span></span>
