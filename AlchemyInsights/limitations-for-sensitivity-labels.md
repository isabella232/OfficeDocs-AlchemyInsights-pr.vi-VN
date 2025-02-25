---
title: Giới hạn của nhãn nhạy cảm cho các tệp Office trong SharePoint và OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: 376c0293c325a725c117d54bb0f15b0146b9224c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332839"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Giới hạn của nhãn nhạy cảm cho các tệp Office trong SharePoint và OneDrive

Khi bật nhãn nhạy cảm cho Office tệp trong SharePoint và OneDrive, hãy lưu ý đến các yêu cầu và giới hạn, bao gồm:

- SharePoint và OneDrive thể xử lý một số tệp được đánh nhãn và mã hóa từ các ứng dụng Office trên máy tính khi tệp chứa dữ liệu PowerQuery, dữ liệu được lưu trữ bởi các bổ trợ tùy chỉnh hoặc phần XML tùy chỉnh.
- SharePoint và OneDrive không tự động áp dụng nhãn nhạy cảm cho các tệp hiện có mà bạn đã mã hóa bằng cách dùng nhãn Azure Information Protection (AIP). Để áp dụng nhãn nhạy cảm cho tệp được mã hóa: 
    - Đảm bảo rằng các nhãn AIP đã được di chuyển và phát hành đến Trung tâm Tuân Microsoft 365 Kế bên.
    - Tải xuống các tệp được gắn nhãn, rồi tải chúng lên vị trí SharePoint hoặc OneDrive gốc của chúng.
- Đối với tài liệu được mã hóa, chức năng in không được hỗ trợ.

Để biết thêm chi tiết về các giới hạn, hãy xem Bật nhãn nhạy cảm cho các Office trong [SharePoint và OneDrive.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations)
