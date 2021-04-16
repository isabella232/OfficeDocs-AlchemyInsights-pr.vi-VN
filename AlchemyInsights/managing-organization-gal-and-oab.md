---
title: Quản lý danh sách địa chỉ toàn cầu của tổ chức và sổ địa chỉ ngoại tuyến
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
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794854"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="b4f63-102">Quản lý danh sách địa chỉ toàn cầu của tổ chức (GAL) và sổ địa chỉ ngoại tuyến (OAB)</span><span class="sxs-lookup"><span data-stu-id="b4f63-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="b4f63-103">Danh sách địa chỉ toàn cầu (GAL) là một danh sách các đối tượng được hỗ trợ thư (bất kỳ loại người nhận nào có thể nhận được email) trong tổ chức.</span><span class="sxs-lookup"><span data-stu-id="b4f63-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="b4f63-104">Một GALLON được tạo tự động trong mọi tổ chức.</span><span class="sxs-lookup"><span data-stu-id="b4f63-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="b4f63-105">Bạn có thể tạo các cô gái bổ sung để phân tách người dùng theo tổ chức hoặc vị trí nhưng một người dùng duy nhất chỉ có thể nhìn thấy và sử dụng một GALLON tại một thời điểm.</span><span class="sxs-lookup"><span data-stu-id="b4f63-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="b4f63-106">Một số ứng dụng khách email, chẳng hạn như Outlook for Windows, tải xuống ứng dụng GAL for offline.</span><span class="sxs-lookup"><span data-stu-id="b4f63-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="b4f63-107">Điều này được gọi là sổ địa chỉ ngoại tuyến (OAB).</span><span class="sxs-lookup"><span data-stu-id="b4f63-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="b4f63-108">Trong Exchange Online, một OAB được Cập Nhật chỉ một lần mỗi 8 giờ, và sau đó khách hàng phải tải xuống để Cập Nhật bản sao OAB cục bộ của họ.</span><span class="sxs-lookup"><span data-stu-id="b4f63-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="b4f63-109">Bất kỳ thay đổi người nhận nào trước tiên có thể nhìn thấy được trong GAL để sau này làm cho nó vào OAB.</span><span class="sxs-lookup"><span data-stu-id="b4f63-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="b4f63-110">Dưới đây là một số quy trình GAL và OAB thường được sử dụng:</span><span class="sxs-lookup"><span data-stu-id="b4f63-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="b4f63-111">Vì nhiều lý do, bạn có thể muốn một số đối tượng bị ẩn khỏi GAL.</span><span class="sxs-lookup"><span data-stu-id="b4f63-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="b4f63-112">Vui lòng xem [ẩn người nhận khỏi danh sách địa chỉ](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="b4f63-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="b4f63-113">Nếu bạn cần cung cấp cho các nhóm người dùng cụ thể tùy chỉnh dạng xem của GAL của tổ chức, hãy xem [chính sách sổ địa chỉ trong Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="b4f63-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="b4f63-114">[Tạo danh sách địa chỉ toàn cầu trong Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) và để tìm hiểu cách làm việc với các quyền gal, hãy xem [danh sách địa chỉ trong Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="b4f63-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="b4f63-115">Xin lưu ý rằng nếu bạn tạo ra các cô gái mới, bạn cũng có thể muốn tạo một OAB mới.</span><span class="sxs-lookup"><span data-stu-id="b4f63-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="b4f63-116">Xem [quy trình sổ địa chỉ ngoại tuyến](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="b4f63-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
