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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="5bee4-102">Trình kết nối trên tiền đề trên InTune</span><span class="sxs-lookup"><span data-stu-id="5bee4-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="5bee4-103">Để biết chi tiết về cách thiết lập kết nối giữa InTune và Exchange được lưu trữ tại chỗ, vui lòng xem tài liệu sau đây:</span><span class="sxs-lookup"><span data-stu-id="5bee4-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="5bee4-104">Thiết lập trình kết nối Exchange tại chỗ InTune trong Microsoft InTune Azure</span><span class="sxs-lookup"><span data-stu-id="5bee4-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="5bee4-105">**DIỄN**</span><span class="sxs-lookup"><span data-stu-id="5bee4-105">**FAQ:**</span></span>

<span data-ttu-id="5bee4-106">Hỏi: tôi thấy một lỗi chẳng hạn như "Phiên bản trình kết nối Exchange không được hỗ trợ" khi cố gắng thiết lập trình kết nối Exchange.</span><span class="sxs-lookup"><span data-stu-id="5bee4-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="5bee4-107">Nguyên nhân có thể là gì?</span><span class="sxs-lookup"><span data-stu-id="5bee4-107">What could be the cause?</span></span>

<span data-ttu-id="5bee4-108">A: tài khoản mà bạn đang dùng được cấp phép thích hợp-nó phải có giấy phép InTune hiện hoạt</span><span class="sxs-lookup"><span data-stu-id="5bee4-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="5bee4-109">Hỏi: có thể có nhiều đường kết nối Exchange không?</span><span class="sxs-lookup"><span data-stu-id="5bee4-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="5bee4-110">A: bạn chỉ có thể thiết lập một trình kết nối Exchange cho mỗi đối tượng thuê InTune cho mỗi tổ chức Exchange.</span><span class="sxs-lookup"><span data-stu-id="5bee4-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="5bee4-111">Chỉ có thể cài đặt đường kết nối trên một máy chủ trong một tổ chức đa máy chủ Exchange.</span><span class="sxs-lookup"><span data-stu-id="5bee4-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="5bee4-112">Ngoài ra, bạn không thể có cấu hình đường kết nối cho cả hai giao dịch và Exchange Online được đặt cấu hình trong cùng một đối tượng thuê.</span><span class="sxs-lookup"><span data-stu-id="5bee4-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="5bee4-113">Hỏi: có thể kết nối sử dụng một mảng CAS làm kết nối với Exchange không?</span><span class="sxs-lookup"><span data-stu-id="5bee4-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="5bee4-114">A: chỉ định một mảng CAS không phải là cấu hình được hỗ trợ trong thiết lập đường kết nối.</span><span class="sxs-lookup"><span data-stu-id="5bee4-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="5bee4-115">Chỉ một máy chủ duy nhất được chỉ định và phải được mã hardcoded trong tệp cấu hình kết nối có thể được tìm thấy trong</span><span class="sxs-lookup"><span data-stu-id="5bee4-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="5bee4-116">chương trình data\microsoft\microsoft InTune trên đường kết nối trao đổi giao dịch OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="5bee4-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="5bee4-117">Xác định vị trí mục nhập sau ```<ExchangeWebServiceURL />``` và thay thế URL bằng máy chủ Exchange.</span><span class="sxs-lookup"><span data-stu-id="5bee4-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="5bee4-118">**Mẫu**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="5bee4-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="5bee4-119">Vui lòng xem tài liệu sau để khắc phục sự cố bổ sung: [khắc phục sự cố trình kết nối Exchange tại cơ sở tại chỗ](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="5bee4-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="5bee4-120">**Bật tính năng ghi nhật ký tiết ra cho trình kết nối Exchange**</span><span class="sxs-lookup"><span data-stu-id="5bee4-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="5bee4-121">Mở tệp cấu hình truy tìm Exchange tracing để chỉnh sửa.</span><span class="sxs-lookup"><span data-stu-id="5bee4-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="5bee4-122">Tệp được đặt tại:%ProgramData%\Microsoft\Windows InTune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="5bee4-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="5bee4-123">**Mẫu**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="5bee4-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="5bee4-124">Xác định vị trí TraceSourceLine với khóa sau: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="5bee4-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="5bee4-125">Thay đổi giá trị nút SourceLevel từ Activitruy tìm thông tin (mặc định) đến verbose ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="5bee4-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="5bee4-126">**Mẫu**</span><span class="sxs-lookup"><span data-stu-id="5bee4-126">**Example:**</span></span>
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
4. <span data-ttu-id="5bee4-127">Khởi động lại dịch vụ Exchange Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="5bee4-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="5bee4-128">Đồng bộ đầy đủ trong InTune Portal cho đến khi kết thúc, rồi thay đổi XML Back to "thông tin ActivityTracing" và khởi động lại dịch vụ Exchange InTune của Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5bee4-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="5bee4-129">Vị trí của Nhật ký là: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="5bee4-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>