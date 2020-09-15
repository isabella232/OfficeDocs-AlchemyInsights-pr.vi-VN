---
title: Active Directory không đồng bộ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697651"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="5e956-102">Active Directory không đồng bộ</span><span class="sxs-lookup"><span data-stu-id="5e956-102">Active Directory not syncing</span></span>

<span data-ttu-id="5e956-103">Nếu bạn đang nhận được các lỗi đồng bộ hóa, chẳng hạn như "không đồng bộ hóa gần đây", hoặc thông báo trạng thái đồng bộ hóa thư mục trong cổng thông tin quản trị Office cho biết: "cuối cùng đã đồng bộ hơn 3 ngày trước," có thể là liên kết này có thiết đặt không chính xác hoặc không đủ quyền để thực hiện đồng bộ.</span><span class="sxs-lookup"><span data-stu-id="5e956-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="5e956-104">Cài đặt lại kết nối bằng cách sử dụng các thiết đặt nhanh có thể giải quyết sự cố nhanh chóng:</span><span class="sxs-lookup"><span data-stu-id="5e956-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="5e956-105">[Tải xuống phiên bản mới nhất của Badconnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="5e956-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="5e956-106">[Làm theo hướng dẫn để cài đặt nhanh](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="5e956-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="5e956-107">Để biết thêm thông tin về các tài khoản Dịch vụ của Badconnect, hãy xem [AZURE AD Connect: tài khoản và quyền](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="5e956-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
