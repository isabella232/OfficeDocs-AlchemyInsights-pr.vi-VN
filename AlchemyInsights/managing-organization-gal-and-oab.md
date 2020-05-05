---
title: Quản lý tổ chức danh sách địa chỉ toàn cầu và sổ địa chỉ gián tuyến
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a7142d68f0197aaca733766daf30fe8a46f13f9e
ms.sourcegitcommit: 8b50994a2979778ce8474ce83bd86b60e7d2cb2f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/05/2020
ms.locfileid: "44022667"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="f6272-102">Quản lý tổ chức toàn cầu địa chỉ danh sách (GAL) và sổ địa chỉ gián tuyến (OAB)</span><span class="sxs-lookup"><span data-stu-id="f6272-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="f6272-103">Danh sách địa chỉ chung (GAL) là danh sách các đối tượng được kích hoạt thư (bất kỳ loại người nhận nào có thể nhận được email) trong tổ chức.</span><span class="sxs-lookup"><span data-stu-id="f6272-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="f6272-104">Một GAL được tự động tạo ra trong mỗi tổ chức.</span><span class="sxs-lookup"><span data-stu-id="f6272-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="f6272-105">Bạn có thể tạo các GALs bổ sung để tách người dùng theo tổ chức hoặc vị trí, nhưng một người dùng chỉ có thể xem và sử dụng một GAL tại một thời gian.</span><span class="sxs-lookup"><span data-stu-id="f6272-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="f6272-106">Một số khách hàng email, chẳng hạn như Outlook dành cho Windows, tải xuống GAL để sử dụng ngoại tuyến.</span><span class="sxs-lookup"><span data-stu-id="f6272-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="f6272-107">Điều này được gọi là một sổ địa chỉ gián tuyến (OAB).</span><span class="sxs-lookup"><span data-stu-id="f6272-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="f6272-108">Trong Exchange Online, một OAB được Cập Nhật chỉ một lần 8 giờ, và sau đó khách hàng phải tải xuống để Cập Nhật bản sao OAB cục bộ của họ.</span><span class="sxs-lookup"><span data-stu-id="f6272-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="f6272-109">Bất kỳ người nhận thay đổi phải đầu tiên được hiển thị trong GAL để sau đó làm cho OAB.</span><span class="sxs-lookup"><span data-stu-id="f6272-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="f6272-110">Dưới đây là một số quy trình GAL và OAB thường được sử dụng:</span><span class="sxs-lookup"><span data-stu-id="f6272-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="f6272-111">Đối với nhiều lý do, bạn có thể muốn một số đối tượng được ẩn từ GAL.</span><span class="sxs-lookup"><span data-stu-id="f6272-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="f6272-112">Vui lòng xem [ẩn người nhận khỏi danh sách địa chỉ](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="f6272-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="f6272-113">Nếu bạn cần cung cấp cho nhóm cụ thể người dùng tuỳ chỉnh xem của tổ chức GAL, xem [chính sách sổ địa chỉ trong Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="f6272-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="f6272-114">[Tạo danh sách địa chỉ toàn cầu trong Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) và để tìm hiểu cách làm việc với quyền gal, hãy xem [danh sách địa chỉ trong Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="f6272-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="f6272-115">Xin lưu ý rằng nếu bạn tạo GALs mới, bạn cũng có thể muốn tạo một OAB mới.</span><span class="sxs-lookup"><span data-stu-id="f6272-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="f6272-116">Xem [thủ tục sổ địa chỉ gián tuyến](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="f6272-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
