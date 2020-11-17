---
title: Chuẩn bị cho việc sử dụng TLS 1,2 trong Microsoft 365
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085926"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a><span data-ttu-id="8107b-102">Chuẩn bị cho việc sử dụng TLS 1,2 trong Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="8107b-102">Prepare for use of TLS 1.2 in Microsoft 365</span></span>

<span data-ttu-id="8107b-103">Tính đến ngày 31 tháng 10, 2018, Microsoft 365 sẽ tiếp tục chuyển sang TLS 1,2.</span><span class="sxs-lookup"><span data-stu-id="8107b-103">As of October 31st, 2018, Microsoft 365 will continue transitioning to TLS 1.2.</span></span> <span data-ttu-id="8107b-104">Bắt đầu từ ngày 15 tháng 10, 2020, O365 sẽ bắt đầu cuộc gọi của TLS 1,0 và 1,1 qua dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="8107b-104">Starting October 15, 2020, O365 will begin the deprecation of TLS 1.0 and 1.1 across the service.</span></span> <span data-ttu-id="8107b-105">Buổi trình phát của thay đổi này sẽ tiếp tục trong vài tuần và tháng tiếp theo, nhưng khách hàng sẽ không phải là các cuộc gọi không có TLS 1.0/1,1 sẽ hoạt động khi tham gia với O365 bắt đầu từ ngày 15 tháng 10, 2020.</span><span class="sxs-lookup"><span data-stu-id="8107b-105">The rollout of this change will continue over the next few weeks and months, but customers should assume no TLS 1.0/1.1 calls will work when engaging with O365 starting Oct 15, 2020.</span></span> <span data-ttu-id="8107b-106">Như truyền đạt (MC126199 trong tháng mười hai 2017, MC128929 trong tháng hai 2018, MC186827 trong tháng bảy 2019, và MC218794 trong tháng bảy 2020), chúng tôi đang di chuyển tất cả các dịch vụ trực tuyến của chúng tôi để truyền dẫn bảo mật tầng (TLS) 1.2 + để cung cấp mã hóa tốt nhất trong lớp và đảm bảo dịch vụ của chúng tôi là bảo mật hơn.</span><span class="sxs-lookup"><span data-stu-id="8107b-106">As previously communicated (MC126199 in Dec 2017, MC128929 in Feb 2018, MC186827 in July 2019, and MC218794 in July 2020), we are moving all of our online services to Transport Layer Security (TLS) 1.2+ to provide best-in-class encryption, and to ensure our service is more secure, by default.</span></span> <span data-ttu-id="8107b-107">Khách hàng vẫn có thể chọn để có TLS 1.0/1.1 trên các máy chủ và tài nguyên của họ, nhưng họ sẽ chỉ đối với TLS 1,2 hoặc cao hơn sẽ hoạt động khi tương tác với các tài nguyên O365.</span><span class="sxs-lookup"><span data-stu-id="8107b-107">Customers can still choose to have TLS 1.0/1.1 on their servers and resources, but they should assume only TLS 1.2 or higher will work when interacting with O365 resources.</span></span>
  
<span data-ttu-id="8107b-108">Để tìm hiểu thêm về những thay đổi này, vui lòng xem [ở đây](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) và [ở đây](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="8107b-108">To learn more about these changes, please see [here](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) and [here](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span></span>

  