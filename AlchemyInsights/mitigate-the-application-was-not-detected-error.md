---
title: Giảm thiểu các ứng dụng không được phát hiện lỗi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810505"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="48f48-102">Giảm thiểu lỗi "ứng dụng không được phát hiện"</span><span class="sxs-lookup"><span data-stu-id="48f48-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="48f48-103">Lỗi cài đặt ứng dụng, "ứng dụng không được phát hiện sau khi cài đặt hoàn tất thành công," báo cáo của InTune, có thể xảy ra trên tất cả các nền tảng hệ điều hành chính (Windows, iOS và Android).</span><span class="sxs-lookup"><span data-stu-id="48f48-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="48f48-104">Các trường hợp phổ biến nhất tạo ra lỗi này bao gồm:</span><span class="sxs-lookup"><span data-stu-id="48f48-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="48f48-105">Ứng dụng đã được cập nhật bên ngoài InTune (từ cửa hàng ứng dụng của bên thứ ba) sau khi triển khai ban đầu.</span><span class="sxs-lookup"><span data-stu-id="48f48-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="48f48-106">Ví dụ một số ứng dụng như Google Chrome có thể thực hiện cập nhật tự động.</span><span class="sxs-lookup"><span data-stu-id="48f48-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="48f48-107">Một người dùng đã gỡ cài đặt các ứng dụng sau khi cài đặt ban đầu.</span><span class="sxs-lookup"><span data-stu-id="48f48-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="48f48-108">Để giảm thiểu vấn đề này, đầu tiên thực hiện đánh giá các thiết bị bị ảnh hưởng để xác định tình huống trong đó lỗi xảy ra.</span><span class="sxs-lookup"><span data-stu-id="48f48-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="48f48-109">Nếu ứng dụng đã được cập nhật bên ngoài InTune, việc triển khai ứng dụng có thể được đặt để bỏ qua phiên bản ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="48f48-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="48f48-110">Để làm như vậy, trong **ứng dụng cấu hình > thông tin ứng dụng**, thiết lập **bỏ qua phiên bản ứng dụng** **có**.</span><span class="sxs-lookup"><span data-stu-id="48f48-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="48f48-111">Khi nhắm mục tiêu khách hàng, có thể thích hợp để triển khai ứng dụng là "bắt buộc" và để đảm bảo rằng phiên bản mới nhất được triển khai.</span><span class="sxs-lookup"><span data-stu-id="48f48-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="48f48-112">Ngoài ra, trên nền tảng iOS, có thể sử dụng chức năng **AutoUpdate** liên quan đến chương trình mua ổ đĩa của Apple, có thể được cấu hình để tự động cập nhật phiên bản ứng dụng mới khi chúng trở nên có sẵn.</span><span class="sxs-lookup"><span data-stu-id="48f48-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="48f48-113">Để biết thêm thông tin về khắc phục sự cố cài đặt ứng dụng, vui lòng xem [khắc phục sự cố cài đặt ứng dụng](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="48f48-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
