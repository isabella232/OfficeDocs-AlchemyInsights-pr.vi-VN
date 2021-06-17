---
title: Sử dụng Microsoft Intune để quản lý quyền truy nhập web trong Microsoft Edge dành cho iOS và Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989730"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="b6877-102">Sử dụng Microsoft Intune để quản lý quyền truy nhập web trong Microsoft Edge dành cho iOS và Android</span><span class="sxs-lookup"><span data-stu-id="b6877-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="b6877-103">Microsoft Edge for iOS và Android cho phép người dùng duyệt web từ nhiều hồ sơ hoàn toàn tách biệt.</span><span class="sxs-lookup"><span data-stu-id="b6877-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="b6877-104">Các chức năng bảo vệ mở rộng nhất cho dữ liệu Microsoft 365 sẽ sẵn dùng khi bạn đăng ký bộ Enterprise Mobility + Security, bao gồm các tính năng của Microsoft Intune và Azure Active Directory Premium, chẳng hạn như truy nhập có điều kiện.</span><span class="sxs-lookup"><span data-stu-id="b6877-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="b6877-105">Tối thiểu, bạn sẽ muốn triển khai một chính sách truy nhập có điều kiện (1) cho phép người dùng kết nối từ các thiết bị di động với Microsoft Edge cho iOS và Android và (2) triển khai chính sách bảo vệ ứng dụng của Microsoft Intune giúp cung cấp trải nghiệm duyệt được bảo vệ.</span><span class="sxs-lookup"><span data-stu-id="b6877-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="b6877-106">Để tìm hiểu cách bạn có thể sử dụng chính sách và truy nhập có điều kiện, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="b6877-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="b6877-107">Áp dụng chính sách truy nhập có điều kiện của Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="b6877-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="b6877-108">Tạo chính sách bảo vệ ứng dụng của Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b6877-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="b6877-109">Sử dụng đăng nhập một lần cho azure Active Directory– các ứng dụng web được kết nối với Azure trong trình duyệt được bảo vệ bởi chính sách</span><span class="sxs-lookup"><span data-stu-id="b6877-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="b6877-110">Sử dụng cấu hình ứng dụng để quản lý trải nghiệm duyệt web</span><span class="sxs-lookup"><span data-stu-id="b6877-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="b6877-111">Cho phép chỉ sử dụng tài khoản cơ quan hoặc trường học</span><span class="sxs-lookup"><span data-stu-id="b6877-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="b6877-112">Triển khai chính sách cấu hình ứng dụng chung</span><span class="sxs-lookup"><span data-stu-id="b6877-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="b6877-113">Triển khai chính sách cấu hình ứng dụng để bảo vệ dữ liệu</span><span class="sxs-lookup"><span data-stu-id="b6877-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="b6877-114">Sử dụng Trình quản lý Điểm cuối của Microsoft để triển khai chính sách cấu hình ứng dụng</span><span class="sxs-lookup"><span data-stu-id="b6877-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="b6877-115">Để tìm hiểu cách truy cập nhật ký ứng dụng được quản lý, hãy xem Sử dụng Microsoft Edge cho iOS và Android để truy [nhập vào nhật ký ứng dụng được quản lý.](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="b6877-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
