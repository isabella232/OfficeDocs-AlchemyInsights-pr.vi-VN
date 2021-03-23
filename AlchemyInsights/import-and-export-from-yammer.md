---
title: Nhập và xuất từ yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037253"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="207b2-102">Nhập và xuất từ yammer</span><span class="sxs-lookup"><span data-stu-id="207b2-102">Import and export from Yammer</span></span>

<span data-ttu-id="207b2-103">**Xuất**</span><span class="sxs-lookup"><span data-stu-id="207b2-103">**Import**</span></span>

<span data-ttu-id="207b2-104">Các tùy chọn nhập người dùng khác nhau tùy thuộc vào việc mạng yammer của bạn nằm trong [chế độ bản địa cho Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)hay không.</span><span class="sxs-lookup"><span data-stu-id="207b2-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="207b2-105">**Chế độ không phải là bản địa**: người dùng có thể được nhập vào các nhóm bằng cách dùng [Thêm từ sổ địa chỉ](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (giới hạn đối với người dùng 100) trong thiết đặt nhóm hoặc vào mạng bằng cách dùng [Cập nhật hàng loạt](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) trong quản trị mạng.</span><span class="sxs-lookup"><span data-stu-id="207b2-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="207b2-106">**Chế độ bản địa**: thành viên nhóm và các hoạt động thành viên mạng phải được thực hiện từ [cổng thông tin quản trị Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [cổng thông tin Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)hoặc dùng tùy chọn Azure AD khác.</span><span class="sxs-lookup"><span data-stu-id="207b2-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="207b2-107">Các mạng trong chế độ bản địa không còn có quyền truy nhập vào bản cập nhật hàng loạt và các tính năng kế thừa khác.</span><span class="sxs-lookup"><span data-stu-id="207b2-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="207b2-108">Yammer không bao giờ được hỗ trợ nhập nội dung từ bên trong quản trị mạng ngay cả khi tính năng xuất dữ liệu được sử dụng trong một mạng khác.</span><span class="sxs-lookup"><span data-stu-id="207b2-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="207b2-109">Nội dung có thể được đăng lên bởi các giải pháp đối tác hoặc các API trong phần còn lại của yammer.</span><span class="sxs-lookup"><span data-stu-id="207b2-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="207b2-110">**Ngạch**</span><span class="sxs-lookup"><span data-stu-id="207b2-110">**Export**</span></span>

<span data-ttu-id="207b2-111">[Xuất dữ liệu mạng trong quản trị mạng](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) cho phép xuất nội dung từ mạng yammer, bao gồm các thư và tệp.</span><span class="sxs-lookup"><span data-stu-id="207b2-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="207b2-112">Tệp đính kèm có thể rất lớn và sẽ gây ra xuất khẩu để có thời gian đáng kể để hoàn thành.</span><span class="sxs-lookup"><span data-stu-id="207b2-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="207b2-113">Chúng tôi khuyên bạn nên xuất các mạng hiện hoạt bằng cách dùng [API xuất dữ liệu](https://developer.yammer.com/docs/data-export-api) trong chunks theo ngày hoặc tuần.</span><span class="sxs-lookup"><span data-stu-id="207b2-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="207b2-114">Hỗ trợ của Microsoft sẽ không cung cấp các tập lệnh tùy chỉnh cho mục đích này.</span><span class="sxs-lookup"><span data-stu-id="207b2-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="207b2-115">Xuất một [Gdpr](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) riêng biệt tồn tại để xuất nội dung cho một người dùng cá nhân.</span><span class="sxs-lookup"><span data-stu-id="207b2-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>