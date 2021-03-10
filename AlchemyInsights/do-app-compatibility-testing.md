---
title: Thử nghiệm tương thích ứng dụng
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9138"
- "9005291"
ms.openlocfilehash: 9a6a9ea3587a851ecf842588ab73421590ce2431
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694863"
---
# <a name="do-app-compatibility-testing"></a><span data-ttu-id="a166e-102">Thử nghiệm tương thích ứng dụng</span><span class="sxs-lookup"><span data-stu-id="a166e-102">Do app compatibility testing</span></span>

<span data-ttu-id="a166e-103">Tính tương thích ứng dụng dành cho Microsoft Edge là vô cùng cao.</span><span class="sxs-lookup"><span data-stu-id="a166e-103">Application compatibility for Microsoft Edge is extremely high.</span></span> <span data-ttu-id="a166e-104">Trong thực tế, It's so cao mà Microsoft cung cấp những lời hứa tương thích sau đây:</span><span class="sxs-lookup"><span data-stu-id="a166e-104">In fact, it's so high that Microsoft provides the following compatibility promises:</span></span>
- <span data-ttu-id="a166e-105">Nếu ứng dụng này hoạt động trên Microsoft Edge 45 và các phiên bản cũ hơn, ứng dụng này sẽ hoạt động trên Microsoft Edge 77 và các phiên bản mới hơn.</span><span class="sxs-lookup"><span data-stu-id="a166e-105">If it works on Microsoft Edge 45 and earlier versions, it will work on Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="a166e-106">Nếu ứng dụng này hoạt động trên Internet Explorer, ứng dụng này sẽ hoạt động trên Microsoft Edge trong Internet Explorer Mode.</span><span class="sxs-lookup"><span data-stu-id="a166e-106">If it works on Internet Explorer, it will work on Microsoft Edge in Internet Explorer mode.</span></span>
- <span data-ttu-id="a166e-107">Nếu ứng dụng này hoạt động trên Google Chrome, ứng dụng này sẽ hoạt động trên Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="a166e-107">If it works on Google Chrome, it will work on Microsoft Edge.</span></span>

<span data-ttu-id="a166e-108">Nếu bạn có một ứng dụng mà chúng tôi không đáp ứng lời hứa này, thì chúng tôi sẽ đứng đằng sau lời hứa để khắc phục sự cố với [ứng dụng Microsoft](https://www.microsoft.com/fasttrack/microsoft-365/app-assure).</span><span class="sxs-lookup"><span data-stu-id="a166e-108">If you have an application where we don't meet this promise, then we stand behind the promise to fix it with [Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure).</span></span>

<span data-ttu-id="a166e-109">Mặc dù lời hứa này, chúng ta biết rằng nhiều tổ chức phải xác thực một số ứng dụng cho các lý do tuân thủ hoặc quản lý rủi ro.</span><span class="sxs-lookup"><span data-stu-id="a166e-109">Despite this promise, we know that many organizations must validate some applications for compliance or risk-management reasons.</span></span> <span data-ttu-id="a166e-110">Ngay cả khi chúng tôi mong đợi điều này rất đơn giản, điều quan trọng là phải được tổ chức và nghiêm ngặt trong thử nghiệm ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="a166e-110">Even though we expect this to be very straightforward, it's important to be organized and rigorous in app testing.</span></span>

<span data-ttu-id="a166e-111">Có hai cách để thực hiện kiểm tra tương thích ứng dụng:</span><span class="sxs-lookup"><span data-stu-id="a166e-111">There are two ways to do app compatibility testing:</span></span>

- <span data-ttu-id="a166e-112">**Kiểm tra Lab**: các ứng dụng được kiểm tra trong một môi trường được kiểm soát chặt chẽ với các cấu hình cụ thể.</span><span class="sxs-lookup"><span data-stu-id="a166e-112">**Lab testing**: Applications are tested in a tightly controlled environment with specific configurations.</span></span>
- <span data-ttu-id="a166e-113">**Kiểm tra thí điểm**: các ứng dụng được kiểm tra bởi một số lượng người dùng hạn chế trong môi trường công việc hàng ngày của họ bằng cách sử dụng các thiết bị của riêng họ.</span><span class="sxs-lookup"><span data-stu-id="a166e-113">**Pilot testing**: Applications are tested by a limited number of users in their daily work environment using their own devices.</span></span>

<span data-ttu-id="a166e-114">Chọn phương pháp phù hợp nhất cho từng ứng dụng và thực hiện kiểm tra trước khi khởi động cho toàn bộ tổ chức.</span><span class="sxs-lookup"><span data-stu-id="a166e-114">Choose the method that is most appropriate for each app and do the testing prior to a launch to the entire organization.</span></span>

<span data-ttu-id="a166e-115">Sau khi bạn đã đảm bảo rằng các ứng dụng của bạn tương thích, bạn đã sẵn sàng triển khai Microsoft Edge sang một nhóm thí điểm.</span><span class="sxs-lookup"><span data-stu-id="a166e-115">Once you've ensured that your apps are compatible, you're ready to deploy Microsoft Edge to a pilot group.</span></span>
