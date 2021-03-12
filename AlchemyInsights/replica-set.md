---
title: Tập hợp bản sao
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
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714589"
---
# <a name="replica-set"></a>Tập hợp bản sao

Tiếng a cũng được gọi là tên miền được quản lý. Nó thực sự là hai bộ điều khiển tên miền được chạy và duy trì bởi bộ phụ trợ. Hai hàm này bao gồm một hình DC chính và một bản sao. Sao lưu trong phần thêm (tên miền được quản lý) là một quy trình tự động do nền tảng Azure quản lý. Trong trường hợp có sự cố với tên miền được quản lý của bạn, Azure hỗ trợ có thể hỗ trợ bạn trong việc khôi phục từ bản sao lưu.

Bạn tạo mỗi bản sao trong một mạng ảo. Mỗi mạng ảo phải được peered đến mọi mạng ảo khác mà lưu trữ tập hợp bản sao của tên miền được quản lý. Cấu hình này tạo một topo mạng lưới hỗ trợ sao chép thư mục. Mạng ảo có thể hỗ trợ nhiều bộ bản sao, được cung cấp cho mỗi tập hợp bản sao nằm trong một mạng con khác.

Để biết thêm chi tiết về bộ bản sao, hãy xem [bộ khái niệm bản sao](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
