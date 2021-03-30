---
title: Single-Sign cho Azure Active Directory đã tham gia thiết bị
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405666"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="2c02c-102">Đăng nhập một lần cho Azure Active Directory đã tham gia thiết bị</span><span class="sxs-lookup"><span data-stu-id="2c02c-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="2c02c-103">Nếu bạn có môi trường Active Directory (AD) tại cơ sở và bạn muốn gia nhập vào các máy tính của bạn tham gia vào Azure AD, bạn có thể thực hiện điều này bằng cách kết hợp kết hợp Azure AD join.</span><span class="sxs-lookup"><span data-stu-id="2c02c-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="2c02c-104">[Cách thức: lập kế hoạch cho việc thực hiện kết hợp Azure Active Directory của bạn](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) sẽ cung cấp cho bạn các bước liên quan để thực hiện kết hợp Azure AD join trong môi trường của bạn.</span><span class="sxs-lookup"><span data-stu-id="2c02c-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="2c02c-105">Cấu hình Azure AD đã tham gia các thiết bị cho Single-Sign tại cơ sở khi sử dụng Windows Hello for Business</span><span class="sxs-lookup"><span data-stu-id="2c02c-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="2c02c-106">Các sự **cố mã thông báo làm mới (PRT) chính** Một mã thông báo làm mới chính (PRT) là một artifact chính của xác thực Azure AD trên Windows 10, Windows Server 2016 và các thiết bị chạy sau, iOS và Android.</span><span class="sxs-lookup"><span data-stu-id="2c02c-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="2c02c-107">Đây là một mã thông báo web JSON (JWT) đặc biệt được phát hành cho môi giới mã thông báo đầu tiên của Microsoft để cho phép đăng nhập một lần (SSO) trên các ứng dụng được sử dụng trên các thiết bị này.</span><span class="sxs-lookup"><span data-stu-id="2c02c-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="2c02c-108">[Trong mã bản làm mới chính là gì?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), chúng tôi sẽ cung cấp chi tiết về cách thức phát hành của PRT, được sử dụng và bảo vệ trên các thiết bị chạy Windows 10.</span><span class="sxs-lookup"><span data-stu-id="2c02c-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="2c02c-109">**Wamdefaultset: có và AzureADPrt: có** Những trường này cho biết người dùng đã xác thực thành công để Azure AD khi đăng nhập vào thiết bị hay không.</span><span class="sxs-lookup"><span data-stu-id="2c02c-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="2c02c-110">Nếu các giá trị là **không có**, thì có thể là do:</span><span class="sxs-lookup"><span data-stu-id="2c02c-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="2c02c-111">Phím lưu trữ xấu trong TPM được liên kết với thiết bị sau khi đăng ký (kiểm tra kiểm tra phím trong khi đang chạy nâng cao).</span><span class="sxs-lookup"><span data-stu-id="2c02c-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="2c02c-112">ID đăng nhập thay thế</span><span class="sxs-lookup"><span data-stu-id="2c02c-112">Alternate Login ID</span></span>
- <span data-ttu-id="2c02c-113">Không tìm thấy proxy HTTP</span><span class="sxs-lookup"><span data-stu-id="2c02c-113">HTTP Proxy not found</span></span>

<span data-ttu-id="2c02c-114">Khắc phục sự cố các thiết bị sử dụng lệnh dsregcmd- [SSO State](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="2c02c-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
