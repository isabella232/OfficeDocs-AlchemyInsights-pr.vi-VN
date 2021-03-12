---
title: Sử dụng PowerShell để chia sẻ chính sách và mối quan hệ tổ chức
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709488"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Sử dụng PowerShell để chia sẻ chính sách và mối quan hệ tổ chức


Đối với các mối quan hệ tổ chức, vui lòng xem lại thông tin chi tiết về cú pháp và tham số cho: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-organizationmối](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship)quan hệ, [Set-organizationmối](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  quan hệ và  [loại bỏ](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Để tạo chính sách chia sẻ sử dụng [mới-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Để  [áp dụng chính sách chia sẻ cho một hộp thư hoặc người dùng](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  mà bạn cần sử dụng kết hợp  [hộp thư đặt](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) và [nhận hộp thư](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) với chính sách mới được tạo. Để  [sửa đổi, tắt hoặc loại bỏ chính sách chia sẻ,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  bạn cần sử dụng  [thiết đặt](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) chính sách và [loại bỏ](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Để biết đầy đủ về chủ đề này, vui lòng đọc:**

[Chia sẻ trong Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)