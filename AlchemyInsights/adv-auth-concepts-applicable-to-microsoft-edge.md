---
title: Các khái niệm xác thực nâng cao áp dụng cho Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573782"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="e0a04-102">Các khái niệm xác thực nâng cao áp dụng cho Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="e0a04-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="e0a04-103">Sau đây là các khái niệm xác thực nâng cao được áp dụng cho Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="e0a04-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="e0a04-104">**Xác thực chủ động**</span><span class="sxs-lookup"><span data-stu-id="e0a04-104">**Proactive Authentication**</span></span>

<span data-ttu-id="e0a04-105">Khi bạn bật chính sách được [kích hoạt Proactiveauth,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge sẽ cố gắng để xác thực chủ động cho người dùng được đăng nhập thông qua Microsoft Services.</span><span class="sxs-lookup"><span data-stu-id="e0a04-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="e0a04-106">Tại các khoảng thời gian thường xuyên, nó sẽ sử dụng một dịch vụ trực tuyến để kiểm tra biểu thị được Cập Nhật có chứa xác thực chủ động quản lý cấu hình.</span><span class="sxs-lookup"><span data-stu-id="e0a04-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="e0a04-107">Lợi ích: xác thực chủ động cho phép xác thực cho các dịch vụ khóa, chẳng hạn như trang tab mới của Office.</span><span class="sxs-lookup"><span data-stu-id="e0a04-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="e0a04-108">Ngoài ra, nếu Bing được dùng làm công cụ tìm kiếm, xác thực chủ động sẽ cải thiện hiệu suất của thanh địa chỉ và giúp tạo các kết quả tìm kiếm được cá nhân hóa với nhu cầu của doanh nghiệp của bạn.</span><span class="sxs-lookup"><span data-stu-id="e0a04-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="e0a04-109">**Windows Xin chào CredUI để xác thực NTLM**</span><span class="sxs-lookup"><span data-stu-id="e0a04-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="e0a04-110">Nếu đăng nhập đơn (SSO) không sẵn dùng khi một trang web cố gắng đăng nhập vào người dùng thông qua công trình NTLM hoặc thương lượng, tính năng này sẽ cho phép người dùng chia sẻ thông tin đăng nhập hệ điều hành với trang web và thỏa mãn thách thức xác thực bằng cách dùng Windows Hello cred UI.</span><span class="sxs-lookup"><span data-stu-id="e0a04-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="e0a04-111">Dòng đăng nhập này sẽ chỉ xuất hiện trong Windows 10 và chỉ dành cho những người dùng không nhận được SSO trong một NTLM hoặc một thách thức thương lượng.</span><span class="sxs-lookup"><span data-stu-id="e0a04-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="e0a04-112">**Sử dụng mật khẩu đã lưu để đăng nhập tự động**</span><span class="sxs-lookup"><span data-stu-id="e0a04-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="e0a04-113">Người dùng lưu mật khẩu trong Microsoft Edge có thể bật tính năng đăng nhập tự động vào các trang web mà họ đã lưu chứng danh.</span><span class="sxs-lookup"><span data-stu-id="e0a04-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="e0a04-114">Người dùng có thể bật hoặc tắt tính năng này trong edge://settings/passwords và bạn có thể cấu hình nó trong chính sách [trình quản lý mật khẩu](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="e0a04-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
