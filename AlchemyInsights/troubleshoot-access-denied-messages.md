---
title: Khắc phục sự cố truy cập từ chối các thư
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: f1a4803838b6511ef4fe7f03cafa4aa13b3c9734
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420722"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="07a69-102">Khắc phục sự cố truy cập từ chối các thư</span><span class="sxs-lookup"><span data-stu-id="07a69-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="07a69-103">Nếu ai đó đã thông báo "Truy cập từ chối" đến một thư mục được chia sẻ, bộ sưu tập trang web quản trị có thể đã kích hoạt "truy cập giới hạn cho phép khoá chế độ người dùng."</span><span class="sxs-lookup"><span data-stu-id="07a69-103">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="07a69-104">Để tắt này:</span><span class="sxs-lookup"><span data-stu-id="07a69-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="07a69-105">Duyệt đến trang web, hãy nhấp vào biểu tượng cài đặt và sau đó nhấp vào **Thiết lập trang web**.</span><span class="sxs-lookup"><span data-stu-id="07a69-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="07a69-106">Theo **Cục quản lý bộ sưu tập trang web**, nhấp vào **tính năng bộ sưu tập trang web**.</span><span class="sxs-lookup"><span data-stu-id="07a69-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="07a69-107">Bên cạnh **chế độ khoá cứng cho phép hạn chế truy cập người dùng**, nhấp vào **vô hiệu hóa**.</span><span class="sxs-lookup"><span data-stu-id="07a69-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="07a69-108">Thông báo truy cập từ chối cũng có thể xảy ra cho cặp chia sẻ nếu các trang web là một trang web xuất bản.</span><span class="sxs-lookup"><span data-stu-id="07a69-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="07a69-109">Để thông tin, hãy xem [Truy cập từ chối khi truy cập vào một thư mục được chia sẻ](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="07a69-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="07a69-110">Nếu một ai đó nhận một tin nhắn "Truy cập từ chối" khi cố gắng để xem yêu cầu truy cập, người dùng cần phải được thêm vào như là một quản trị viên bộ sưu tập trang web hay một thành viên của nhóm chủ sở hữu cho các trang web.</span><span class="sxs-lookup"><span data-stu-id="07a69-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="07a69-111">Để biết thêm chi tiết, hãy xem [Truy cập từ chối yêu cầu truy cập danh sách](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="07a69-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="07a69-112">Nếu người dùng nhận một tin nhắn "Truy cập từ chối" sau khi họ đã được gỡ bỏ từ Active Directory tại chỗ và sau đó thêm vào lại, hãy xem [Truy cập từ chối khi trương mục người dùng đồng bộ hóa với Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="07a69-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

