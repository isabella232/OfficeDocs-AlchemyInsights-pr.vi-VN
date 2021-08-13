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
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813171"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Giới hạn của nhãn nhạy cảm cho các tệp Office trong SharePoint và OneDrive

Khi bật nhãn nhạy cảm cho Office tệp trong SharePoint và OneDrive, hãy lưu ý đến các yêu cầu và giới hạn, bao gồm:

- SharePoint và OneDrive thể xử lý một số tệp được đánh nhãn và mã hóa từ các ứng dụng Office trên máy tính khi tệp chứa dữ liệu PowerQuery, dữ liệu được lưu trữ bởi các bổ trợ tùy chỉnh hoặc phần XML tùy chỉnh.
- SharePoint và OneDrive tự động áp dụng nhãn nhạy cảm với các tệp hiện có mà bạn đã mã hóa bằng cách dùng nhãn Azure Information Protection (AIP). Để áp dụng nhãn nhạy cảm cho các tệp được mã hóa: 
    - Đảm bảo rằng các nhãn AIP đã được di chuyển và phát hành đến Trung Microsoft 365 Thủ tục.
    - Tải xuống các tệp được gắn nhãn, rồi tải lên tệp gốc của SharePoint hoặc OneDrive trí khác.
- Đối với tài liệu được mã hóa, chức năng in không được hỗ trợ.

Để biết thêm chi tiết về các giới hạn, hãy xem Bật nhãn nhạy cảm cho các Office trong SharePoint [và OneDrive.](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations)
