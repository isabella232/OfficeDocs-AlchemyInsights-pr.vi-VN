---
title: Truy cập Dịch vụ nghỉ hưu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: cb8123583b68e945ef878fdbaf211fd1d8205bb3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050511"
---
# <a name="access-services-retirement"></a>Truy cập Dịch vụ nghỉ hưu

Như chúng tôi ban đầu được công bố trong MC97576, vào tháng ba 2017, và tiếp tục giao tiếp trong năm qua truy cập Dịch vụ đang được nghỉ hưu từ văn phòng 365. Giai đoạn tiếp theo trong quá trình này sẽ là loại bỏ truy cập web cơ sở dữ liệu sử dụng danh sách SharePoint như lưu trữ dữ liệu cơ bản của họ.

**Điều này ảnh hưởng đến tôi như thế nào?**

Bắt đầu từ ngày 2019 tháng 6, chúng tôi sẽ ngừng tạo cơ sở dữ liệu Access mới trong SharePoint Online và tắt dịch vụ và bất kỳ ứng dụng còn lại nào vào tháng 2020.

**Tôi cần làm gì để chuẩn bị cho sự thay đổi này?**

Chúng tôi khuyến khích bạn tạo một kế hoạch chuyển tiếp cho cơ sở dữ liệu Web Access của tổ chức bạn. Quản trị viên có thể sử dụng [máy quét ứng dụng SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) để lấy hàng tồn kho của các ứng dụng truy cập mà các trang web đang sử dụng.

Có một số cách để di chuyển dữ liệu truy cập cơ sở dữ liệu web:

- Nhập vào cơ sở dữ liệu Access cục bộ (. ACCDB) hoặc tệp Excel.
- Chúng tôi cũng khuyên bạn nên khám phá Microsoft PowerApps như một nền tảng thay thế để tạo các giải pháp kinh doanh không có mã cho các thiết bị web và di động.