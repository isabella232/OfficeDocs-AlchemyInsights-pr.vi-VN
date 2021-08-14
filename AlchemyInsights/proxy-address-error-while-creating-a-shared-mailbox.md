---
title: Lỗi địa chỉ proxy trong khi tạo hộp thư chung
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062930"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Lỗi địa chỉ proxy trong khi tạo hộp thư hoặc đối tượng hỗ trợ email khác

Nếu bạn đã tìm cách tạo một đối tượng cho phép email (hộp thư, hộp thư chung, v.v.) và nhận được lỗi "Địa chỉ proxy "SMTP:alias@domain.com" đã được sử dụng..." thì địa chỉ email bạn đã chọn đã được một đối tượng hỗ trợ email khác trong tổ chức của bạn sử dụng.
  
Bạn cần tìm người dùng, nhóm, hộp thư chung hoặc thư mục công cộng có địa chỉ email này và xóa đối tượng đó hoặc thay đổi địa chỉ email của đối tượng. Sau đó, bạn có thể tạo một đối tượng mới hỗ trợ email với địa chỉ email miễn phí. Sử dụng tính năng Tìm kiếm trên Trang chủ để tìm. Bạn cũng có thể sử dụng lệnh Exchange Online PowerShell sau đây để tìm kiếm:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Nếu bạn không muốn xóa địa chỉ email hiện có, hãy chọn một địa chỉ email mới cho đối tượng mới mà bạn đang tạo.
  