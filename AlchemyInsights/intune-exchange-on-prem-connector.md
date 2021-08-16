---
title: Bộ nối Exchange tại chỗ của Intune
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
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013986"
---
# <a name="intune-exchange-on-premise-connector"></a>Bộ nối Exchange tại chỗ của Intune

Để biết chi tiết về cách thiết lập đường kết nối giữa Intune và Exchange thư được lưu trữ tại chỗ, vui lòng xem tài liệu sau:

[Thiết lập bộ nối Exchange tại chỗ Intune trong Azure Microsoft Intune](https://docs.microsoft.com/intune/exchange-connector-install)

**Câu hỏi thường gặp:**

H: Tôi thấy lỗi như "Phiên bản Bộ nối Exchange không được hỗ trợ" khi tìm cách thiết lập bộ nối Exchange kết nối. Nguyên nhân có thể là gì?

Đáp: Tài khoản bạn đang sử dụng được cấp phép phù hợp - tài khoản phải có giấy phép Intune hiện hoạt

Hỏi: Có thể có nhiều đường kết nối Exchange không?

A: Bạn chỉ có thể thiết lập một trình kết nối Exchange cho mỗi đối tượng thuê Intune cho Exchange chức. Chỉ có thể cài đặt bộ nối trên một máy chủ trong tổ chức trao đổi nhiều máy chủ.

Bạn cũng không thể cấu hình các đường kết nối cho Exchange tại chỗ và Exchange Online cấu hình trong cùng một đối tượng thuê.

Hỏi: Bộ nối có thể dùng mảng CAS làm kết nối của nó với đường kết Exchange?

A: Việc xác định mảng CAS không phải là một cấu hình được hỗ trợ trong thiết lập bộ nối. Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in

dữ liệu chương trình\microsoft\microsoft Intune tại cơ sở Exchange kết nối\ OnpremiseExchangeConnectorServiceConfiguration.xml

Định vị mục nhập ```<ExchangeWebServiceURL />``` sau đây và thay thế URL bằng máy chủ exchange.

**Ví dụ:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Vui lòng xem tài liệu sau đây để biết thêm cách khắc phục sự cố: Khắc phục sự cố cho bộ nối Exchange tại [chỗ của Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Bật ghi nhật ký Verbose cho bộ Exchange nối**

1. Mở tệp cấu Exchange nối Theo sau để chỉnh sửa.  
Tệp được đặt tại : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Ví dụ:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Định vị TraceSourceLine bằng khóa sau: OnPremisesExchangeConnectorService  
  
3. Thay đổi giá trị nút Mức Nguồn từ Kết hợp Hoạt động Thông tin (mặc định) thành Verbose ActivityTracing  

**Ví dụ:**
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
4. Khởi động lại dịch Microsoft Intune Exchange Service  
5. Đồng bộ đầy đủ trong Cổng thông tin Intune cho đến khi hoàn tất và sau đó thay đổi XML trở lại "Information ActivityTracing" và khởi động lại Microsoft Intune Exchange Service.  
6. Vị trí của nhật ký là: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`