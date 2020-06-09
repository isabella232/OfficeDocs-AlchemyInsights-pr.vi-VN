---
title: 'Lỗi: các quy tắc trên máy tính này không khớp'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/09/2020
ms.locfileid: "44618035"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="7ca96-102">Lỗi: các quy tắc trên máy tính này không khớp</span><span class="sxs-lookup"><span data-stu-id="7ca96-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="7ca96-103">Để xem trạng thái Cập Nhật của vấn đề này, [hãy xem các quy tắc trên máy tính này không phù hợp với các quy tắc trên Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="7ca96-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="7ca96-104">Nhóm Outlook đã thực hiện một khắc phục trong xây dựng 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="7ca96-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="7ca96-105">Việc khắc phục đã có tại Insider Fast và sẽ đi đến hàng tháng Channel vào cuối tháng sáu 2020.</span><span class="sxs-lookup"><span data-stu-id="7ca96-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="7ca96-106">Một khi bạn đã xây dựng cố định bạn có thể nhận được lời nhắc "những quy tắc nào bạn muốn giữ" một lần cuối cùng.</span><span class="sxs-lookup"><span data-stu-id="7ca96-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="7ca96-107">Chọn máy chủ khi được nhắc và sau đó quay trở lại trong Outlook và kích hoạt lại bất kỳ quy tắc đã bị vô hiệu hoá.</span><span class="sxs-lookup"><span data-stu-id="7ca96-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="7ca96-108">Cho đến khi sửa chữa có sẵn vui lòng sử dụng giải pháp sau:</span><span class="sxs-lookup"><span data-stu-id="7ca96-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="7ca96-109">Cách **giải quyết**: trong báo cáo gần đây, sự cố đã xảy ra đối với những người đã chỉ tạo ra các quy tắc khách hàng trong màn hình Outlook.</span><span class="sxs-lookup"><span data-stu-id="7ca96-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="7ca96-110">Nếu bạn tiếp tục chạy vào sự cố, hãy xem xét xoá các quy tắc và sau đó tạo và chỉnh sửa quy tắc chỉ trong OWA (Outlook Web App) cho đến khi vấn đề được giải quyết.</span><span class="sxs-lookup"><span data-stu-id="7ca96-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="7ca96-111">Nếu bạn không thể xoá các quy tắc theo cách thủ công, bạn có thể chạy lệnh Outlook khi bạn khởi động Outlook bằng Outlook. exe/cleanrules.</span><span class="sxs-lookup"><span data-stu-id="7ca96-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="7ca96-112">Điều này sẽ xóa cả quy tắc máy khách và máy chủ.</span><span class="sxs-lookup"><span data-stu-id="7ca96-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="7ca96-113">Nó sẽ xóa tất cả các quy tắc cho tất cả các tài khoản trong hồ sơ Outlook.</span><span class="sxs-lookup"><span data-stu-id="7ca96-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="7ca96-114">Lệnh này là thêm tài liệu trong bài viết chuyển dòng lệnh.</span><span class="sxs-lookup"><span data-stu-id="7ca96-114">This command is further documented in the Command-line switches  article.</span></span>