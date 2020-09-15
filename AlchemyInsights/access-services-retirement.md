---
title: Hưu trí dịch vụ Access
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698704"
---
# <a name="access-services-retirement"></a>Hưu trí dịch vụ Access

Như chúng tôi ban đầu được công bố trong MC97576, trong tháng ba 2017 và vẫn tiếp tục liên lạc trong các dịch vụ truy nhập năm trước đang được ngừng hoạt động. Giai đoạn tiếp theo trong quá trình này sẽ là loại bỏ cơ sở dữ liệu Web Access sử dụng danh sách SharePoint khi lưu trữ dữ liệu cơ bản của họ.

**Điều này ảnh hưởng đến tôi như thế nào?**

Bắt đầu 2019 tháng sáu, chúng tôi sẽ ngừng tạo cơ sở dữ liệu Access mới trong SharePoint Online và tắt dịch vụ và mọi ứng dụng còn lại của tháng tư 2020.

**Tôi cần làm gì để chuẩn bị cho thay đổi này?**

Chúng tôi khuyên bạn nên tạo một kế hoạch chuyển tiếp cho cơ sở dữ liệu Web Access của tổ chức bạn. Người quản trị có thể sử dụng máy [quét ứng dụng Access của SharePoint](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) để có được hàng tồn kho trong các ứng dụng Access mà các site đang sử dụng.

Có một vài cách để di chuyển dữ liệu cơ sở dữ liệu Web Access:

- Nhập vào cơ sở dữ liệu Access cục bộ (. ACCDB) hoặc vào một tệp Excel.
- Chúng tôi cũng khuyên bạn nên khám phá Microsoft PowerApps làm nền tảng thay thế để tạo ra các giải pháp kinh doanh không có mã cho các thiết bị chạy web và di động.