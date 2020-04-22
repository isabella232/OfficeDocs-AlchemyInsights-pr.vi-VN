---
title: Vị trí dữ liệu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655304"
---
# <a name="data-location"></a><span data-ttu-id="56e6a-102">Vị trí dữ liệu</span><span class="sxs-lookup"><span data-stu-id="56e6a-102">Data location</span></span>

<span data-ttu-id="56e6a-103">Bạn có thể xem vị trí của đối tượng thuê của bạn trong Trung tâm quản trị hoặc bằng cách kết nối với Exchange Online qua PowerShell.</span><span class="sxs-lookup"><span data-stu-id="56e6a-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="56e6a-104">**Trung tâm quản trị:**</span><span class="sxs-lookup"><span data-stu-id="56e6a-104">**Admin center:**</span></span>
1. <span data-ttu-id="56e6a-105">Đăng nhập vào [Trung tâm quản trị](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="56e6a-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="56e6a-106">Chọn**cấu hình tổ chức** **cài đặt** > .</span><span class="sxs-lookup"><span data-stu-id="56e6a-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="56e6a-107">Trong **vị trí dữ liệu**, chọn **xem chi tiết**.</span><span class="sxs-lookup"><span data-stu-id="56e6a-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="56e6a-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="56e6a-108">**PowerShell:**</span></span>
1. <span data-ttu-id="56e6a-109">Kết nối với Exchange Online bằng cách sử dụng Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="56e6a-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="56e6a-110">Thực hiện lệnh [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) để hiển thị danh sách các thuộc tính của người thuê.</span><span class="sxs-lookup"><span data-stu-id="56e6a-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="56e6a-111">Xem thuộc tính OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="56e6a-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="56e6a-112">Khi bạn có vị trí dữ liệu cho EXO và SPO, bạn có thể xác định vị trí dữ liệu cho các dịch vụ khác mà bạn có thể sử dụng từ [nơi dữ liệu của bạn nằm ở đâu](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="56e6a-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>