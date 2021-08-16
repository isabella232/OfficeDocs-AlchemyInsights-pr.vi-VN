---
title: Thực hiện kiểm tra tính tương thích của ứng dụng
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9138"
- "9005291"
ms.openlocfilehash: 40c16324270e26a882b16e5c2e0a6cf248d34ed84e95e845aac5dfa44ac58c72
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004859"
---
# <a name="do-app-compatibility-testing"></a>Thực hiện kiểm tra tính tương thích của ứng dụng

Tính tương thích của ứng Microsoft Edge rất cao. Trên thực tế, rất cao đến mức Microsoft cung cấp những lời hứa về tính tương thích sau:
- Nếu phiên bản này hoạt động Microsoft Edge 45 trở lên, công cụ này sẽ hoạt động trên Microsoft Edge 77 trở lên.
- Nếu trình duyệt này hoạt động trên Internet Explorer, trình duyệt sẽ hoạt động Microsoft Edge chế độ Internet Explorer.
- Nếu nó hoạt động trên Google Chrome, nó sẽ hoạt động trên Microsoft Edge.

Nếu bạn có ứng dụng mà chúng tôi không đáp ứng lời hứa này thì chúng tôi sẽ nộp đơn cam kết khắc phục sự cố với [Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure).

Bất chấp lời hứa này, chúng tôi biết rằng nhiều tổ chức phải xác thực một số ứng dụng vì lý do tuân thủ hoặc quản lý rủi ro. Mặc dù chúng tôi mong đợi điều này sẽ rất đơn giản, nhưng điều quan trọng là phải có tổ chức và nghiêm ngặt trong việc thử nghiệm ứng dụng.

Có hai cách để thực hiện kiểm tra tính tương thích ứng dụng:

- **Kiểm tra phòng thí** nghiệm : Các ứng dụng được kiểm tra trong môi trường được kiểm soát chặt chẽ với các cấu hình cụ thể.
- **Thử nghiệm thí điểm**: Số lượng người dùng được kiểm tra ứng dụng trong môi trường làm việc hàng ngày có giới hạn bằng cách sử dụng thiết bị của riêng họ.

Chọn phương pháp phù hợp nhất cho từng ứng dụng và thực hiện thử nghiệm trước khi cho ra mắt toàn bộ tổ chức.

Sau khi đảm bảo rằng các ứng dụng của bạn tương thích, bạn đã sẵn sàng triển khai các Microsoft Edge vào nhóm thí điểm.
