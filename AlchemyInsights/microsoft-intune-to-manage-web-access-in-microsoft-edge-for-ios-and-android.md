---
title: Sử dụng Microsoft InTune để quản lý truy nhập web trong Microsoft Edge for iOS và Android
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
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/10/2020
ms.locfileid: "49679613"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="343b5-102">Sử dụng Microsoft InTune để quản lý truy nhập web trong Microsoft Edge for iOS và Android</span><span class="sxs-lookup"><span data-stu-id="343b5-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="343b5-103">Microsoft Edge cho iOS và Android cho phép người dùng duyệt web từ nhiều, Hồ sơ riêng biệt hoàn toàn.</span><span class="sxs-lookup"><span data-stu-id="343b5-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="343b5-104">Các chức năng bảo vệ rộng nhất đối với dữ liệu Microsoft 365 sẽ sẵn dùng khi bạn đăng ký với bộ tính di động của doanh nghiệp + bộ bảo mật, trong đó có các tính năng của Microsoft InTune và Azure Active Directory Premium, chẳng hạn như quyền truy nhập có điều kiện.</span><span class="sxs-lookup"><span data-stu-id="343b5-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="343b5-105">Tối thiểu, bạn sẽ muốn triển khai chính sách truy nhập có điều kiện (1) cho phép người dùng kết nối từ thiết bị di động sang Microsoft Edge for iOS và Android và đó (2) thực hiện một chính sách bảo vệ trong Microsoft InTune cung cấp trải nghiệm duyệt web được bảo vệ.</span><span class="sxs-lookup"><span data-stu-id="343b5-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="343b5-106">Để hiểu cách bạn có thể sử dụng quyền truy nhập và chính sách có điều kiện, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="343b5-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="343b5-107">Áp dụng các chính sách truy nhập có điều kiện Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="343b5-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="343b5-108">Tạo các chính sách bảo vệ ứng dụng Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="343b5-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="343b5-109">Sử dụng đăng nhập đơn cho Azure Active Directory – các ứng dụng web được kết nối trong trình duyệt được bảo vệ bằng chính sách</span><span class="sxs-lookup"><span data-stu-id="343b5-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="343b5-110">Sử dụng cấu hình ứng dụng để quản lý trải nghiệm duyệt web</span><span class="sxs-lookup"><span data-stu-id="343b5-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="343b5-111">Cho phép sử dụng tài khoản cơ quan và trường học chỉ</span><span class="sxs-lookup"><span data-stu-id="343b5-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="343b5-112">Triển khai các chính sách cấu hình ứng dụng chung</span><span class="sxs-lookup"><span data-stu-id="343b5-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="343b5-113">Triển khai chính sách cấu hình ứng dụng để bảo vệ dữ liệu</span><span class="sxs-lookup"><span data-stu-id="343b5-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="343b5-114">Sử dụng Microsoft Endpoint Manager để triển khai các chính sách cấu hình ứng dụng</span><span class="sxs-lookup"><span data-stu-id="343b5-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="343b5-115">Để tìm hiểu cách truy nhập Nhật ký ứng dụng được quản lý, hãy xem [sử dụng Microsoft Edge for iOS và Android để truy nhập Nhật ký ứng dụng được quản lý](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="343b5-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
