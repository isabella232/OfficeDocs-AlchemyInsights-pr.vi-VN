---
title: Truy nhập có điều kiện với InTune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704808"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="820b2-102">Truy nhập có điều kiện với InTune</span><span class="sxs-lookup"><span data-stu-id="820b2-102">Conditional Access with Intune</span></span>

<span data-ttu-id="820b2-103">Sử dụng  **quyền truy nhập**  có điều kiện với InTune đòi hỏi phải có 3 bước:</span><span class="sxs-lookup"><span data-stu-id="820b2-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="820b2-104">Tạo  **chính sách tuân thủ**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) để xác định các thiết đặt phải được đáp ứng trước khi thiết bị được xem là tuân thủ.</span><span class="sxs-lookup"><span data-stu-id="820b2-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="820b2-105">Ví dụ: một thiết bị phải có mã pin của ít nhất 6 chữ số trước khi nó được xem là compliant.</span><span class="sxs-lookup"><span data-stu-id="820b2-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="820b2-106">Tạo một **chính sách truy nhập**  có điều kiện xác định những tài nguyên đang được bảo vệ và điều kiện nào cần được đáp ứng để truy nhập các tài nguyên đó.</span><span class="sxs-lookup"><span data-stu-id="820b2-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="820b2-107">Ví [dụ:](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) thiết bị phải tuân thủ trước khi truy nhập email công ty.</span><span class="sxs-lookup"><span data-stu-id="820b2-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="820b2-108">Đảm bảo cả **chính sách tuân thủ**  và  **chính sách truy nhập**  có điều kiện được nhắm vào các nhóm bạn muốn của người dùng.</span><span class="sxs-lookup"><span data-stu-id="820b2-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="820b2-109">Điều này có thể yêu cầu tạo các nhóm người dùng cụ thể trong Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="820b2-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="820b2-110">**Liên kết hữu ích:**</span><span class="sxs-lookup"><span data-stu-id="820b2-110">**Helpful links:**</span></span>

[<span data-ttu-id="820b2-111">Tổng quan về tuân thủ thiết bị</span><span class="sxs-lookup"><span data-stu-id="820b2-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="820b2-112">Khắc phục sự cố</span><span class="sxs-lookup"><span data-stu-id="820b2-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="820b2-113">Chính sách khắc phục sự cố</span><span class="sxs-lookup"><span data-stu-id="820b2-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="820b2-114">Để bảo vệ email (Exchange Online) từ Access bằng các thiết bị không tuân thủ, cả hai tài liệu đều phải được theo dõi:</span><span class="sxs-lookup"><span data-stu-id="820b2-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="820b2-115">Bảo vệ truy nhập email từ các thiết bị bằng cách dùng EAS</span><span class="sxs-lookup"><span data-stu-id="820b2-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="820b2-116">Bảo vệ truy nhập email từ các thiết bị bằng cách dùng các máy khách xác thực hiện đại như Outlook</span><span class="sxs-lookup"><span data-stu-id="820b2-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)