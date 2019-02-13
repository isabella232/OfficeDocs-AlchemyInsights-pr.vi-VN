---
title: Làm thế nào để vô hiệu hóa nhóm bên ngoài
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4d911c319c3e8e327f9b3af3ba67816e646bc468
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29899158"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="038e3-102">Làm thế nào để vô hiệu hóa nhóm bên ngoài</span><span class="sxs-lookup"><span data-stu-id="038e3-102">How to disable External Groups</span></span>

<span data-ttu-id="038e3-p101">Yammer tin nhắn bên ngoài áp dụng quy tắc truyền tải Exchange (ETRs), một bộ điều khiển chủ động ngăn chặn thông tin công ty được chia sẻ. Để hạn chế người dùng tạo các nhóm bên ngoài, bạn cần phải đặt cấu hình quy tắc truyền tải Exchange (ETR), và sau đó cấu hình Yammer sử dụng quy tắc truyền tải Exchange để chặn tin nhắn bên ngoài.</span><span class="sxs-lookup"><span data-stu-id="038e3-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="038e3-105">Một khi bạn đã tạo ra một quy tắc trong Trung tâm quản trị Exchange Online, hãy làm theo các bước sau để thiết lập ETR để áp dụng trong Yammer:</span><span class="sxs-lookup"><span data-stu-id="038e3-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="038e3-106">Đăng nhập vào Yammer như là một quản trị viên xác minh, và trong **Yammer Trung tâm quản trị**, hãy vào C **ontent và an ninh \> cài đặt bảo mật.**</span><span class="sxs-lookup"><span data-stu-id="038e3-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="038e3-107">Theo **Tin nhắn bên ngoài**, chọn **thực thi của bạn trao đổi trực tuyến trao đổi quy tắc truyền tải (ETRs) ở Yammer.**</span><span class="sxs-lookup"><span data-stu-id="038e3-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="038e3-108">Chọn **lưu**.</span><span class="sxs-lookup"><span data-stu-id="038e3-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="038e3-109">Để biết thêm chi tiết, hãy xem [kiểm soát bên ngoài tin nhắn trong một mạng Yammer với quy tắc truyền tải Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="038e3-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

