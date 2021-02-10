---
title: Vấn đề với nhóm bảo mật
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177638"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="453cc-102">Vấn đề với nhóm bảo mật</span><span class="sxs-lookup"><span data-stu-id="453cc-102">Issue with security groups</span></span>

<span data-ttu-id="453cc-103">**Nếu bạn đang nhận được thông báo lỗi mạng AADDS104**</span><span class="sxs-lookup"><span data-stu-id="453cc-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="453cc-104">Các quy tắc nhóm bảo mật mạng không hợp lệ là nguyên nhân phổ biến nhất của các lỗi mạng cho Azure dịch vụ miền Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="453cc-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="453cc-105">Nhóm bảo mật mạng cho mạng ảo phải cho phép truy nhập vào các cổng và giao thức cụ thể.</span><span class="sxs-lookup"><span data-stu-id="453cc-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="453cc-106">Nếu các cổng này bị chặn, nền tảng Azure không thể theo dõi hoặc Cập Nhật tên miền được quản lý.</span><span class="sxs-lookup"><span data-stu-id="453cc-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="453cc-107">Đồng bộ hóa giữa các Azure AD và Azure AD DS cũng bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="453cc-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="453cc-108">Đảm bảo bạn tiếp tục mở cổng thông tin mặc định để tránh bị gián đoạn dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="453cc-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="453cc-109">Để hiểu và giải quyết các vấn đề về cấu hình nhóm bảo mật mạng, hãy xem mục [Thêm và xác nhận nhóm bảo mật](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span><span class="sxs-lookup"><span data-stu-id="453cc-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
