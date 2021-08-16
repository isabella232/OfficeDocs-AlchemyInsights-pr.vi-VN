---
title: Sử dụng PowerShell để chia sẻ chính sách và mối quan hệ Tổ chức
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 48df03b1397b0e924aa878cea3d1cac07ca862c3636c1273d10f4841a03fddcf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998518"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Sử dụng PowerShell để chia sẻ chính sách và mối quan hệ Tổ chức


Đối với mối quan hệ Tổ chức, vui lòng xem lại thông tin cú pháp và tham số chi tiết cho : [Get-FederationInformationation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Để tạo chính sách chia [sẻ, hãy sử dụng New-SharingPolicy.](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy) Để  [áp dụng chính sách chia sẻ](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  cho hộp thư hoặc người dùng, bạn cần sử dụng kết hợp cả  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) và [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) với chính sách mới được tạo. Để [sửa đổi, hãy tắt hoặc loại bỏ chính sách chia](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) sẻ, bạn cần sử dụng [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) [và Remove-SharingPolicy.](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)

**Để hiểu đầy đủ về chủ đề này, vui lòng đọc:**

[Chia sẻ trong Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)