---
title: Cấu hình mã hóa thư cho môi trường hỗn hợp
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747943"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="0e9ed-102">Cấu hình mã hóa thư cho môi trường hỗn hợp</span><span class="sxs-lookup"><span data-stu-id="0e9ed-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="0e9ed-103">Để biết môi trường trao đổi hỗn hợp, người dùng tại cơ sở có thể gửi email được mã hóa bằng cách dùng mã hóa thư Office (OME) nếu email được định tuyến qua Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="0e9ed-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="0e9ed-104">Để mã hóa email bằng OME, hãy thực hiện các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="0e9ed-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="0e9ed-105">Sử dụng trình [hướng dẫn cấu hình hỗn](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) hợp để thiết lập môi trường hỗn hợp của bạn.</span><span class="sxs-lookup"><span data-stu-id="0e9ed-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="0e9ed-106">Không cần các bước đặc biệt nào để thiết lập mã hóa.</span><span class="sxs-lookup"><span data-stu-id="0e9ed-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="0e9ed-107">[Thiết lập các quy tắc dòng thư của bạn để mã hóa](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) như bình thường.</span><span class="sxs-lookup"><span data-stu-id="0e9ed-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>


