---
title: Khắc phục sự cố truy cập từ chối các thư
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: ee154a60d80472639371d44faef464eea8734dc9
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716668"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Khắc phục sự cố truy cập từ chối các thư trong Trung tâm quản trị Sharepoint/OneDrive

<p><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Nếu bạn nhận được quyền truy cập bị từ chối thư khi cố gắng để duyệt đến một trung tâm quản trị Sharepoint/OneDrive, hãy chắc chắn rằng bạn <a href="https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One">gán một giấy phép cho người dùng </a>. Nếu người dùng có một giấy phép, bạn cũng nên chắc chắn họ là <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/about-admin-roles?view=o365-worldwide">được gán vai trò người quản trị</a> mà có thể truy cập Trung tâm quản trị.</span></p>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Vấn đề này cũng có thể xảy ra khi người dùng xóa và tạo lại với cùng tên người dùng chính (UPN). Tài khoản mới được tạo ra bằng cách sử dụng một giá trị PUID (hộ chiếu duy nhất ID) khác nhau. Khi người dùng cố gắng truy cập vào một bộ sưu tập trang web hoặc OneDrive của họ, người dùng có một PUID không chính xác. Một kịch bản thứ hai liên quan đến việc đồng bộ hóa thư mục với một đơn vị tổ chức hoạt động Directory (OU). Nếu người dùng đã đăng nhập vào SharePoint, và sau đó được chuyển đến một OU khác nhau và resynced với SharePoint, họ có thể gặp vấn đề này.</span></span></p>  <ul style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;" type="disc">  <li style="line-height: normal; ; font-size: 11pt; font-style: normal; font-weight: 400;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Để giải quyết vấn đề này, bạn nên khôi phục lại UPN ban đầu với các bước trong bài viết, <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">khôi phục người dùng trong Office 365</a>.</span></span></li>  </ul>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><strong><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;">Lưu ý:</span></span></strong><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-fareast-font-family: 'Times New Roman'; mso-bidi-font-family: 'Times New Roman';"><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><em style="mso-bidi-font-style: normal;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">&nbsp;</span></em><em><span style="font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;font-style: normal; mso-bidi-font-style: italic;">nếu một trung tâm OneDrive hoặc SharePoint Admin là không có sẵn cho nhiều người dùng trước đó đã truy cập, có thể có một vấn đề dịch vụ tạm thời.&nbsp; </span></span></em> <em><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;"> <a href="https://portal.office.com/adminportal/home#/servicehealth" target="_blank" rel="noopener"><span style="font-style: normal; mso-bidi-font-style: italic;">Kiểm tra bảng điều khiển dịch vụ y tế</span></a>.</span></em></span></span></p>


