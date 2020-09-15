---
title: Cách tắt các nhóm bên ngoài
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704150"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="1d7d8-102">Cách tắt các nhóm bên ngoài</span><span class="sxs-lookup"><span data-stu-id="1d7d8-102">How to disable External Groups</span></span>

<span data-ttu-id="1d7d8-103">Nhắn tin bên ngoài yammer áp dụng quy tắc truyền dẫn Exchange (ETRs), một tập hợp các điều khiển chủ động để ngăn không cho thông tin công ty chia sẻ.</span><span class="sxs-lookup"><span data-stu-id="1d7d8-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="1d7d8-104">Để hạn chế người dùng tạo nhóm bên ngoài, bạn cần đặt cấu hình quy tắc truyền dẫn Exchange (ETR), rồi đặt cấu hình yammer để sử dụng quy tắc truyền dẫn Exchange để chặn gửi tin nhắn bên ngoài.</span><span class="sxs-lookup"><span data-stu-id="1d7d8-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="1d7d8-105">Sau khi bạn đã tạo một quy tắc trong Trung tâm quản trị Exchange Online, hãy làm theo các bước sau đây để đặt ETR để áp dụng trong yammer:</span><span class="sxs-lookup"><span data-stu-id="1d7d8-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="1d7d8-106">Đăng nhập vào yammer với tư cách là người quản trị đã xác nhận và trong **Trung tâm quản trị yammer**, hãy đi đến \*\* \> thiết đặt nội dung và bảo mật\*\* của C.</span><span class="sxs-lookup"><span data-stu-id="1d7d8-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="1d7d8-107">Bên dưới **nhắn tin bên ngoài**, chọn thực **thi quy tắc truyền dẫn Exchange Online Exchange của bạn (etrs) trong yammer.**</span><span class="sxs-lookup"><span data-stu-id="1d7d8-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="1d7d8-108">Chọn **lưu**.</span><span class="sxs-lookup"><span data-stu-id="1d7d8-108">Choose **Save**.</span></span>

<span data-ttu-id="1d7d8-109">Để biết thêm thông tin, hãy xem mục [tắt nhắn tin bên ngoài trong mạng yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="1d7d8-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  