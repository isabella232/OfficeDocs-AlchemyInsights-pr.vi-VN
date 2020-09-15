---
title: lỗi 1554 Winsock 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698884"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="00d09-102">Lỗi Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="00d09-102">Winsock error 10061</span></span>

<span data-ttu-id="00d09-103">Mã lỗi này có nghĩa là Microsoft không thể thiết lập một ổ cắm TCP (kết nối) với máy chủ đích.</span><span class="sxs-lookup"><span data-stu-id="00d09-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="00d09-104">Nguyên nhân có thể nhất của lỗi này là sự cố với cấu hình tường lửa của bạn.</span><span class="sxs-lookup"><span data-stu-id="00d09-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="00d09-105">Để khắc phục sự cố, hãy kiểm tra các thiết đặt sau:</span><span class="sxs-lookup"><span data-stu-id="00d09-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="00d09-106">Xác nhận cấu hình tường lửa của bạn với thông tin trong [URL Microsoft 365 và dải địa chỉ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="00d09-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="00d09-107">Nếu lỗi cụ thể với Exchange Online Protection (EOP), bạn nên trước đó đã được thông báo đến một thay đổi đối với các [địa chỉ IP của Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="00d09-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="00d09-108">Xác minh rằng nhà cung cấp dịch vụ Internet (ISP của bạn) không ngăn không cho cổng.</span><span class="sxs-lookup"><span data-stu-id="00d09-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="00d09-109">Xác nhận thiết đặt máy chủ lưu trữ và đích thông minh trong đường kết nối của bạn.</span><span class="sxs-lookup"><span data-stu-id="00d09-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="00d09-110">Lưu ý rằng Microsoft 365 không chặn kết nối *đến* theo cách này.</span><span class="sxs-lookup"><span data-stu-id="00d09-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
