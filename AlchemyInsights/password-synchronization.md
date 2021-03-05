---
title: Đồng bộ hoá mật khẩu
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
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483089"
---
# <a name="password-synchronization"></a><span data-ttu-id="d427f-102">Đồng bộ hoá mật khẩu</span><span class="sxs-lookup"><span data-stu-id="d427f-102">Password synchronization</span></span>

<span data-ttu-id="d427f-103">**Đồng bộ hóa hash mật khẩu không hoạt động ở tất cả**</span><span class="sxs-lookup"><span data-stu-id="d427f-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="d427f-104">Một số khách hàng thường gặp sự cố khi đồng bộ hóa hash mật khẩu không hoạt động là:</span><span class="sxs-lookup"><span data-stu-id="d427f-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="d427f-105">Tài khoản Active Directory được sử dụng bởi Azure AD Connect để liên lạc với Active Directory tại chỗ không được cấp cho các **thay đổi thư mục** nhân bản và nhân rộng **thay đổi tất cả** các quyền, vốn cần thiết cho việc đồng bộ hóa mật khẩu-bạn cần phải khắc phục sự cố này bằng cách cấp các quyền đối với tài khoản Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d427f-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="d427f-106">Đồng bộ hóa hash mật khẩu bị vô hiệu hóa sau khi người quản trị thay đổi phương pháp Sign-In người dùng từ việc **đồng bộ hóa mật khẩu** đến một tùy chọn khác chẳng hạn như **liên kết với AD FS** trong trình hướng dẫn kết nối Azure AD-bạn có thể khắc phục điều này bằng cách bật lại tính năng **đồng bộ hóa hash mật khẩu** trong trình hướng dẫn Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d427f-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="d427f-107">Vấn đề kết nối với Active Directory tại chỗ.</span><span class="sxs-lookup"><span data-stu-id="d427f-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="d427f-108">Ví dụ: một số bộ điều khiển tên miền không được truy nhập bằng Azure AD Connect, hoặc các [cổng bắt buộc](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) bị tường lửa-bạn cần khắc phục điều này bằng cách đảm bảo rằng kết nối giữa máy chủ Azure AD Connect và Active Directory tại chỗ hoạt động chính xác.</span><span class="sxs-lookup"><span data-stu-id="d427f-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="d427f-109">Máy chủ Azure AD Connect hiện đang ở chế độ tổ chức, vốn sẽ kết quả là máy chủ không thể sử dụng để khắc phục sự cố này, hãy làm theo các bước được mô tả trong phần [khắc phục sự cố mật khẩu đồng bộ hóa với AZURE AD Connect Sync-không có mật khẩu được đồng bộ](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="d427f-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="d427f-110">**Đồng bộ hóa hash mật khẩu không hoạt động đối với một số người dùng của tôi**</span><span class="sxs-lookup"><span data-stu-id="d427f-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="d427f-111">Nếu bạn nhận thấy rằng băm mật khẩu không đồng bộ với người dùng, hãy sử dụng tác vụ **khắc phục sự cố** trong Azure AD Connect để điều tra và giải quyết sự cố.</span><span class="sxs-lookup"><span data-stu-id="d427f-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="d427f-112">Thực hiện các tác vụ sau đây:</span><span class="sxs-lookup"><span data-stu-id="d427f-112">Perform the following tasks:</span></span>

    <span data-ttu-id="d427f-113">một.</span><span class="sxs-lookup"><span data-stu-id="d427f-113">a.</span></span> [<span data-ttu-id="d427f-114">Chạy nhiệm vụ khắc phục sự cố trong trình hướng dẫn</span><span class="sxs-lookup"><span data-stu-id="d427f-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="d427f-115">b.</span><span class="sxs-lookup"><span data-stu-id="d427f-115">b.</span></span> [<span data-ttu-id="d427f-116">Sử dụng lệnh ghép ngắn khắc phục sự cố để điều tra sự cố đồng bộ hóa mật khẩu của Hash cho một dùng cụ thể</span><span class="sxs-lookup"><span data-stu-id="d427f-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="d427f-117">Đối tượng người dùng Active Directory tại chỗ được kích hoạt cho **người dùng phải thay đổi mật khẩu tại tùy chọn đăng nhập tiếp theo** .</span><span class="sxs-lookup"><span data-stu-id="d427f-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="d427f-118">Khi tùy chọn này được bật, người dùng được gán một mật khẩu tạm thời và sẽ được nhắc thay đổi mật khẩu trong đăng nhập tiếp theo.</span><span class="sxs-lookup"><span data-stu-id="d427f-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="d427f-119">Azure AD Connect sẽ không đồng bộ hóa mật khẩu tạm thời cho Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d427f-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="d427f-120">Để giải quyết sự cố trên đây, hãy thực hiện một trong các tác vụ sau:</span><span class="sxs-lookup"><span data-stu-id="d427f-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="d427f-121">Yêu cầu người dùng đăng nhập vào ứng dụng tại cơ sở (ví dụ, Windows Desktop) và thay đổi mật khẩu.</span><span class="sxs-lookup"><span data-stu-id="d427f-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="d427f-122">Mật khẩu mới sẽ được đồng bộ hóa với Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d427f-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="d427f-123">Có người quản trị Cập nhật mật khẩu của người dùng mà không cho phép **người dùng tùy chọn phải thay đổi mật khẩu tại mục đăng nhập tiếp theo** và chia sẻ mật khẩu mới với người dùng.</span><span class="sxs-lookup"><span data-stu-id="d427f-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="d427f-124">Đối tượng người dùng Active Directory tại cơ sở **không được cấu hình chính xác** cho đồng bộ hóa đối tượng hoặc đồng bộ hóa mật khẩu.</span><span class="sxs-lookup"><span data-stu-id="d427f-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="d427f-125">Để khắc phục sự cố này, hãy làm theo các bước được mô tả trong [đồng bộ hóa hash mật khẩu khắc phục sự cố với AZURE AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="d427f-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







