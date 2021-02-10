---
title: Đồng bộ hóa hash mật khẩu cho dịch vụ miền
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
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177616"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="f2563-102">Đồng bộ hóa hash mật khẩu cho dịch vụ miền</span><span class="sxs-lookup"><span data-stu-id="f2563-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="f2563-103">**Nếu ví dụ Azure AD DS của bạn là nhắc bạn bật đồng bộ hóa hash mật khẩu**</span><span class="sxs-lookup"><span data-stu-id="f2563-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="f2563-104">Bạn gặp phải một tình huống mà bạn đang chạy môi trường hỗn hợp với người dùng đang đồng bộ hóa từ môi trường dịch vụ miền (AD DS) tại chỗ của Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f2563-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="f2563-105">Tình huống này gặp mặc dù bạn có đồng bộ hóa hash mật khẩu từ AD DS tại cơ sở với đối tượng thuê Azure AD của bạn.</span><span class="sxs-lookup"><span data-stu-id="f2563-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="f2563-106">**Bởi**</span><span class="sxs-lookup"><span data-stu-id="f2563-106">**Cause**</span></span>

<span data-ttu-id="f2563-107">Điều này xảy ra vì Azure AD kết nối theo mặc định không đồng bộ hóa công nghệ mới của Microsoft Manager (NTLM) và Kerberos mật khẩu hàm băm cần thiết cho Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="f2563-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="f2563-108">**Lỗi**</span><span class="sxs-lookup"><span data-stu-id="f2563-108">**Workaround**</span></span> 

<span data-ttu-id="f2563-109">Bạn sẽ cần phải cấu hình Azure AD Connect để đồng bộ hóa các hàm hàm băm mật khẩu được yêu cầu cho NTLM và Kerberos xác thực.</span><span class="sxs-lookup"><span data-stu-id="f2563-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="f2563-110">Sau khi Azure AD Connect được cấu hình, một tài khoản tại chỗ hoặc tạo sự kiện thay đổi mật khẩu cũng đồng bộ hóa mật khẩu kế thừa hàm băm thành Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f2563-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="f2563-111">Vui lòng xem mục [ở đây](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) để biết thêm thông tin về điều này và để được hướng dẫn về cách bật đồng bộ hóa mật khẩu trong AZURE AD DS Hybrid môi trường.</span><span class="sxs-lookup"><span data-stu-id="f2563-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>