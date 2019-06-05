---
title: Cấp phép SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716913"
---
# <a name="sharepoint-designer-connection-issues"></a>Vấn đề kết nối SharePoint Designer 

<p>Nếu SharePoint Designer gặp phải vấn đề kết nối với các trang web SharePoint, xin vui lòng thử các giải pháp phổ biến sau.</p> <p><strong>Bước 1:</strong> <strong>Xác minh SharePoint Designer là Cập Nhật&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Cập Nhật cho SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>Bước 2:</strong> <strong>Xóa các tập tin bộ đệm ẩn cục bộ</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Đóng SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">Trên máy tính địa phương, trình duyệt các thư mục sau đây để loại bỏ các tập tin lưu trữ.&nbsp;</li> <li style="font-weight: 400;">Click vào <strong>bắt đầu -&gt; chạy</strong> và xóa tất cả các tệp tìm thấy dưới mỗi của các bên dưới vị trí.&nbsp;<br /><br />%AppData%\Microsoft\Web server Extensions\Cache<br />%AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Mở SharePoint Designer 2013 và nhập vào tài khoản một lần nữa để xem nếu nó hoạt động.</li> </ol> <p><strong>Bước 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Sử xác thực hiện đại cho Office 2013 trên cửa sổ thiết bị</strong></a>&nbsp;</p> <p><strong>Bước 4:</strong> <strong>Quản trị viên sẽ cần phải cho phép tuỳ chỉnh Script cho phép kết nối SharePoint Designer</strong>.</p> <p>Bước chi tiết, ví dụ và cân nhắc xem <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">cho phép hoặc ngăn chặn các tuỳ chỉnh script</a>.&nbsp;</p>


