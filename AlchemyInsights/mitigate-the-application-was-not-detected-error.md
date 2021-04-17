---
title: Giảm nhẹ ứng dụng không được phát hiện lỗi
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836373"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="4c26a-102">Lỗi giảm thiểu "ứng dụng không được phát hiện"</span><span class="sxs-lookup"><span data-stu-id="4c26a-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="4c26a-103">Lỗi cài đặt ứng dụng, "ứng dụng không được phát hiện sau khi cài đặt đã hoàn tất thành công", được báo cáo bởi InTune, có thể xảy ra trên tất cả các nền tảng hệ điều hành chính (Windows, iOS và Android).</span><span class="sxs-lookup"><span data-stu-id="4c26a-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="4c26a-104">Các kịch bản phổ biến nhất tạo ra lỗi này bao gồm:</span><span class="sxs-lookup"><span data-stu-id="4c26a-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="4c26a-105">Ứng dụng này đã được cập nhật bên ngoài InTune (từ App Store của bên thứ ba) sau khi triển khai ban đầu.</span><span class="sxs-lookup"><span data-stu-id="4c26a-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="4c26a-106">Ví dụ một số ứng dụng chẳng hạn như Google Chrome có thể thực hiện cập nhật tự động.</span><span class="sxs-lookup"><span data-stu-id="4c26a-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="4c26a-107">Người dùng đã gỡ cài đặt ứng dụng sau khi cài đặt ban đầu.</span><span class="sxs-lookup"><span data-stu-id="4c26a-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="4c26a-108">Để giảm thiểu sự cố này, trước tiên hãy thực hiện xem xét các thiết bị bị ảnh hưởng để xác định kịch bản có lỗi xảy ra.</span><span class="sxs-lookup"><span data-stu-id="4c26a-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="4c26a-109">Nếu ứng dụng này đã được cập nhật bên ngoài InTune, triển khai ứng dụng có thể được thiết lập để bỏ qua phiên bản ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="4c26a-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="4c26a-110">Để thực hiện như vậy, bên dưới **thông tin ứng dụng cấu hình ứng dụng >**, hãy đặt **bỏ qua phiên bản ứng dụng** thành **có**.</span><span class="sxs-lookup"><span data-stu-id="4c26a-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="4c26a-111">Khi mục tiêu của máy khách, có thể là phù hợp để triển khai ứng dụng là "bắt buộc" và để đảm bảo rằng phiên bản mới nhất được triển khai.</span><span class="sxs-lookup"><span data-stu-id="4c26a-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="4c26a-112">Ngoài ra, trên nền tảng iOS, có thể sử dụng các chức năng **AutoUpdate** liên kết với chương trình mua âm lượng của Apple, có thể được cấu hình để tự động cập nhật các phiên bản ứng dụng mới khi chúng trở nên sẵn dùng.</span><span class="sxs-lookup"><span data-stu-id="4c26a-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="4c26a-113">Để biết thêm thông tin về khắc phục sự cố cài đặt ứng dụng, vui lòng xem [khắc phục sự cố cài đặt ứng dụng](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="4c26a-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
