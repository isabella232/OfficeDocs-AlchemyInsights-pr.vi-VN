---
title: Cấu hình điểm kết nối dịch vụ (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037294"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="4c40c-102">Cấu hình điểm kết nối dịch vụ (SCP)</span><span class="sxs-lookup"><span data-stu-id="4c40c-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="4c40c-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="4c40c-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="4c40c-104">**Lý do**: không thể đọc được đối tượng SCP và nhận được thông tin về người thuê Azure AD</span><span class="sxs-lookup"><span data-stu-id="4c40c-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="4c40c-105">**Giải** Pháp: tham khảo phần [cấu hình điểm kết nối dịch vụ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="4c40c-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="4c40c-106">**Kế hoạch hành động**</span><span class="sxs-lookup"><span data-stu-id="4c40c-106">**Action plan**</span></span>

- <span data-ttu-id="4c40c-107">Kiểm tra xem thiết bị đã nhận được GPO để xác thực được kiểm soát hay không.</span><span class="sxs-lookup"><span data-stu-id="4c40c-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="4c40c-108">Đảm bảo rằng GPO đã tạo khóa đăng ký.</span><span class="sxs-lookup"><span data-stu-id="4c40c-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="4c40c-109">Đảm bảo rằng bạn có 2 phím được tạo bằng ID thư mục và tên miền onmicrosoft của bạn.</span><span class="sxs-lookup"><span data-stu-id="4c40c-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="4c40c-110">**Cấu hình thiết đặt sổ đăng ký phía máy khách cho SCP**</span><span class="sxs-lookup"><span data-stu-id="4c40c-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="4c40c-111">Dùng ví dụ sau đây để tạo một đối tượng chính sách Nhóm (GPO) để triển khai thiết đặt sổ đăng ký cấu hình một mục nhập SCP trong sổ đăng ký thiết bị của bạn.</span><span class="sxs-lookup"><span data-stu-id="4c40c-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="4c40c-112">Mở bảng điều khiển quản lý chính sách nhóm và tạo một GPO mới trong tên miền của bạn.</span><span class="sxs-lookup"><span data-stu-id="4c40c-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="4c40c-113">Cung cấp một tên mới được tạo là GPO của bạn (ví dụ: ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="4c40c-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="4c40c-114">Sửa GPO và định vị đường dẫn sau đây: **cấu hình máy tính > tùy chọn > thiết đặt Windows > sổ đăng ký**.</span><span class="sxs-lookup"><span data-stu-id="4c40c-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="4c40c-115">Bấm chuột phải vào **sổ đăng ký** và chọn **> mục đăng ký mới**.</span><span class="sxs-lookup"><span data-stu-id="4c40c-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="4c40c-116">Trên tab **chung** , hãy cấu hình các mục sau:</span><span class="sxs-lookup"><span data-stu-id="4c40c-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="4c40c-117">**Hành động**: Cập Nhật</span><span class="sxs-lookup"><span data-stu-id="4c40c-117">**Action**: Update</span></span>
    
- <span data-ttu-id="4c40c-118">**Hive**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="4c40c-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="4c40c-119">**Đường dẫn chính**: Software\microsoft\windows\currentversion\cdj\aad</span><span class="sxs-lookup"><span data-stu-id="4c40c-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="4c40c-120">**Giá trị tên**: tenantid</span><span class="sxs-lookup"><span data-stu-id="4c40c-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="4c40c-121">**Loại giá trị**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="4c40c-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="4c40c-122">**Dữ liệu giá trị**: GUID hoặc ID thư mục của mẫu Azure AD của bạn (giá trị này có thể được tìm thấy trong **Azure Portal > azure Active Directory > thuộc tính > ID thư mục**)</span><span class="sxs-lookup"><span data-stu-id="4c40c-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="4c40c-123">Bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="4c40c-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="4c40c-124">Bấm chuột phải vào **sổ đăng ký** và chọn **> mục đăng ký mới**.</span><span class="sxs-lookup"><span data-stu-id="4c40c-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="4c40c-125">Trên tab **chung** , hãy cấu hình các mục sau:</span><span class="sxs-lookup"><span data-stu-id="4c40c-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="4c40c-126">**Hành động**: Cập Nhật</span><span class="sxs-lookup"><span data-stu-id="4c40c-126">**Action**: Update</span></span>
    
- <span data-ttu-id="4c40c-127">**Hive**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="4c40c-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="4c40c-128">**Đường dẫn chính**: Software\microsoft\windows\currentversion\cdj\aad</span><span class="sxs-lookup"><span data-stu-id="4c40c-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="4c40c-129">**Giá trị tên**: tenantname</span><span class="sxs-lookup"><span data-stu-id="4c40c-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="4c40c-130">**Loại giá trị**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="4c40c-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="4c40c-131">**Dữ liệu giá trị**: tên miền đã xác nhận nếu bạn đang sử dụng môi trường liên kết chẳng hạn như AD FS.</span><span class="sxs-lookup"><span data-stu-id="4c40c-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="4c40c-132">Tên miền đã xác nhận của bạn hoặc tên miền onmicrosoft.com của bạn (ví dụ: contoso. onmicrosoft). com nếu bạn đang sử dụng môi trường được quản lý</span><span class="sxs-lookup"><span data-stu-id="4c40c-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="4c40c-133">Bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="4c40c-133">Click **OK**.</span></span>

7. <span data-ttu-id="4c40c-134">Đóng trình soạn thảo cho GPO mới được tạo.</span><span class="sxs-lookup"><span data-stu-id="4c40c-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="4c40c-135">Nối kết các máy tính có thể tham gia vào trình phát triển tên miền của bạn.</span><span class="sxs-lookup"><span data-stu-id="4c40c-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="4c40c-136">Để biết thêm thông tin, hãy xem kiểm soát xác thực của kết hợp kết nối [AZURE AD-AZURE AD | ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) Tài liệu Microsoft và  [khắc phục sự cố kết hợp Azure Active Directory đã tham gia thiết bị | ](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)Tài liệu Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4c40c-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









