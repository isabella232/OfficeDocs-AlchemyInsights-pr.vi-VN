---
title: 902 (sync lỗi do các đối tượng trùng lặp)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 06cd582c30a59a94ee117728bd5daebecca77bc8
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758017"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="1a528-102">Lỗi đồng bộ hóa do các đối tượng trùng lặp</span><span class="sxs-lookup"><span data-stu-id="1a528-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="1a528-103">Bạn có thể nhận được một trong các thông báo lỗi sau khi đồng bộ hoá thư mục kết thúc:</span><span class="sxs-lookup"><span data-stu-id="1a528-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>

- <span data-ttu-id="1a528-104">Không thể cập nhật các đối tượng này ở Microsoft dịch vụ trực tuyến bởi vì các thuộc tính sau đây liên quan đến đối tượng này có giá trị có thể đã được liên kết với các đối tượng khác trong thư mục địa phương của bạn.</span><span class="sxs-lookup"><span data-stu-id="1a528-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="1a528-105">Một đối tượng được đồng bộ hoá với cùng một địa chỉ proxy đã tồn tại trong thư mục Microsoft dịch vụ trực tuyến của bạn.</span><span class="sxs-lookup"><span data-stu-id="1a528-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="1a528-106">Không thể cập nhật các đối tượng này bởi vì các thuộc tính sau đây liên quan đến đối tượng này có giá trị mà có thể đã được liên kết với các đối tượng khác trong dịch vụ thư mục địa phương của bạn: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="1a528-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="1a528-107">Để xác định và khắc phục sự cố, hãy tải về và chạy [Công cụ khắc phục lỗi IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="1a528-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="1a528-108">Để biết thêm thông tin, hãy xem [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="1a528-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
