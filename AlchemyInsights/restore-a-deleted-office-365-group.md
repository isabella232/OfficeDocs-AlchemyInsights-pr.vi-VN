---
title: Khôi phục nhóm Microsoft 365 đã xóa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645153"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="4b4d6-102">Khôi phục nhóm Microsoft 365 đã xóa</span><span class="sxs-lookup"><span data-stu-id="4b4d6-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="4b4d6-103">Bạn có thể khôi phục một nhóm Microsoft 365 đã xóa hoặc các nhóm Microsoft trong vòng 30 ngày kể từ khi xóa.</span><span class="sxs-lookup"><span data-stu-id="4b4d6-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="4b4d6-104">Đi đến [Trung tâm quản trị Microsoft 365](https://aka.ms/RestoreDeletedGroup) để đăng nhập vào danh sách bạn là nhóm và nhóm đã xóa.</span><span class="sxs-lookup"><span data-stu-id="4b4d6-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of your the deleted groups and teams.</span></span>

    <span data-ttu-id="4b4d6-105">**Lưu ý:** Đăng nhập bằng cách sử dụng tài khoản được gán cho người quản trị đối tượng thuê hoặc vai trò quản trị nhóm.</span><span class="sxs-lookup"><span data-stu-id="4b4d6-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="4b4d6-106">Chọn Nhóm Microsoft 365/nhóm đã xóa sẽ được khôi phục và bấm **khôi phục nhóm**.</span><span class="sxs-lookup"><span data-stu-id="4b4d6-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="4b4d6-107">Nếu nhóm không thể khôi phục do địa chỉ SMTP xung đột, hãy dùng lệnh sau để tìm đối tượng gây ra xung đột và loại bỏ địa chỉ SMTP:</span><span class="sxs-lookup"><span data-stu-id="4b4d6-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="4b4d6-108">**Lưu ý:** Trong một số trường hợp, có thể mất đến 24 giờ cho nhóm và tất cả dữ liệu của nó sẽ được khôi phục.</span><span class="sxs-lookup"><span data-stu-id="4b4d6-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="4b4d6-109">Để biết thêm thông tin, hoặc để tìm hiểu cách khôi phục nhóm bằng PowerShell, hãy xem [khôi phục nhóm Microsoft 365 đã xóa](https://go.microsoft.com/fwlink/?linkid=867802).</span><span class="sxs-lookup"><span data-stu-id="4b4d6-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>