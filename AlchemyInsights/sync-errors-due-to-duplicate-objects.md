---
title: 902 (lỗi đồng bộ do các đối tượng trùng lặp)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708084"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="4b02c-102">Lỗi đồng bộ do các đối tượng trùng lặp</span><span class="sxs-lookup"><span data-stu-id="4b02c-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="4b02c-103">Bạn có thể nhận được một trong các thông báo lỗi sau đây khi đồng bộ hóa thư mục kết thúc trong Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="4b02c-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="4b02c-104">Không thể cập nhật đối tượng này trong Microsoft Online Services vì các thuộc tính sau được liên kết với đối tượng này có các giá trị mà có thể đã được liên kết với một đối tượng khác trong thư mục cục bộ của bạn.</span><span class="sxs-lookup"><span data-stu-id="4b02c-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="4b02c-105">Một đối tượng đã đồng bộ với cùng địa chỉ proxy đã tồn tại trong danh bạ Microsoft Online Services của bạn.</span><span class="sxs-lookup"><span data-stu-id="4b02c-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="4b02c-106">Không thể cập nhật đối tượng này vì các thuộc tính sau được liên kết với đối tượng này có các giá trị mà có thể đã được liên kết với một đối tượng khác trong các dịch vụ thư mục cục bộ của bạn: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="4b02c-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="4b02c-107">Để xác định và khắc phục sự cố, hãy tải xuống và chạy [công cụ khắc phục lỗi không đồng bộ Idfix Dirsync](https://github.com/Microsoft/idfix).</span><span class="sxs-lookup"><span data-stu-id="4b02c-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="4b02c-108">Để biết thêm thông tin, hãy xem [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="4b02c-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
