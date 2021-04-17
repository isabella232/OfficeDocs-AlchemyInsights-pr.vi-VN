---
title: Thay đổi thiết đặt điều chỉnh
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
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818058"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="c1265-102">Thay đổi thiết đặt điều chỉnh</span><span class="sxs-lookup"><span data-stu-id="c1265-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="c1265-103">Vui lòng chạy thử nghiệm tự động cho phép bạn sửa đổi chính sách kiểm tra EWS trong khoảng thời gian di chuyển của bạn.</span><span class="sxs-lookup"><span data-stu-id="c1265-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="c1265-104">Lưu ý rằng ngay cả sau khi thực hiện điều này, các phép nhập từ EWS sẽ vẫn được giới hạn trong 150mb mỗi 5 phút mỗi hộp thư; để đạt được tốc độ chuyển tiếp thông lượng di chuyển cao hơn, vui lòng di chuyển thêm người dùng đồng thời.</span><span class="sxs-lookup"><span data-stu-id="c1265-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="c1265-105">Vui lòng lưu ý rằng những thay đổi chính sách đối với các kiểu di chuyển sau đây không có hiệu lực trong các kiểu di chuyển sau (sử dụng công cụ Microsoft): kết hợp, chuyển giao/theo giai đoạn (RPC/HTTP), IMAP, G Suite, thư mục công cộng hoặc dịch vụ nhập PST.</span><span class="sxs-lookup"><span data-stu-id="c1265-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>