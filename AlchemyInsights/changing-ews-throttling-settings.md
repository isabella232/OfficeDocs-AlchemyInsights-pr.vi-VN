---
title: Thay đổi thiết đặt điều chỉnh EWS
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
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968399"
---
# <a name="changing-ews-throttling-settings"></a>Thay đổi thiết đặt điều chỉnh EWS

Vui lòng chạy kiểm tra tự động của chúng tôi, điều này sẽ cho phép bạn sửa đổi chính sách điều chỉnh EWS trong thời gian di chuyển. Lưu ý rằng ngay cả sau khi chạy chức năng này, hoạt động nhập EWS vẫn sẽ bị giới hạn ở 150mb/5 phút cho mỗi hộp thư; để đạt được tốc độ lưu lượng di chuyển cao hơn, vui lòng di chuyển nhiều người dùng hơn đồng thời.

Xin lưu ý rằng các thay đổi về chính sách điều chỉnh EWS không ảnh hưởng đến các loại di chuyển sau đây (sử dụng công cụ của Microsoft): Kết hợp, Chuyển giao/Theo giai đoạn (RPC/HTTP), IMAP, G Suite, Thư mục Công cộng hoặc Dịch vụ Nhập PST.