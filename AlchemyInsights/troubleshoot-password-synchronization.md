---
title: Khắc phục sự cố đồng bộ hóa mật khẩu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732532"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="753c9-102">Khắc phục sự cố đồng bộ hóa mật khẩu</span><span class="sxs-lookup"><span data-stu-id="753c9-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="753c9-103">Để khắc phục sự cố mà không có mật khẩu được đồng bộ hoá với Azure AD kết nối phiên bản 1.1.614.0 hoặc mới hơn:</span><span class="sxs-lookup"><span data-stu-id="753c9-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="753c9-104">Mở phiên Windows PowerShell mới trên máy chủ Azure AD kết nối với tùy chọn **chạy như quản trị viên** .</span><span class="sxs-lookup"><span data-stu-id="753c9-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="753c9-105">Chạy **thiết lập ExecutionPolicy RemoteSigned** hoặc **thiết lập ExecutionPolicy không hạn**chế.</span><span class="sxs-lookup"><span data-stu-id="753c9-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="753c9-106">Khởi động thuật sĩ Azure AD kết nối.</span><span class="sxs-lookup"><span data-stu-id="753c9-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="753c9-107">Điều hướng đến trang **tác vụ bổ sung** , chọn **khắc phục sự cố**và nhấp vào **tiếp theo**.</span><span class="sxs-lookup"><span data-stu-id="753c9-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="753c9-108">Trang khắc phục sự cố, bấm **khởi động để khởi động trình đơn khắc phục sự cố** trong PowerShell.</span><span class="sxs-lookup"><span data-stu-id="753c9-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="753c9-109">Trong menu chính, chọn **khắc phục sự cố đồng bộ hóa mật khẩu**.</span><span class="sxs-lookup"><span data-stu-id="753c9-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="753c9-110">Trong menu phụ, chọn **đồng bộ hóa mật khẩu không hoạt động ở tất cả**.</span><span class="sxs-lookup"><span data-stu-id="753c9-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="753c9-111">**Hiểu kết quả của tác vụ khắc phục sự cố**</span><span class="sxs-lookup"><span data-stu-id="753c9-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="753c9-112">Việc khắc phục sự cố thực hiện kiểm tra sau:</span><span class="sxs-lookup"><span data-stu-id="753c9-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="753c9-113">Xác thực rằng tính năng đồng bộ hóa mật khẩu được kích hoạt cho thuê Azure AD.</span><span class="sxs-lookup"><span data-stu-id="753c9-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="753c9-114">Xác nhận rằng Azure AD kết nối máy chủ không ở chế độ dàn.</span><span class="sxs-lookup"><span data-stu-id="753c9-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="753c9-115">Đối với mỗi kết nối Active Directory tại chỗ hiện tại (tương ứng với một nhóm Active Directory hiện có):</span><span class="sxs-lookup"><span data-stu-id="753c9-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="753c9-116">Xác nhận rằng tính năng đồng bộ hóa mật khẩu được kích hoạt.</span><span class="sxs-lookup"><span data-stu-id="753c9-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="753c9-117">Tìm kiếm đồng bộ hóa mật khẩu Heartbeat sự kiện trong Nhật ký sự kiện ứng dụng Windows.</span><span class="sxs-lookup"><span data-stu-id="753c9-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="753c9-118">Đối với mỗi miền Active Directory trong kết nối Active Directory tại chỗ:</span><span class="sxs-lookup"><span data-stu-id="753c9-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="753c9-119">Xác nhận tên miền có thể truy cập từ máy chủ Azure AD kết nối.</span><span class="sxs-lookup"><span data-stu-id="753c9-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="753c9-120">Xác thực rằng tài khoản Dịch vụ miền Active Directory (AD DS) sử dụng kết nối Active Directory tại chỗ có đúng tên người dùng, mật khẩu và quyền cần thiết để đồng bộ hóa mật khẩu.</span><span class="sxs-lookup"><span data-stu-id="753c9-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="753c9-121">Để được trợ giúp thêm khắc phục sự cố đồng bộ hóa mật khẩu, xem [khắc phục sự cố đồng bộ hóa mật khẩu với AZURE AD kết nối đồng](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)</span><span class="sxs-lookup"><span data-stu-id="753c9-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  