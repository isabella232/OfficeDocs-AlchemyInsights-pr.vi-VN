---
title: Sử dụng quyền truy nhập có điều kiện với InTune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694719"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="3f214-102">Sử dụng quyền truy nhập có điều kiện với InTune</span><span class="sxs-lookup"><span data-stu-id="3f214-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="3f214-103">Sử dụng quyền truy nhập có điều kiện với InTune đòi hỏi phải có 3 bước:</span><span class="sxs-lookup"><span data-stu-id="3f214-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="3f214-104">Tạo chính sách tuân thủ để xác định các thiết đặt phải được đáp ứng trước khi thiết bị được xem là tuân thủ. Ví dụ: một thiết bị phải có mã pin của ít nhất 6 chữ số trước khi nó được xem là compliant.</span><span class="sxs-lookup"><span data-stu-id="3f214-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="3f214-105">Tạo một chính sách truy nhập có điều kiện xác định những tài nguyên đang được bảo vệ và điều kiện nào cần được đáp ứng để truy nhập các tài nguyên đó. Ví dụ: thiết bị phải tuân thủ trước khi truy nhập email công ty.</span><span class="sxs-lookup"><span data-stu-id="3f214-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="3f214-106">Đảm bảo cả chính sách tuân thủ và chính sách truy nhập có điều kiện được nhắm vào các nhóm bạn muốn của người dùng. Điều này có thể yêu cầu tạo các nhóm người dùng cụ thể trong Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3f214-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="3f214-107">Đọc thêm...</span><span class="sxs-lookup"><span data-stu-id="3f214-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
