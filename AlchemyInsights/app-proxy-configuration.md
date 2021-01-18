---
title: Cấu hình proxy ứng dụng
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885533"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="0d987-102">Cấu hình proxy ứng dụng</span><span class="sxs-lookup"><span data-stu-id="0d987-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="0d987-103">Để tìm hiểu cách cấu hình ứng dụng proxy ứng dụng trong Azure AD để hiển thị các ứng dụng tại chỗ của bạn vào đám mây, hãy xem [cách cấu hình ứng dụng proxy ứng](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)dụng.</span><span class="sxs-lookup"><span data-stu-id="0d987-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="0d987-104">Đăng nhập đơn (SSO) cho phép người dùng của bạn truy nhập vào một ứng dụng mà không cần xác thực nhiều lần.</span><span class="sxs-lookup"><span data-stu-id="0d987-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="0d987-105">Nó cho phép xác thực duy nhất xảy ra trong đám mây, so với Azure Active Directory và cho phép Dịch vụ hoặc đường kết nối để mạo danh người dùng để hoàn thành bất kỳ thách thức xác thực bổ sung nào từ ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="0d987-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="0d987-106">Để tìm hiểu thêm, hãy xem [làm thế nào để cấu hình đăng nhập đơn vào ứng dụng proxy ứng dụng](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="0d987-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="0d987-107">Sử dụng [bài viết này](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) để khắc phục sự cố phổ biến mọi người phải đối mặt khi tạo ứng dụng proxy ứng dụng mới.</span><span class="sxs-lookup"><span data-stu-id="0d987-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="0d987-108">Nếu bạn đang gặp sự cố về việc thiết lập xác thực Back-end cho ứng dụng của bạn, bạn có thể cần [khắc phục các cấu hình ủy quyền của Kerberos ràng buộc đối](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) với ứng dụng proxy hoặc làm theo hướng dẫn về việc [cấu hình ứng dụng với pingaccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) để giải quyết vấn đề của bạn.</span><span class="sxs-lookup"><span data-stu-id="0d987-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
