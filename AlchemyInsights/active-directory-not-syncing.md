---
title: Active Directory không đồng bộ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930997"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="cd1f4-102">Active Directory không đồng bộ</span><span class="sxs-lookup"><span data-stu-id="cd1f4-102">Active Directory not syncing</span></span>

<span data-ttu-id="cd1f4-103">Nếu bạn đang nhận được lỗi đồng bộ, chẳng hạn như "không đồng bộ hóa gần đây" hoặc nhận thấy trạng thái đồng bộ hóa thư mục trong cổng thông tin quản trị Office cho biết "Đã đồng bộ lần cuối hơn 3 ngày trước", đó có thể là AADConnect có cài đặt không chính xác hoặc không đủ quyền để thực hiện đồng bộ.</span><span class="sxs-lookup"><span data-stu-id="cd1f4-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="cd1f4-104">Việc cài đặt lại AADConnect bằng cách sử dụng cài đặt nhanh có thể giải quyết sự cố một cách nhanh chóng:</span><span class="sxs-lookup"><span data-stu-id="cd1f4-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="cd1f4-105">[Tải xuống phiên bản AADConnect mới nhất.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="cd1f4-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="cd1f4-106">[Làm theo hướng dẫn để cài đặt nhanh.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="cd1f4-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="cd1f4-107">Azure AD Kết nối được cài đặt trên Windows Server 2012 trở lên.</span><span class="sxs-lookup"><span data-stu-id="cd1f4-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="cd1f4-108">Máy chủ này phải nối miền và có thể là bộ kiểm soát miền hoặc máy chủ thành viên.</span><span class="sxs-lookup"><span data-stu-id="cd1f4-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="cd1f4-109">Để biết danh sách đầy đủ các yêu cầu và Kết nối điều kiện tiên quyết của Azure AD, hãy xem lại Điều kiện tiên quyết cho [Azure AD Kết nối.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)</span><span class="sxs-lookup"><span data-stu-id="cd1f4-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="cd1f4-110">Để biết thêm thông tin về tài khoản dịch vụ AADConnect, hãy [xem mục Azure AD Kết nối: Tài khoản và quyền.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="cd1f4-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
