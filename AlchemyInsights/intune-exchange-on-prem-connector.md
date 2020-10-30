---
title: Trình kết nối trên tiền đề trên InTune
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808190"
---
# <a name="intune-exchange-on-premise-connector"></a>Trình kết nối trên tiền đề trên InTune

Để biết chi tiết về cách thiết lập kết nối giữa InTune và Exchange được lưu trữ tại chỗ, vui lòng xem tài liệu sau đây:

[Thiết lập trình kết nối Exchange tại chỗ InTune trong Microsoft InTune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**DIỄN**

Hỏi: tôi thấy một lỗi chẳng hạn như "Phiên bản trình kết nối Exchange không được hỗ trợ" khi cố gắng thiết lập trình kết nối Exchange. Nguyên nhân có thể là gì?

A: tài khoản mà bạn đang dùng được cấp phép thích hợp-nó phải có giấy phép InTune hiện hoạt

Hỏi: có thể có nhiều đường kết nối Exchange không?

A: bạn chỉ có thể thiết lập một trình kết nối Exchange cho mỗi đối tượng thuê InTune cho mỗi tổ chức Exchange. Chỉ có thể cài đặt đường kết nối trên một máy chủ trong một tổ chức đa máy chủ Exchange.

Ngoài ra, bạn không thể có cấu hình đường kết nối cho cả hai giao dịch và Exchange Online được đặt cấu hình trong cùng một đối tượng thuê.

Hỏi: có thể kết nối sử dụng một mảng CAS làm kết nối với Exchange không?

A: chỉ định một mảng CAS không phải là cấu hình được hỗ trợ trong thiết lập đường kết nối. Chỉ một máy chủ duy nhất được chỉ định và phải được mã hardcoded trong tệp cấu hình kết nối có thể được tìm thấy trong

chương trình data\microsoft\microsoft InTune trên đường kết nối trao đổi giao dịch OnpremiseExchangeConnectorServiceConfiguration.xml

Xác định vị trí mục nhập sau ```<ExchangeWebServiceURL />``` và thay thế URL bằng máy chủ Exchange.

**Mẫu**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Vui lòng xem tài liệu sau để khắc phục sự cố bổ sung: [khắc phục sự cố trình kết nối Exchange tại cơ sở tại chỗ](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Bật tính năng ghi nhật ký tiết ra cho trình kết nối Exchange**

1. Mở tệp cấu hình truy tìm Exchange tracing để chỉnh sửa.  
Tệp được đặt tại:%ProgramData%\Microsoft\Windows InTune Exchange Connector\TracingConfiguration.xml  

**Mẫu**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Xác định vị trí TraceSourceLine với khóa sau: OnPremisesExchangeConnectorService  
  
3. Thay đổi giá trị nút SourceLevel từ Activitruy tìm thông tin (mặc định) đến verbose ActivityTracing  

**Mẫu**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Khởi động lại dịch vụ Exchange Microsoft InTune  
5. Đồng bộ đầy đủ trong InTune Portal cho đến khi kết thúc, rồi thay đổi XML Back to "thông tin ActivityTracing" và khởi động lại dịch vụ Exchange InTune của Microsoft.  
6. Vị trí của Nhật ký là: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`