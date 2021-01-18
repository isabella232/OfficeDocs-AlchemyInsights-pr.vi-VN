---
title: Sự cố khi gia nhập VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885782"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="58c32-102">Sự cố khi gia nhập VMs</span><span class="sxs-lookup"><span data-stu-id="58c32-102">Issue joining VMs</span></span>

<span data-ttu-id="58c32-103">Để giải quyết các sự cố xảy ra trong khi tìm cách gia nhập VMs, hãy thực hiện các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="58c32-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="58c32-104">Tìm cách đăng nhập bằng định dạng **UPN** (ví dụ: ' joeuser@contoso.com ') thay vì định dạng **SAMAccountName** (' CONTOSO\joeuser ').</span><span class="sxs-lookup"><span data-stu-id="58c32-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="58c32-105">Đảm bảo rằng bạn đã bật tính năng đồng bộ hóa mật khẩu theo các bước được nêu trong hướng dẫn *bắt đầu* .</span><span class="sxs-lookup"><span data-stu-id="58c32-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="58c32-106">Đảm bảo rằng tài khoản người dùng bị ảnh hưởng không phải là tài khoản bên ngoài trong đối tượng thuê Azure AD.</span><span class="sxs-lookup"><span data-stu-id="58c32-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="58c32-107">Người dùng bên ngoài không thể đăng nhập vào tên miền được quản lý kể từ Azure AD Domain Services không có thông tin xác thực cho các tài khoản người dùng đó.</span><span class="sxs-lookup"><span data-stu-id="58c32-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="58c32-108">Nếu tài khoản người dùng bị ảnh hưởng là một tài khoản người dùng chỉ trên đám mây, hãy đảm bảo rằng người dùng đã thay đổi mật khẩu của họ sau khi bạn bật dịch vụ tên miền Azure AD.</span><span class="sxs-lookup"><span data-stu-id="58c32-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="58c32-109">Bước này khiến các hàm hàm băm chứng danh bắt buộc đối với dịch vụ tên miền Azure AD sẽ được tạo ra.</span><span class="sxs-lookup"><span data-stu-id="58c32-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="58c32-110">Nếu tài khoản người dùng bị ảnh hưởng được đồng bộ từ một thư mục tại chỗ, hãy xác minh rằng bản phát hành được đề xuất của Azure AD Connect đã được cấu hình để thực hiện đồng bộ hóa đầy đủ.</span><span class="sxs-lookup"><span data-stu-id="58c32-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="58c32-111">Nếu sự cố vẫn tiếp diễn sau khi xác nhận bước 4, thực hiện các lệnh sau đây từ máy tính đồng bộ của bạn:</span><span class="sxs-lookup"><span data-stu-id="58c32-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="58c32-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="58c32-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>