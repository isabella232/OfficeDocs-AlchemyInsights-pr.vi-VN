---
title: Writeback thiết bị
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256974"
---
# <a name="device-writeback"></a><span data-ttu-id="860b2-102">Writeback thiết bị</span><span class="sxs-lookup"><span data-stu-id="860b2-102">Device Writeback</span></span>

<span data-ttu-id="860b2-103">Writeback của thiết bị được dùng trong các kịch bản sau đây:</span><span class="sxs-lookup"><span data-stu-id="860b2-103">Device Writeback is used in the following scenarios:</span></span>

- <span data-ttu-id="860b2-104">[Cho phép Windows Hello for Business sử dụng triển khai tin cậy chứng chỉ hỗn](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration) hợp</span><span class="sxs-lookup"><span data-stu-id="860b2-104">Enable [Windows Hello for Business using hybrid certificate trust deployment](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span></span>
- <span data-ttu-id="860b2-105">Cho phép truy nhập có điều kiện dựa trên các thiết bị đến các ứng dụng bảo vệ (2012 R2 hoặc cao hơn) (dựa vào tín thác của bên)</span><span class="sxs-lookup"><span data-stu-id="860b2-105">Enable Conditional Access based on devices to ADFS (2012 R2 or higher) protected applications (relying party trusts)</span></span>

    > [!NOTE]
    > <span data-ttu-id="860b2-106">Đăng ký vào Azure AD Premium được yêu cầu cho writeback thiết bị.</span><span class="sxs-lookup"><span data-stu-id="860b2-106">A subscription to Azure AD Premium is required for device writeback.</span></span>

<span data-ttu-id="860b2-107">Điều này cung cấp bảo mật bổ sung và đảm bảo rằng quyền truy nhập vào các ứng dụng chỉ được cấp cho các thiết bị tin cậy.</span><span class="sxs-lookup"><span data-stu-id="860b2-107">This provides additional security and assurance that access to applications is granted only to trusted devices.</span></span> <span data-ttu-id="860b2-108">Để biết thêm thông tin về truy nhập có điều kiện, hãy xem [quản lý rủi ro với quyền truy nhập có điều kiện](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) và [thiết lập quyền truy nhập có điều kiện tại chỗ bằng cách đăng ký thiết bị Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview).</span><span class="sxs-lookup"><span data-stu-id="860b2-108">For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and [Setting up On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span></span>

<span data-ttu-id="860b2-109">Để biết thêm thông tin về bật tính năng thiết bị cho các thiết bị, hãy xem bật tính năng lưu [thiết bị](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span><span class="sxs-lookup"><span data-stu-id="860b2-109">For more information on Enabling Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span></span>
