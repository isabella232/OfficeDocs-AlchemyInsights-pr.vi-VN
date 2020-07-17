---
title: Truy cập có điều kiện với InTune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931458"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="8d658-102">Truy cập có điều kiện với InTune</span><span class="sxs-lookup"><span data-stu-id="8d658-102">Conditional Access with Intune</span></span>

<span data-ttu-id="8d658-103">Sử dụng **truy cập có điều kiện** với InTune yêu cầu 3 bước:</span><span class="sxs-lookup"><span data-stu-id="8d658-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="8d658-104">Tạo **chính sách tuân thủ** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) để xác định cài đặt phải được đáp ứng trước khi thiết bị được coi là tuân thủ.</span><span class="sxs-lookup"><span data-stu-id="8d658-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="8d658-105">Ví dụ: một thiết bị phải có một pin ít nhất 6 chữ số trước khi nó được coi là phù hợp.</span><span class="sxs-lookup"><span data-stu-id="8d658-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="8d658-106">Tạo **chính sách truy cập có điều kiện** xác định tài nguyên nào đang được bảo vệ và điều kiện nào cần được đáp ứng để truy cập các tài nguyên đó.</span><span class="sxs-lookup"><span data-stu-id="8d658-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="8d658-107">Ví [dụ:](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) một thiết bị phải tuân thủ trước khi truy cập email công ty.</span><span class="sxs-lookup"><span data-stu-id="8d658-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="8d658-108">Đảm bảo cả **chính sách tuân thủ** và **chính sách truy cập có điều kiện** đều được nhắm mục tiêu đến các nhóm người dùng mong muốn.</span><span class="sxs-lookup"><span data-stu-id="8d658-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="8d658-109">Điều này có thể yêu cầu tạo nhóm người dùng cụ thể trong Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8d658-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="8d658-110">**Liên kết hữu ích:**</span><span class="sxs-lookup"><span data-stu-id="8d658-110">**Helpful links:**</span></span>

[<span data-ttu-id="8d658-111">Tổng quan về tuân thủ thiết bị</span><span class="sxs-lookup"><span data-stu-id="8d658-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="8d658-112">Khắc phục sự cố CA</span><span class="sxs-lookup"><span data-stu-id="8d658-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="8d658-113">Chính sách khắc phục sự cố</span><span class="sxs-lookup"><span data-stu-id="8d658-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="8d658-114">Để bảo vệ email (Exchange Online) từ truy cập bởi các thiết bị noncompliant, cả hai tài liệu phải được tuân theo:</span><span class="sxs-lookup"><span data-stu-id="8d658-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="8d658-115">Bảo vệ truy cập email từ các thiết bị sử dụng EAS</span><span class="sxs-lookup"><span data-stu-id="8d658-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="8d658-116">Bảo vệ truy cập email từ các thiết bị sử dụng các máy khách xác thực hiện đại như Outlook</span><span class="sxs-lookup"><span data-stu-id="8d658-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)