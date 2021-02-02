---
title: Thay đổi thiết đặt điều chỉnh
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075919"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="ca9a3-102">Thay đổi thiết đặt điều chỉnh</span><span class="sxs-lookup"><span data-stu-id="ca9a3-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="ca9a3-103">Vui lòng chạy thử nghiệm tự động cho phép bạn sửa đổi chính sách kiểm tra EWS trong khoảng thời gian di chuyển của bạn.</span><span class="sxs-lookup"><span data-stu-id="ca9a3-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="ca9a3-104">Lưu ý rằng ngay cả sau khi thực hiện điều này, các phép nhập từ EWS sẽ vẫn được giới hạn trong 150mb mỗi 5 phút mỗi hộp thư; để đạt được tốc độ chuyển tiếp thông lượng di chuyển cao hơn, vui lòng di chuyển thêm người dùng đồng thời.</span><span class="sxs-lookup"><span data-stu-id="ca9a3-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="ca9a3-105">Vui lòng lưu ý rằng những thay đổi chính sách đối với các kiểu di chuyển sau đây không có hiệu lực trong các kiểu di chuyển sau (sử dụng công cụ Microsoft): kết hợp, chuyển giao/theo giai đoạn (RPC/HTTP), IMAP, G Suite, thư mục công cộng hoặc dịch vụ nhập PST.</span><span class="sxs-lookup"><span data-stu-id="ca9a3-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>