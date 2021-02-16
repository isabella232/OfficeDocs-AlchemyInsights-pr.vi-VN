---
title: Chính sách Nhóm
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256911"
---
# <a name="group-policy"></a><span data-ttu-id="7483f-102">Chính sách Nhóm</span><span class="sxs-lookup"><span data-stu-id="7483f-102">Group policy</span></span>

<span data-ttu-id="7483f-103">Thiết đặt cho các đối tượng người dùng và máy tính trong Azure Active Directory Services (Azure AD DS) thường được quản lý bằng các đối tượng chính sách Nhóm (GPOs).</span><span class="sxs-lookup"><span data-stu-id="7483f-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="7483f-104">Azure AD DS bao gồm tích hợp sẵn trong GPOs cho người dùng và các bộ chứa máy tính của Hh_ngá.</span><span class="sxs-lookup"><span data-stu-id="7483f-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="7483f-105">Bạn có thể tùy chỉnh các GPOs tích hợp sẵn để cấu hình chính sách nhóm khi cần thiết cho môi trường của bạn.</span><span class="sxs-lookup"><span data-stu-id="7483f-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="7483f-106">Các thành viên của nhóm người quản trị Azure AD DC có các đặc quyền quản trị chính sách nhóm trong tên miền Azure AD DS và cũng có thể tạo các đơn vị GPOs và tổ chức tùy chỉnh (ơ).</span><span class="sxs-lookup"><span data-stu-id="7483f-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="7483f-107">Để biết thêm thông tin về chính sách nhóm là gì và cách thức hoạt động, hãy xem [tổng quan về chính sách Nhóm](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span><span class="sxs-lookup"><span data-stu-id="7483f-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="7483f-108">Trong môi trường hỗn hợp, chính sách nhóm được cấu hình trong môi trường AD DS tại cơ sở không được đồng bộ hóa với Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="7483f-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="7483f-109">Để xác định thiết đặt cấu hình cho người dùng hoặc máy tính trong Azure AD DS, hãy chỉnh sửa một trong các phần mặc định của GPOs hoặc tạo một GPO tùy chỉnh.</span><span class="sxs-lookup"><span data-stu-id="7483f-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="7483f-110">Bài viết này [quản lý chính sách Nhóm](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) hướng dẫn bạn cách cài đặt công cụ quản lý chính sách nhóm, làm thế nào tấn chỉnh sửa GPOs tích hợp sẵn và cách tạo GPOs tùy chỉnh.</span><span class="sxs-lookup"><span data-stu-id="7483f-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



