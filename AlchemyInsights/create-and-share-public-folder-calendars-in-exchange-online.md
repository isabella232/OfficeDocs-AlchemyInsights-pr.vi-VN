---
title: Tạo và chia sẻ lịch thư mục công cộng trong Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "634"
- "3500007"
ms.openlocfilehash: d8b28d373db21da42b90aeef75139affd802a5d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47804085"
---
# <a name="create-and-share-public-folder-calendars-in-exchange-online"></a><span data-ttu-id="eb388-102">Tạo và chia sẻ lịch thư mục công cộng trong Exchange Online</span><span class="sxs-lookup"><span data-stu-id="eb388-102">Create and share public folder calendars in Exchange Online</span></span>

<span data-ttu-id="eb388-103">Bạn có thể tạo lịch trong thư mục công cộng chỉ trong ứng dụng khách Outlook trên máy tính.</span><span class="sxs-lookup"><span data-stu-id="eb388-103">You can create a calendar in the Public folder only from the Outlook desktop client.</span></span> <span data-ttu-id="eb388-104">Sử dụng các bước này để thiết lập các lịch thư mục công cộng:</span><span class="sxs-lookup"><span data-stu-id="eb388-104">Use these steps to set up public folder calendars:</span></span>

1. <span data-ttu-id="eb388-105">Đảm bảo các thư mục công cộng được triển khai trong Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="eb388-105">Ensure public folders are deployed in Exchange Online.</span></span> <span data-ttu-id="eb388-106">Để biết thêm thông tin, hãy xem [tạo một hộp thư thư mục công cộng](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox).</span><span class="sxs-lookup"><span data-stu-id="eb388-106">For more info, see [Create a public folder mailbox](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox).</span></span> 

2. <span data-ttu-id="eb388-107">Đảm bảo bạn đã gán quyền truy nhập cần thiết để tạo thư mục công cộng.</span><span class="sxs-lookup"><span data-stu-id="eb388-107">Ensure you're assigned necessary access permissions to create the public folder.</span></span> <span data-ttu-id="eb388-108">Để biết thêm thông tin, hãy xem [quyền đối với thư mục công cộng cho Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span><span class="sxs-lookup"><span data-stu-id="eb388-108">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span> 
  
3. <span data-ttu-id="eb388-109">Đăng nhập vào ứng dụng khách Outlook trên máy tính và đảm bảo bạn có thể truy nhập vào triển khai thư mục công cộng của bạn.</span><span class="sxs-lookup"><span data-stu-id="eb388-109">Log in to the Outlook desktop client and ensure you can access your public folder deployment.</span></span>

    <span data-ttu-id="eb388-110">Nếu bạn đang gặp sự cố khi truy nhập vào các thư mục công cộng bằng cách sử dụng máy khách Outlook, hãy xem mục [người dùng Exchange Online không thể kết nối với các thư mục công cộng bằng cách dùng Outlook hoặc OWA](https://aka.ms/pfcte).</span><span class="sxs-lookup"><span data-stu-id="eb388-110">If you're having trouble accessing public folders by using the Outlook desktop client, see [Exchange Online users can't connect to public folders by using Outlook or OWA](https://aka.ms/pfcte).</span></span>

4. <span data-ttu-id="eb388-111">Tạo kiểu lịch công cộng mới.</span><span class="sxs-lookup"><span data-stu-id="eb388-111">Create a new public folder calendar type.</span></span>

<span data-ttu-id="eb388-112">Thư mục công cộng được chia sẻ với tất cả những người dùng khác theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="eb388-112">The public folder is shared to all other users by default.</span></span> <span data-ttu-id="eb388-113">Chủ sở hữu thư mục công cộng có thể thay đổi quyền từ ứng dụng khách Outlook trên máy tính.</span><span class="sxs-lookup"><span data-stu-id="eb388-113">Owner of the public folder can change the permissions from Outlook desktop client.</span></span> <span data-ttu-id="eb388-114">Để biết thêm thông tin, hãy xem [quyền đối với thư mục công cộng cho Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span><span class="sxs-lookup"><span data-stu-id="eb388-114">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span>

<span data-ttu-id="eb388-115">**Ghi chú** Các lịch thư mục công cộng được thiết kế để sử dụng trong tổ chức và không thể phát hành trên Internet.</span><span class="sxs-lookup"><span data-stu-id="eb388-115">**Note** Public folder calendars are designed to be used within the organization and can't be published on the Internet.</span></span> <span data-ttu-id="eb388-116">Sử dụng hộp thư chung nếu ý định của bạn là phát hành lịch trên Internet.</span><span class="sxs-lookup"><span data-stu-id="eb388-116">Use a shared mailbox if your intention is to publish a calendar on the  Internet.</span></span>