---
title: Làm thế nào để vô hiệu hóa nhóm bên ngoài
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36739515"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="0781a-102">Làm thế nào để vô hiệu hóa nhóm bên ngoài</span><span class="sxs-lookup"><span data-stu-id="0781a-102">How to disable External Groups</span></span>

<span data-ttu-id="0781a-103">Thông điệp bên ngoài yammer áp dụng quy tắc truyền tải Exchange (ETRs), một tập hợp các điều khiển chủ động để ngăn chặn chia sẻ công ty.</span><span class="sxs-lookup"><span data-stu-id="0781a-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="0781a-104">Để hạn chế người dùng tạo nhóm bên ngoài, bạn cần cấu hình quy tắc truyền tải Exchange (ETR), và sau đó cấu hình yammer sử dụng quy tắc truyền tải Exchange để chặn tin nhắn bên ngoài.</span><span class="sxs-lookup"><span data-stu-id="0781a-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="0781a-105">Khi bạn đã tạo một quy tắc trong Trung tâm quản trị Exchange Online, hãy làm theo các bước sau để đặt ETR áp dụng trong yammer:</span><span class="sxs-lookup"><span data-stu-id="0781a-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="0781a-106">Đăng nhập vào yammer với tư cách là quản trị viên đã xác minh và trong **Trung tâm quản trị yammer**, đi tới **nội dung C và thiết đặt bảo mật an ninh \> .**</span><span class="sxs-lookup"><span data-stu-id="0781a-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="0781a-107">Trong **nhắn tin bên ngoài**, chọn thực **thi quy tắc truyền tải Exchange Online Exchange (etrs) trong yammer.**</span><span class="sxs-lookup"><span data-stu-id="0781a-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="0781a-108">Chọn **lưu**.</span><span class="sxs-lookup"><span data-stu-id="0781a-108">Choose **Save**.</span></span>

<span data-ttu-id="0781a-109">Để biết thêm thông tin, xem [vô hiệu hoá nhắn tin bên ngoài trong mạng yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="0781a-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  