---
title: Thiết đặt nhãn Outlook định không được áp dụng
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/17/2021
ms.locfileid: "58455081"
---
# <a name="default-outlook-label-setting-not-applied"></a>Thiết đặt nhãn Outlook định không được áp dụng

Nếu thiết đặt nhãn mặc định của Outlook của bạn không áp dụng đúng cách và một nhãn khác hoặc không có nhãn nào được áp dụng, bạn có thể đang gặp phải một vấn đề đã biết (MC277818) và nên thực hiện một trong hai tùy chọn sau để giải quyết vấn đề này:

**Tùy chọn 1:**

1. Đi đến Trung Microsoft 365 Tuân thủ để > **Bảo vệ Thông tin** Giải  >  **pháp**.
1. Chọn **Chính sách nhãn**, rồi chọn chính sách nhãn bạn cần chỉnh sửa ( Cài đặt **OutlookDefaultlabel** không được đặt đúng cách trên chính sách nhãn mình cần sửa. Chạy **Tải nhãn chính sách để** xem cài đặt này), rồi chọn Chỉnh sửa chính **sách**.
1. Chọn **Tiếp** cho đến khi bạn nhìn thấy thiết đặt Áp dụng nhãn mặc định này cho **email,** có sẵn nếu bạn chọn Yêu cầu người dùng áp dụng nhãn cho **email** và tài liệu thừa tự trong hộp thoại Thiết đặt **chính** sách.
1. Trong hộp **thoại Áp dụng nhãn mặc định cho tài** liệu, chọn Không **có** từ danh sách thả xuống.
1. Chọn **Tiếp theo** và **Gửi** để lưu thiết đặt nhãn của bạn.

**Tùy chọn 2:**

Trong Trung tâm Bảo mật và Tuân thủ [Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps), hãy sử dụng commandlet Set-LabelPolicy để thay đổi **OutlookDefaultlabel** thành **None** trên {OutlookDefaultLabel="None"}.

Chạy: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Để biết thêm thông tin về các nhãn mặc định cho Outlook, hãy [xem Đặt một nhãn mặc định khác cho Outlook.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)