---
title: 902 (lỗi đồng bộ hoá do các đối tượng trùng lặp)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767163"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="d8d9c-102">Lỗi đồng bộ hóa do các đối tượng trùng lặp</span><span class="sxs-lookup"><span data-stu-id="d8d9c-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="d8d9c-103">Bạn có thể nhận được một thông báo lỗi sau khi đồng bộ hóa thư mục kết thúc trong Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="d8d9c-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="d8d9c-104">Không thể cập nhật đối tượng này trong dịch vụ trực tuyến của Microsoft do các thuộc tính sau liên quan đến đối tượng này có giá trị có thể đã được liên kết với một đối tượng trong thư mục địa phương của bạn.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="d8d9c-105">Đối tượng được đồng bộ hoá với cùng một địa chỉ proxy đã tồn tại trong thư mục Dịch vụ Microsoft Online của bạn.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="d8d9c-106">Không thể cập nhật đối tượng này vì các thuộc tính sau liên quan đến đối tượng này có giá trị có thể đã được liên kết với một đối tượng trong dịch vụ thư mục địa phương của bạn: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="d8d9c-107">Để xác định và khắc phục sự cố, tải xuống và chạy [công cụ sửa chữa lỗi Idfix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="d8d9c-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="d8d9c-108">Để biết thêm thông tin, xem [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="d8d9c-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
