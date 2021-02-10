---
title: Triển khai AD FS
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
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177711"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="446c1-102">Triển khai AD FS</span><span class="sxs-lookup"><span data-stu-id="446c1-102">Deploy AD FS</span></span>

<span data-ttu-id="446c1-103">Triển khai dịch vụ liên kết Active Directory (AD FS) sử dụng cơ sở hạ tầng tại chỗ của bạn để xác thực người dùng cho các dịch vụ Office 365.</span><span class="sxs-lookup"><span data-stu-id="446c1-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="446c1-104">Với đăng nhập được liên kết, bạn có thể cho phép người dùng đăng nhập vào các dịch vụ và phần mềm Office 365 dưới dạng các ứng dụng dịch vụ (SAAS) được tích hợp với Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="446c1-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="446c1-105">Xác thực đăng nhập đã liên kết người dùng đối với Active Directory tại chỗ của bạn thông qua AD FS.</span><span class="sxs-lookup"><span data-stu-id="446c1-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="446c1-106">Ngoài ra, khi ở trên mạng công ty, người dùng sẽ không được yêu cầu nhập lại mật khẩu của họ.</span><span class="sxs-lookup"><span data-stu-id="446c1-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="446c1-107">[Cố vấn triển khai AD FS](https://go.microsoft.com/fwlink/?linkid=2071178) cung cấp cho bạn hướng dẫn từng bước về triển khai cơ sở hạ tầng AD FS tại cơ sở xác định người dùng cho các dịch vụ Microsoft 365 và Office 365.</span><span class="sxs-lookup"><span data-stu-id="446c1-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="446c1-108">Với hướng dẫn này, tổ chức của bạn có thể xem lại các cấu phần và yêu cầu AD FS, thu thập và cài đặt chứng chỉ SSL cần thiết để triển khai và cài đặt máy chủ proxy của ứng dụng web bắt buộc.</span><span class="sxs-lookup"><span data-stu-id="446c1-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>
