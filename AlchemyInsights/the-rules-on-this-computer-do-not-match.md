---
title: 'Lỗi: các quy tắc trên máy tính này không khớp'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782974"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="56c2f-102">Lỗi: các quy tắc trên máy tính này không khớp</span><span class="sxs-lookup"><span data-stu-id="56c2f-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="56c2f-103">Để xem trạng thái Cập Nhật của vấn đề đã biết này, hãy xem [các quy tắc trên máy tính này không khớp với quy tắc trên Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="56c2f-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="56c2f-104">Nhóm Outlook đã triển khai bản sửa lỗi trong bản dựng 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="56c2f-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="56c2f-105">Bản sửa lỗi đã có sẵn trong người dùng nội bộ nhanh và sẽ đi tới kênh hàng tháng vào cuối tháng 6 năm 2020.</span><span class="sxs-lookup"><span data-stu-id="56c2f-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="56c2f-106">Sau khi bạn có bản dựng đã khắc phục, bạn có thể nhận được lời nhắc "những quy tắc nào bạn muốn giữ lại" lần cuối cùng.</span><span class="sxs-lookup"><span data-stu-id="56c2f-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="56c2f-107">Chọn máy chủ khi được nhắc và sau đó quay lại trong Outlook và kích hoạt lại bất kỳ quy tắc nào đã bị vô hiệu hóa.</span><span class="sxs-lookup"><span data-stu-id="56c2f-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="56c2f-108">Cho đến khi sửa lỗi sẵn dùng, vui lòng sử dụng giải pháp thay thế sau đây:</span><span class="sxs-lookup"><span data-stu-id="56c2f-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="56c2f-109">Giải pháp thay **thế: trong** báo cáo gần đây, sự cố đã xảy ra đối với những người chỉ có các quy tắc máy khách tạo trong Outlook trên máy tính.</span><span class="sxs-lookup"><span data-stu-id="56c2f-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="56c2f-110">Nếu bạn tiếp tục gặp vấn đề, hãy cân nhắc việc xóa bỏ quy tắc, rồi tạo và chỉnh sửa quy tắc chỉ trong OWA (Outlook Web App) cho đến khi sự cố này được giải quyết.</span><span class="sxs-lookup"><span data-stu-id="56c2f-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="56c2f-111">Nếu bạn không thể xóa bỏ quy tắc theo cách thủ công, bạn có thể chạy lệnh Outlook khi bạn khởi động Outlook bằng cách chạy Outlook.exe/cleanrules.</span><span class="sxs-lookup"><span data-stu-id="56c2f-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="56c2f-112">Việc này sẽ xóa cả quy tắc máy khách và máy chủ.</span><span class="sxs-lookup"><span data-stu-id="56c2f-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="56c2f-113">Nó sẽ xóa tất cả các quy tắc cho tất cả các tài khoản trong hồ sơ Outlook.</span><span class="sxs-lookup"><span data-stu-id="56c2f-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="56c2f-114">Lệnh này được thêm vào tài liệu trong bài viết chuyển dòng lệnh.</span><span class="sxs-lookup"><span data-stu-id="56c2f-114">This command is further documented in the Command-line switches article.</span></span>

