---
title: Hỗ trợ của Microsoft Edge cho bảo vệ ứng dụng Microsoft Defender
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584177"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Hỗ trợ của Microsoft Edge cho bảo vệ ứng dụng Microsoft Defender

Được thiết kế dành cho Windows 10 và Microsoft Edge, ứng dụng guard dùng phương pháp phân cách phần cứng cho phép người dùng dẫn hướng một site không đáng tin cậy từ bên trong bộ chứa siêu bị cô lập, Hyper-V – đã được phân tách khỏi hệ điều hành máy chủ lưu trữ.

Người quản trị doanh nghiệp xác định danh sách các website đáng tin cậy, tài nguyên điện toán đám mây và các mạng nội bộ. Khi người dùng truy nhập vào một site không có trong danh sách, Microsoft Edge sẽ mở site đó trong bộ chứa. Điều này có nghĩa là nếu site đó trở thành độc hại, máy tính lưu trữ sẽ vẫn được bảo vệ và kẻ tấn công sẽ không nhận được dữ liệu doanh nghiệp.

Việc cài đặt các phần mở rộng trong bộ chứa được hỗ trợ dưới dạng Microsoft Edge Phiên bản 81 và có thể điều khiển thông qua chính sách. Địa chỉ updateURL được dùng trong chính sách ExtensionInstallForcelist sẽ được thêm vào như một nguồn tài nguyên trung lập trong các chính sách phân cách mạng được sử dụng bởi bộ bảo vệ ứng dụng.

Để biết thêm thông tin, hãy xem [hỗ trợ Microsoft Edge cho bộ bảo vệ ứng dụng bảo vệ Microsoft](https://go.microsoft.com/fwlink/?linkid=2134229).
