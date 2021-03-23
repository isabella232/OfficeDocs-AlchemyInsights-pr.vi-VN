---
title: Khắc phục sự cố đăng nhập một lần cho Azure AD đã gia nhập thiết bị
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037338"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="cd604-102">Khắc phục sự cố đăng nhập một lần cho Azure AD đã gia nhập thiết bị</span><span class="sxs-lookup"><span data-stu-id="cd604-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="cd604-103">Nếu bạn có môi trường Active Directory (AD) tại cơ sở và bạn muốn gia nhập vào các máy tính của bạn tham gia vào Azure AD, bạn có thể thực hiện điều này bằng cách kết hợp kết hợp Azure AD join.</span><span class="sxs-lookup"><span data-stu-id="cd604-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="cd604-104">[Cách thức: lập kế hoạch cho việc thực hiện kết hợp Azure Active Directory của bạn](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) sẽ cung cấp cho bạn các bước liên quan để thực hiện kết hợp Azure AD join trong môi trường của bạn.</span><span class="sxs-lookup"><span data-stu-id="cd604-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="cd604-105">Để biết thêm thông tin, hãy xem mục [đặt cấu hình AZURE AD đã gia nhập thiết bị cho các Single-Sign tại cơ sở khi sử dụng Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span><span class="sxs-lookup"><span data-stu-id="cd604-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="cd604-106">**Các sự cố mã thông báo làm mới (PRT) chính**</span><span class="sxs-lookup"><span data-stu-id="cd604-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="cd604-107">Một mã thông báo làm mới chính (PRT) là một artifact chính của xác thực Azure AD trên Windows 10, Windows Server 2016 và các thiết bị chạy sau, iOS và Android.</span><span class="sxs-lookup"><span data-stu-id="cd604-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="cd604-108">Đây là một mã thông báo web JSON (JWT) đặc biệt được phát hành cho môi giới mã thông báo đầu tiên của Microsoft để cho phép đăng nhập một lần (SSO) trên các ứng dụng được sử dụng trên các thiết bị này.</span><span class="sxs-lookup"><span data-stu-id="cd604-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="cd604-109">Để biết chi tiết về cách thức phát hành của PRT, được sử dụng và bảo vệ trên thiết bị chạy Windows 10, hãy xem mã thông báo [làm mới chính là gì?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="cd604-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="cd604-110">**WamDefaultSet: có và AzureADPrt: có**</span><span class="sxs-lookup"><span data-stu-id="cd604-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="cd604-111">Những trường này cho biết người dùng đã xác thực thành công để Azure AD khi đăng nhập vào thiết bị hay không.</span><span class="sxs-lookup"><span data-stu-id="cd604-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="cd604-112">Nếu các giá trị là **không có**, có thể là do:</span><span class="sxs-lookup"><span data-stu-id="cd604-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="cd604-113">Phím lưu trữ xấu trong TPM được liên kết với thiết bị sau khi đăng ký (kiểm tra kiểm tra phím trong khi đang chạy nâng cao)</span><span class="sxs-lookup"><span data-stu-id="cd604-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="cd604-114">ID đăng nhập thay thế</span><span class="sxs-lookup"><span data-stu-id="cd604-114">Alternate Login ID</span></span>
- <span data-ttu-id="cd604-115">Không tìm thấy proxy HTTP</span><span class="sxs-lookup"><span data-stu-id="cd604-115">HTTP Proxy not found</span></span>

<span data-ttu-id="cd604-116">Để khắc phục các thiết bị bằng cách dùng lệnh dsregcmd, hãy xem [trạng thái SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="cd604-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
