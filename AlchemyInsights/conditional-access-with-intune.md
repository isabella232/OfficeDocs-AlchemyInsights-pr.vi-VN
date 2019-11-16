---
title: Truy cập có điều kiện với InTune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/15/2019
ms.locfileid: "36505016"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="4eb37-102">Truy cập có điều kiện với InTune</span><span class="sxs-lookup"><span data-stu-id="4eb37-102">Conditional Access with Intune</span></span>

<span data-ttu-id="4eb37-103">Sử dụng **truy cập có điều kiện** với InTune yêu cầu 3 bước:</span><span class="sxs-lookup"><span data-stu-id="4eb37-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="4eb37-104">Tạo **chính sách truy cập có điều kiện** xác định tài nguyên nào đang được bảo vệ và điều kiện nào cần được đáp ứng để truy cập các tài nguyên đó.</span><span class="sxs-lookup"><span data-stu-id="4eb37-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="4eb37-105">Ví dụ: một thiết bị phải tuân thủ trước khi truy cập email công ty.</span><span class="sxs-lookup"><span data-stu-id="4eb37-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="4eb37-106">Tạo **chính sách tuân thủ** để xác định các cài đặt phải được đáp ứng trước khi thiết bị được coi là tuân thủ.</span><span class="sxs-lookup"><span data-stu-id="4eb37-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="4eb37-107">Ví dụ: một thiết bị phải có một pin ít nhất 6 chữ số trước khi nó được coi là phù hợp.</span><span class="sxs-lookup"><span data-stu-id="4eb37-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="4eb37-108">Đảm bảo cả **chính sách tuân thủ** và **chính sách truy cập có điều kiện** được nhắm mục tiêu đến các nhóm người dùng mong muốn.</span><span class="sxs-lookup"><span data-stu-id="4eb37-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="4eb37-109">Điều này có thể yêu cầu tạo nhóm người dùng cụ thể trong Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4eb37-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="4eb37-110">Đọc thêm:</span><span class="sxs-lookup"><span data-stu-id="4eb37-110">Read more:</span></span>
  
- [<span data-ttu-id="4eb37-111">Điều kiện truy cập thực tiễn tốt nhất</span><span class="sxs-lookup"><span data-stu-id="4eb37-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="4eb37-112">Bắt đầu với truy cập có điều kiện</span><span class="sxs-lookup"><span data-stu-id="4eb37-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

