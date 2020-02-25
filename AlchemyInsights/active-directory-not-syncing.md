---
title: Active Directory không đồng bộ hoá
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265278"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="abe0f-102">Active Directory không đồng bộ hoá</span><span class="sxs-lookup"><span data-stu-id="abe0f-102">Active Directory not syncing</span></span>

<span data-ttu-id="abe0f-103">Nếu bạn đang nhận được lỗi đồng bộ hoá, chẳng hạn như "không đồng bộ hóa gần đây" hoặc thông báo trạng thái đồng bộ hóa thư mục trong Cổng quản trị Office cho biết, "cuối cùng nhiều hơn 3 ngày trước", có thể là AADConnect có cài đặt không đúng hoặc không đủ quyền để thực hiện đồng bộ hóa.</span><span class="sxs-lookup"><span data-stu-id="abe0f-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="abe0f-104">Cài đặt lại AADConnect bằng cách sử dụng thiết lập nhanh có thể khắc phục sự cố một cách nhanh chóng:</span><span class="sxs-lookup"><span data-stu-id="abe0f-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="abe0f-105">[Tải về phiên bản mới nhất của AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="abe0f-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="abe0f-106">[Làm theo hướng dẫn để cài đặt nhanh](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="abe0f-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="abe0f-107">Để biết thêm thông tin về tài khoản Dịch vụ AADConnect, xem [AZURE AD kết nối: tài khoản và quyền](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="abe0f-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
