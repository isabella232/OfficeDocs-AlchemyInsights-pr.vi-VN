---
title: 'Lỗi: các quy tắc trên máy tính này không khớp'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690985"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="1e607-102">Lỗi: các quy tắc trên máy tính này không khớp</span><span class="sxs-lookup"><span data-stu-id="1e607-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="1e607-103">Để xem trạng thái Cập Nhật của vấn đề đã biết này, hãy xem [các quy tắc trên máy tính này không khớp với quy tắc trên Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="1e607-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="1e607-104">Nhóm Outlook đã triển khai bản sửa lỗi trong bản dựng 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="1e607-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="1e607-105">Bản sửa lỗi đã có sẵn trong người dùng nội bộ nhanh và sẽ đi tới kênh hàng tháng vào cuối tháng 6 năm 2020.</span><span class="sxs-lookup"><span data-stu-id="1e607-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="1e607-106">Sau khi bạn có bản dựng đã khắc phục, bạn có thể nhận được lời nhắc "những quy tắc nào bạn muốn giữ lại" lần cuối cùng.</span><span class="sxs-lookup"><span data-stu-id="1e607-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="1e607-107">Chọn máy chủ khi được nhắc và sau đó quay lại trong Outlook và kích hoạt lại bất kỳ quy tắc nào đã bị vô hiệu hóa.</span><span class="sxs-lookup"><span data-stu-id="1e607-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="1e607-108">Cho đến khi sửa lỗi sẵn dùng, vui lòng sử dụng giải pháp thay thế sau đây:</span><span class="sxs-lookup"><span data-stu-id="1e607-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="1e607-109">Giải pháp thay **thế: trong**báo cáo gần đây, sự cố đã xảy ra đối với những người chỉ có các quy tắc máy khách tạo trong Outlook trên máy tính.</span><span class="sxs-lookup"><span data-stu-id="1e607-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="1e607-110">Nếu bạn tiếp tục gặp vấn đề, hãy cân nhắc việc xóa bỏ quy tắc, rồi tạo và chỉnh sửa quy tắc chỉ trong OWA (Outlook Web App) cho đến khi sự cố này được giải quyết.</span><span class="sxs-lookup"><span data-stu-id="1e607-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="1e607-111">Nếu bạn không thể xóa bỏ quy tắc theo cách thủ công, bạn có thể chạy lệnh Outlook khi bạn khởi động Outlook bằng cách chạy Outlook.exe/cleanrules.</span><span class="sxs-lookup"><span data-stu-id="1e607-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="1e607-112">Việc này sẽ xóa cả quy tắc máy khách và máy chủ.</span><span class="sxs-lookup"><span data-stu-id="1e607-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="1e607-113">Nó sẽ xóa tất cả các quy tắc cho tất cả các tài khoản trong hồ sơ Outlook.</span><span class="sxs-lookup"><span data-stu-id="1e607-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="1e607-114">Lệnh này được thêm vào tài liệu trong bài viết chuyển dòng lệnh.</span><span class="sxs-lookup"><span data-stu-id="1e607-114">This command is further documented in the Command-line switches article.</span></span>

