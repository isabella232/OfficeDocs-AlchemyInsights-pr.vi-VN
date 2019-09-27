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
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207283"
---
# <a name="data-location"></a><span data-ttu-id="389db-102">Vị trí dữ liệu</span><span class="sxs-lookup"><span data-stu-id="389db-102">Data location</span></span>

<span data-ttu-id="389db-103">Bạn có thể xem vị trí của người thuê văn phòng 365 trong Trung tâm quản trị hoặc bằng cách kết nối với Exchange Online qua PowerShell.</span><span class="sxs-lookup"><span data-stu-id="389db-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="389db-104">**Trung tâm quản trị:**</span><span class="sxs-lookup"><span data-stu-id="389db-104">**Admin center:**</span></span>
1. <span data-ttu-id="389db-105">Đăng nhập vào [Trung tâm quản trị](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="389db-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="389db-106">Chọn**cấu hình tổ chức** **cài đặt** > .</span><span class="sxs-lookup"><span data-stu-id="389db-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="389db-107">Trong **vị trí dữ liệu**, chọn **xem chi tiết**.</span><span class="sxs-lookup"><span data-stu-id="389db-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="389db-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="389db-108">**PowerShell:**</span></span>
1. <span data-ttu-id="389db-109">Kết nối với Exchange Online bằng cách sử dụng Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="389db-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="389db-110">Thực hiện lệnh [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) để hiển thị danh sách các thuộc tính của người thuê.</span><span class="sxs-lookup"><span data-stu-id="389db-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="389db-111">Xem thuộc tính OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="389db-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="389db-112">Khi bạn có vị trí dữ liệu cho EXO và SPO, bạn có thể xác định vị trí dữ liệu cho các dịch vụ khác mà bạn có thể sử dụng từ [nơi dữ liệu của bạn nằm ở đâu](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="389db-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>