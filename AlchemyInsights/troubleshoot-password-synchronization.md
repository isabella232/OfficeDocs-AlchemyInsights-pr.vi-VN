---
title: Khắc phục sự cố đồng bộ hoá mật khẩu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28320866"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="154f2-102">Khắc phục sự cố đồng bộ hoá mật khẩu</span><span class="sxs-lookup"><span data-stu-id="154f2-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="154f2-103">Để khắc phục sự cố mà không có mật khẩu là đồng bộ hóa với phiên bản Azure quảng cáo kết nối 1.1.614.0 hoặc sau này:</span><span class="sxs-lookup"><span data-stu-id="154f2-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="154f2-104">Mở một phiên Windows PowerShell mới trên máy chủ Azure quảng cáo kết nối của bạn với tùy chọn **Run as Administrator** .</span><span class="sxs-lookup"><span data-stu-id="154f2-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="154f2-105">Chạy **thiết lập-ExecutionPolicy thành RemoteSigned** hoặc **thiết lập-ExecutionPolicy không giới hạn**.</span><span class="sxs-lookup"><span data-stu-id="154f2-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="154f2-106">Khởi động thuật sĩ Azure quảng cáo kết nối.</span><span class="sxs-lookup"><span data-stu-id="154f2-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="154f2-107">Điều hướng đến các \*\* nhiệm vụ bổ sung \*\* trang, chọn \*\* khắc phục \*\*, và nhấp vào **tiếp theo**.</span><span class="sxs-lookup"><span data-stu-id="154f2-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="154f2-108">Trên trang giải đáp thắc mắc, hãy nhấp vào trình đơn **khởi động để bắt đầu việc khắc phục sự cố** trong PowerShell.</span><span class="sxs-lookup"><span data-stu-id="154f2-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="154f2-109">Trong menu chính, chọn **Khắc phục sự cố đồng bộ hoá mật khẩu**.</span><span class="sxs-lookup"><span data-stu-id="154f2-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="154f2-110">Trong trình đơn phụ, chọn **đồng bộ hoá mật khẩu không hoạt động ở tất cả**.</span><span class="sxs-lookup"><span data-stu-id="154f2-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="154f2-111">**Hiểu các kết quả của công tác khắc phục sự cố**</span><span class="sxs-lookup"><span data-stu-id="154f2-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="154f2-112">Nhiệm vụ khắc phục sự cố thực hiện kiểm tra sau đây:</span><span class="sxs-lookup"><span data-stu-id="154f2-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="154f2-113">Xác nhận rằng tính năng đồng bộ hoá mật khẩu được kích hoạt cho người thuê nhà Azure quảng cáo của bạn.</span><span class="sxs-lookup"><span data-stu-id="154f2-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="154f2-114">Xác nhận rằng Azure quảng cáo kết nối máy chủ không phải là trong dàn chế độ.</span><span class="sxs-lookup"><span data-stu-id="154f2-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="154f2-115">Đối với mỗi chỗ hiện kết nối hoạt động thư mục (mà tương ứng với một cụm nhánh Active Directory hiện có):</span><span class="sxs-lookup"><span data-stu-id="154f2-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="154f2-116">Xác nhận rằng tính năng đồng bộ hoá mật khẩu được kích hoạt.</span><span class="sxs-lookup"><span data-stu-id="154f2-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="154f2-117">Đang tìm kiếm sự kiện nhịp tim đồng bộ hoá mật khẩu trong Nhật ký sự kiện ứng dụng của Windows.</span><span class="sxs-lookup"><span data-stu-id="154f2-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="154f2-118">Đối với mỗi hoạt động thư mục tên miền dưới đầu nối Active Directory tại chỗ:</span><span class="sxs-lookup"><span data-stu-id="154f2-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="154f2-119">Xác nhận rằng tên miền là thể truy cập từ Azure quảng cáo kết nối máy chủ.</span><span class="sxs-lookup"><span data-stu-id="154f2-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="154f2-120">Xác nhận rằng các tài khoản Dịch vụ miền Active Directory (AD DS) được sử dụng bởi kết nối Active Directory tại chỗ có đúng tên người dùng, mật khẩu, và các quyền cần thiết để đồng bộ hoá mật khẩu.</span><span class="sxs-lookup"><span data-stu-id="154f2-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="154f2-121">Để thêm trợ giúp khắc phục sự cố đồng bộ mật khẩu, hãy xem [đồng bộ hoá mật khẩu khắc phục với Azure quảng cáo kết nối đồng bộ](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="154f2-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

