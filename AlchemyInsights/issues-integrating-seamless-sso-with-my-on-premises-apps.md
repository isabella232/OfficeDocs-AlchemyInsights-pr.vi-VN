---
title: Các vấn đề với việc tích hợp SSO liền mạch với các ứng dụng tại chỗ của tôi
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868772"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a><span data-ttu-id="b8d55-102">Các vấn đề với việc tích hợp SSO liền mạch với các ứng dụng tại chỗ của tôi</span><span class="sxs-lookup"><span data-stu-id="b8d55-102">Issues with integrating Seamless SSO with my on-premises apps</span></span>

<span data-ttu-id="b8d55-103">Để khắc phục sự cố với việc tích hợp SSO liền mạch với các ứng dụng tại cơ sở, hãy làm như sau:</span><span class="sxs-lookup"><span data-stu-id="b8d55-103">To troubleshoot issues with integrating Seamless SSO with on-premises applications, do the following:</span></span>

<span data-ttu-id="b8d55-104">**Các bước được đề xuất**</span><span class="sxs-lookup"><span data-stu-id="b8d55-104">**Recommended steps**</span></span>

1. <span data-ttu-id="b8d55-105">Để cấu hình một **ứng dụng tại chỗ** cho **đăng nhập đơn thông qua proxy ứng dụng**, hãy xem [khung vòm mật khẩu cho đăng nhập đơn với proxy ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span><span class="sxs-lookup"><span data-stu-id="b8d55-105">To configure an **on-premises application** for **single sign-on through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
1. <span data-ttu-id="b8d55-106">**Khắc phục sự cố về vấn đề proxy ứng dụng**: chúng tôi khuyên bạn nên bắt đầu với việc xem xét dòng khắc phục sự cố, các [vấn đề về trình kết nối proxy ứng dụng gỡ lỗi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), để xác định xem bạn có cấu hình đúng không.</span><span class="sxs-lookup"><span data-stu-id="b8d55-106">**Troubleshooting Application Proxy issues**: we recommend that you start with reviewing the troubleshooting flow, [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), to determine if Application Proxy connectors are configured correctly.</span></span> <span data-ttu-id="b8d55-107">Nếu bạn vẫn gặp sự cố khi kết nối với ứng dụng, hãy làm theo các bước khắc phục sự cố trong các [vấn đề về ứng dụng proxy ứng dụng gỡ lỗi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span><span class="sxs-lookup"><span data-stu-id="b8d55-107">If you're still having trouble connecting to the application, follow the troubleshooting steps in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="b8d55-108">Bạn có thể [xác định các vấn đề về CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) bằng cách sử dụng các công cụ gỡ lỗi của trình duyệt sau:</span><span class="sxs-lookup"><span data-stu-id="b8d55-108">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by using the following browser debug tools:</span></span>
    1. <span data-ttu-id="b8d55-109">Khởi động trình duyệt và duyệt đến ứng dụng web.</span><span class="sxs-lookup"><span data-stu-id="b8d55-109">Launch the browser and browse to the web app.</span></span>
    1. <span data-ttu-id="b8d55-110">Nhấn **F12** để đưa lên bàn điều khiển Debug.</span><span class="sxs-lookup"><span data-stu-id="b8d55-110">Press **F12** to bring up the debug console.</span></span>
    1. <span data-ttu-id="b8d55-111">Tìm cách tái tạo giao dịch và xem lại thông điệp bàn điều khiển.</span><span class="sxs-lookup"><span data-stu-id="b8d55-111">Try to reproduce the transaction, and review the console message.</span></span> <span data-ttu-id="b8d55-112">Vi phạm CORS tạo ra lỗi bàn điều khiển về nguồn gốc.</span><span class="sxs-lookup"><span data-stu-id="b8d55-112">A CORS violation produces a console error about origin.</span></span>
    1. <span data-ttu-id="b8d55-113">Một số không thể giải quyết được sự cố, chẳng hạn như khi ứng dụng của bạn chuyển hướng đến login.microsoftonline.com để xác thực và mã thông báo Access hết hạn.</span><span class="sxs-lookup"><span data-stu-id="b8d55-113">Some CORS issues can't be resolved, such as when your app redirects to login.microsoftonline.com to authenticate, and the access token expires.</span></span> <span data-ttu-id="b8d55-114">Sau đó, cuộc gọi CORS không thành công.</span><span class="sxs-lookup"><span data-stu-id="b8d55-114">The CORS call then fails.</span></span> <span data-ttu-id="b8d55-115">Một giải pháp thay thế cho kịch bản này là mở rộng thời gian của mã thông báo Access, để tránh không bị hết hạn trong suốt phiên của người dùng.</span><span class="sxs-lookup"><span data-stu-id="b8d55-115">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="b8d55-116">Để biết thêm thông tin về cách thực hiện thao tác này, hãy xem [cấu hình hạn trong Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="b8d55-116">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="b8d55-117">**Tài liệu được đề xuất**</span><span class="sxs-lookup"><span data-stu-id="b8d55-117">**Recommended documents**</span></span>

- [<span data-ttu-id="b8d55-118">Cách đặt cấu hình đăng nhập một lần vào ứng dụng proxy ứng dụng</span><span class="sxs-lookup"><span data-stu-id="b8d55-118">How to configure single sign-on to an Application Proxy application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [<span data-ttu-id="b8d55-119">Đăng nhập đơn SAML cho các ứng dụng tại chỗ với proxy ứng dụng</span><span class="sxs-lookup"><span data-stu-id="b8d55-119">SAML single sign-on for on-premises applications with Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [<span data-ttu-id="b8d55-120">Tìm hiểu và giải quyết các vấn đề về dữ liệu proxy của ứng dụng Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="b8d55-120">Understand and solve Azure Active Directory Application Proxy CORS issues</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [<span data-ttu-id="b8d55-121">Khắc phục các cấu hình ủy quyền của Kerberos ràng buộc cho proxy ứng dụng</span><span class="sxs-lookup"><span data-stu-id="b8d55-121">Troubleshoot Kerberos constrained delegation configurations for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)