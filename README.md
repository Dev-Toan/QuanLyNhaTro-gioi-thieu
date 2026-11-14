<div align="center">

<img src="docs/assets/banner.svg" alt="Quản lý nhà trọ" width="100%" />

<br />

![Java](https://img.shields.io/badge/Java-21-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.5-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-16-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react&logoColor=black)
![Kotlin](https://img.shields.io/badge/Kotlin-Jetpack_Compose-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
<br />
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-7-DC382D?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Compose-2496ED?style=flat-square&logo=docker&logoColor=white)
![OpenAPI](https://img.shields.io/badge/OpenAPI-0.8.0-6BA539?style=flat-square&logo=openapiinitiative&logoColor=white)

<a href="mailto:toanit5.haui@gmail.com"><img src="https://img.shields.io/badge/Email-toanit5.haui%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
<a href="https://zalo.me/0773332973"><img src="https://img.shields.io/badge/Zalo-0773332973-0068FF?style=for-the-badge&logo=zalo&logoColor=white" alt="Zalo" /></a>

[Tính năng](#-tính-năng) · [Ảnh màn hình](#-ảnh-màn-hình) · [Kiến trúc](#-kiến-trúc) · [Công nghệ](#-công-nghệ) · [Liên hệ](#-liên-hệ)

</div>

## 🏠 Giới thiệu

> Hệ thống nội bộ để một chủ trọ quản lý vài dãy trọ, có thuê người quản lý.

Hệ thống lo trọn vòng lặp hằng tháng: ghi điện nước, ra hóa đơn, thu tiền, đối chiếu, nhắc nợ, xử lý sự cố. Chủ biết phòng nào trống, ai nợ bao nhiêu, quản lý nào đang giữ bao nhiêu tiền mặt, ai sửa gì lúc nào.

## 🔒 Cam kết dữ liệu

> [!IMPORTANT]
> Mục đích chính của hệ thống là để chủ tin được con số. Khi phân vân giữa tiện và đúng, luôn chọn đúng.
>
> - Số trên hóa đơn không thể đổi mà không để lại dấu vết: có nhật ký thao tác và chốt kỳ để khóa số liệu.
> - Quản lý chỉ thấy các dãy được gán, việc xóa dữ liệu thuộc về chủ.
> - Dữ liệu được sao lưu tự động và đã thử khôi phục sang môi trường mới.
> - Ghi điện nước trên điện thoại không phải chờ mạng.

## 👥 Ai dùng gì

| Vai | Nền tảng | Việc chính |
|---|---|---|
| 👑 **Chủ** | Web, Android khi đi kiểm tra | Toàn quyền, báo cáo, duyệt bàn giao tiền, chốt kỳ, sao lưu |
| 🧑‍💼 **Quản lý** | Android, web khi làm hợp đồng hay in ấn | Làm việc trên các dãy được gán, quyền bật tắt riêng cho từng người |
| 🧳 **Người thuê** | Android | Xem hợp đồng và hóa đơn, quét VietQR, báo đã chuyển, báo sự cố, nhận thông báo |

## ✨ Tính năng

- 🏘 **Dãy, phòng, khách, hợp đồng:** sơ đồ phòng, ảnh phòng, chụp CCCD, lập hợp đồng theo bước, tiền cọc, mã mời, in hợp đồng PDF.
- ⚡ **Điện nước và hóa đơn:** ghi chỉ số kể cả khi mất sóng, giá điện bậc thang, nước theo khối hoặc theo người, tạo hóa đơn hàng loạt, điều chỉnh, phí trễ hạn, hóa đơn PDF.
- 💳 **Thanh toán:** VietQR, khách báo đã chuyển rồi quản lý xác nhận, trả một phần, tất toán khi trả phòng có bù trừ tiền cọc.
- 🔍 **Kiểm soát:** bàn giao tiền mặt có chủ xác nhận, biên bản có chữ ký, chốt kỳ, nhật ký thao tác, thùng rác khôi phục được.
- 🛠 **Vận hành:** sự cố hai phía, chi phí và phân bổ chi phí chung vào hóa đơn, thông báo chung, push qua Firebase.
- 📊 **Báo cáo:** doanh thu, đã thu, còn nợ, chi phí, lợi nhuận theo tháng, có biểu đồ, xuất Excel, xuất toàn bộ dữ liệu, sao lưu.

## 📱 App cho người thuê

Người thuê dùng chung app Android với chủ và quản lý: đăng nhập bằng số điện thoại thì app tự vào đúng vai.

- **Vào lần đầu:** nhập mã mời quản lý gửi khi làm hợp đồng, rồi đặt mật khẩu.
- **Hóa đơn:** xem chi tiết từng dòng tiền phòng, điện, nước, dịch vụ; quét VietQR có sẵn số tiền và nội dung; chạm để chép số tài khoản; bấm "Tôi đã chuyển khoản" kèm ảnh để quản lý xác nhận.
- **Hợp đồng:** thông tin phòng, giá thuê, tiền cọc, đơn giá dịch vụ, biên bản bàn giao, tải hợp đồng PDF.
- **Sự cố:** báo hỏng hóc kèm ảnh, mất mạng vẫn gửi được, theo dõi đến khi xử lý xong.
- **Thông báo:** push khi có hóa đơn mới, thanh toán được xác nhận, sự cố được cập nhật, thông báo chung của dãy.

## 📸 Ảnh màn hình

Chụp từ hệ thống chạy thật với dữ liệu mẫu của profile `dev`. Tên, số điện thoại và tài khoản ngân hàng trong ảnh đều là dữ liệu mẫu.

App Android dùng giao diện kính mờ: nền màu dịu, thẻ trong suốt, thanh điều hướng dạng viên kính nổi phía dưới làm nhòe nội dung đang cuộn qua.

### Web cho chủ và quản lý

<table>
  <tr>
    <td width="33%"><img src="docs/assets/screenshots/web-tong-quan.png" alt="Tổng quan" /><br /><sub><b>Tổng quan:</b> lấp đầy, phải thu, nợ, quá hạn</sub></td>
    <td width="33%"><img src="docs/assets/screenshots/web-so-do-phong.png" alt="Sơ đồ phòng" /><br /><sub><b>Sơ đồ phòng</b> theo tầng và trạng thái</sub></td>
    <td width="33%"><img src="docs/assets/screenshots/web-hop-dong.png" alt="Hợp đồng" /><br /><sub><b>Hợp đồng:</b> người ở, cọc, dịch vụ, in PDF</sub></td>
  </tr>
  <tr>
    <td width="33%"><img src="docs/assets/screenshots/web-dien-nuoc.png" alt="Điện nước" /><br /><sub><b>Điện nước:</b> nhập chỉ số cả dãy, cảnh báo số bất thường</sub></td>
    <td width="33%"><img src="docs/assets/screenshots/web-hoa-don.png" alt="Hóa đơn" /><br /><sub><b>Hóa đơn</b> theo kỳ, trạng thái, số còn nợ</sub></td>
    <td width="33%"><img src="docs/assets/screenshots/web-thanh-toan.png" alt="Thanh toán" /><br /><sub><b>Thanh toán:</b> chờ xác nhận và lịch sử</sub></td>
  </tr>
  <tr>
    <td width="33%"><img src="docs/assets/screenshots/web-tien-mat.png" alt="Tiền mặt" /><br /><sub><b>Tiền mặt:</b> ai đang giữ bao nhiêu, bàn giao</sub></td>
    <td width="33%"><img src="docs/assets/screenshots/web-chot-thang.png" alt="Chốt tháng" /><br /><sub><b>Chốt tháng:</b> khóa hóa đơn và chỉ số của kỳ</sub></td>
    <td width="33%"><img src="docs/assets/screenshots/web-bao-cao.png" alt="Báo cáo" /><br /><sub><b>Báo cáo:</b> phải thu, đã thu, lợi nhuận, xuất Excel</sub></td>
  </tr>
</table>

### Android cho quản lý

<table>
  <tr>
    <td width="33%" align="center"><img src="docs/assets/screenshots/android-quan-ly-trang-chu.jpg" alt="Trang chủ quản lý" width="240" /><br /><sub>Trang chủ: nợ, phòng, điện nước, tiền mặt</sub></td>
    <td width="33%" align="center"><img src="docs/assets/screenshots/android-quan-ly-phong.jpg" alt="Sơ đồ phòng" width="240" /><br /><sub>Sơ đồ phòng theo tầng</sub></td>
    <td width="33%" align="center"><img src="docs/assets/screenshots/android-quan-ly-dien-nuoc.jpg" alt="Ghi điện nước" width="240" /><br /><sub>Ghi điện nước, ghi được khi mất mạng</sub></td>
  </tr>
  <tr>
    <td width="33%" align="center"><img src="docs/assets/screenshots/android-quan-ly-hoa-don.jpg" alt="Hóa đơn theo kỳ" width="240" /><br /><sub>Hóa đơn theo kỳ, gửi cho khách</sub></td>
    <td width="33%" align="center"><img src="docs/assets/screenshots/android-quan-ly-tien-mat.jpg" alt="Tiền mặt" width="240" /><br /><sub>Tiền mặt đang giữ, chọn khoản bàn giao</sub></td>
    <td width="33%" align="center"><img src="docs/assets/screenshots/android-quan-ly-them.jpg" alt="Các chức năng" width="240" /><br /><sub>Thêm khách, lập hợp đồng, sự cố, chi phí</sub></td>
  </tr>
</table>

### Android cho người thuê

<table>
  <tr>
    <td width="33%" align="center"><img src="docs/assets/screenshots/android-khach-trang-chu.jpg" alt="Trang chủ người thuê" width="240" /><br /><sub>Trang chủ: tổng còn nợ, phòng, liên hệ</sub></td>
    <td width="33%" align="center"><img src="docs/assets/screenshots/android-khach-ds-hoa-don.jpg" alt="Danh sách hóa đơn" width="240" /><br /><sub>Hóa đơn các kỳ</sub></td>
    <td width="33%" align="center"><img src="docs/assets/screenshots/android-khach-hoa-don.jpg" alt="Hóa đơn và VietQR" width="240" /><br /><sub>Chi tiết hóa đơn, chuyển khoản bằng VietQR</sub></td>
  </tr>
  <tr>
    <td width="33%" align="center"><img src="docs/assets/screenshots/android-khach-hop-dong.jpg" alt="Hợp đồng của tôi" width="240" /><br /><sub>Hợp đồng của tôi, tải PDF</sub></td>
    <td width="33%" align="center"><img src="docs/assets/screenshots/android-khach-su-co.jpg" alt="Báo sự cố" width="240" /><br /><sub>Báo sự cố kèm ảnh, gửi được khi mất mạng</sub></td>
    <td width="33%" align="center"><img src="docs/assets/screenshots/android-khach-thong-bao.jpg" alt="Thông báo" width="240" /><br /><sub>Thông báo hóa đơn, thanh toán, thông báo chung</sub></td>
  </tr>
</table>

## 🧭 Kiến trúc

```mermaid
flowchart LR
    web["Web Next.js<br/>Chủ, quản lý"] --> api
    android["Android<br/>Chủ, quản lý, người thuê"] --> api

    api["Spring Boot API<br/>/api/v1"] --> pg[("PostgreSQL")]
    api --> redis[("Redis")]
    api --> cloudinary["Cloudinary<br/>Ảnh"]
    api --> firebase["Firebase<br/>Push"]
```

Contract API (OpenAPI) viết tay trước khi code và là nguồn sự thật. Kiểu của web và DTO Android đều sinh từ file này.

## 🧰 Công nghệ

| Phần | Công nghệ |
|---|---|
| Backend | Java 21, Spring Boot 3.5, PostgreSQL 16, Redis 7, Flyway, JWT, OpenHTMLtoPDF, Apache POI, Docker |
| Web | Next.js 16 (App Router), React 19, TypeScript, Tailwind CSS 4, HeroUI v3, TanStack Query, Recharts |
| Android | Kotlin, Jetpack Compose, Material 3, Hilt, Retrofit, Room, `minSdk` 26 |

## 📐 Quy ước

- Giao diện và thông báo lỗi tiếng Việt.
- Tiền là số nguyên VND. Múi giờ `Asia/Ho_Chi_Minh`. Ngày `yyyy-MM-dd`, kỳ hóa đơn `yyyy-MM`.
- Mỗi giai đoạn đều qua review code, kiểm tra trên hệ thống thật, đối chiếu số liệu báo cáo với cơ sở dữ liệu.

## 📬 Liên hệ

Cần tìm hiểu thêm, xem demo hay trao đổi về hệ thống, liên hệ:

| Kênh | Thông tin |
|---|---|
| 📧 Email | [toanit5.haui@gmail.com](mailto:toanit5.haui@gmail.com) |
| 💬 Zalo | [0773332973](https://zalo.me/0773332973) |

## 📄 Giấy phép

Dự án nội bộ, không cấp phép sử dụng lại. Đây là trang giới thiệu; mã nguồn để ở repo riêng tư.
