---
title: Nhật ký mật khẩu
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
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527776"
---
# <a name="password-logs"></a><span data-ttu-id="ae03a-102">Nhật ký mật khẩu</span><span class="sxs-lookup"><span data-stu-id="ae03a-102">Password logs</span></span>

<span data-ttu-id="ae03a-103">**Tôi đang gặp sự cố khi truy nhập Nhật ký kiểm tra đặt lại mật khẩu**</span><span class="sxs-lookup"><span data-stu-id="ae03a-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="ae03a-104">Để khắc phục sự cố về quyền truy nhập vào Nhật ký kiểm tra đặt lại mật khẩu, hãy thực hiện bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="ae03a-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="ae03a-105">Đảm bảo bạn được ủy quyền để xem Nhật ký kiểm nghiệm.</span><span class="sxs-lookup"><span data-stu-id="ae03a-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="ae03a-106">Chỉ những vai trò sau đây được ủy quyền:</span><span class="sxs-lookup"><span data-stu-id="ae03a-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="ae03a-107">Người quản trị toàn cầu</span><span class="sxs-lookup"><span data-stu-id="ae03a-107">Global administrator</span></span>
 - <span data-ttu-id="ae03a-108">Người quản trị bảo mật</span><span class="sxs-lookup"><span data-stu-id="ae03a-108">Security administrator</span></span>
 - <span data-ttu-id="ae03a-109">Bộ đọc bảo mật</span><span class="sxs-lookup"><span data-stu-id="ae03a-109">Security reader</span></span>

<span data-ttu-id="ae03a-110">**Tôi muốn xem tất cả các sự kiện kiểm tra khôi phục mật khẩu từ lúc tôi triển khai ban đầu**</span><span class="sxs-lookup"><span data-stu-id="ae03a-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="ae03a-111">Lên đến 120.000 đặt lại mật khẩu/sự kiện đăng ký được lưu trữ trong các báo cáo của 30 ngày qua.</span><span class="sxs-lookup"><span data-stu-id="ae03a-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="ae03a-112">Giới hạn tối đa này áp dụng cho giao diện người dùng khi tải xuống CSV.</span><span class="sxs-lookup"><span data-stu-id="ae03a-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="ae03a-113">sự kiện 1.000.000 sẵn dùng thông qua PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ae03a-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="ae03a-114">Để biết thêm thông tin, hãy xem các nối kết dưới đây:</span><span class="sxs-lookup"><span data-stu-id="ae03a-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="ae03a-115">Tự khôi phục mật khẩu các sự kiện từ Azure AD Reports and events API</span><span class="sxs-lookup"><span data-stu-id="ae03a-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="ae03a-116">Làm thế nào để tải lại các sự kiện đăng ký mật khẩu nhanh chóng với PowerShell</span><span class="sxs-lookup"><span data-stu-id="ae03a-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="ae03a-117">**Tôi muốn tìm hiểu thêm về các chức năng báo cáo đặt lại mật khẩu**</span><span class="sxs-lookup"><span data-stu-id="ae03a-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="ae03a-118">Kiểm tra xem ai đang đăng ký hoặc đặt lại mật khẩu có Nhật ký kiểm tra khôi phục mật khẩu Azure AD trong cổng thông tin Azure bên dưới **người dùng và nhóm**.</span><span class="sxs-lookup"><span data-stu-id="ae03a-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="ae03a-119">Để biết thêm thông tin, hãy xem các nối kết sau đây:</span><span class="sxs-lookup"><span data-stu-id="ae03a-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="ae03a-120">Tổng quan về báo cáo đặt lại mật khẩu</span><span class="sxs-lookup"><span data-stu-id="ae03a-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="ae03a-121">Cách xem báo cáo đặt lại mật khẩu trong cổng thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="ae03a-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="ae03a-122">Tự khôi phục mật khẩu các sự kiện từ Azure AD Reports and events API</span><span class="sxs-lookup"><span data-stu-id="ae03a-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="ae03a-123">Làm thế nào để tải lại các sự kiện đăng ký mật khẩu nhanh chóng với PowerShell</span><span class="sxs-lookup"><span data-stu-id="ae03a-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


