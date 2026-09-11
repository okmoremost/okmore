# okmore

[English](README.md) | [简体中文](README.zh.md) | [繁體中文](README.zh-Hant.md) | [Português](README.pt.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Türkçe](README.tr.md) | [العربية](README.ar.md) | [ไทย](README.th.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) | [Bahasa Melayu](README.ms.md)

## Tải xuống

Các liên kết bên dưới luôn trỏ đến gói phiên bản mới nhất (GitHub Release):

- **Zh/En**: [okmore_lite.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_lite.apk)
- **All Language**: [okmore_full.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_full.apk)

> Tất cả các lượt tải xuống đều đi qua `releases/latest/download/`, vì vậy bạn luôn nhận được gói mới nhất mà không cần cập nhật địa chỉ này.

## Bản địa hóa

Chúng tôi hoan nghênh mọi người tham gia đóng góp cho việc bản địa hóa dự án này — dù là thêm một ngôn ngữ mới hay cải thiện bản dịch hiện có. Mọi sự giúp đỡ đều được trân trọng.

Tất cả các chuỗi có thể dịch nằm trong thư mục `res/`. Mỗi ngôn ngữ có thư mục riêng được đặt tên theo locale của nó:

- `res/values/` — chuỗi mặc định/cơ sở (tiếng Trung giản thể), dùng làm nguồn tham chiếu
- `res/values-en/` — tiếng Anh
- `res/values-ja/` — tiếng Nhật
- `res/values-ko/` — tiếng Hàn
- `res/values-ru/` — tiếng Nga
- `res/values-de/` — tiếng Đức
- `res/values-fr/` — tiếng Pháp
- `res/values-es/` — tiếng Tây Ban Nha
- `res/values-pt/` — tiếng Bồ Đào Nha
- `res/values-it/` — tiếng Ý
- `res/values-tr/` — tiếng Thổ Nhĩ Kỳ
- `res/values-ar/` — tiếng Ả Rập
- `res/values-th/` — tiếng Thái
- `res/values-vi/` — tiếng Việt
- `res/values-in/` — tiếng Indonesia
- `res/values-ms/` — tiếng Mã Lai
- `res/values-zh-rTW/` — tiếng Trung phồn thể

Mỗi thư mục chứa một tệp `strings.xml`. Thuộc tính `name` của mỗi mục `<string>` là khóa và **không được thay đổi** — chỉ dịch phần văn bản giữa các thẻ.

### Cách dịch

1. Fork kho lưu trữ này và sao chép (clone) về máy cục bộ.
2. Mở thư mục `res/` và tìm thư mục ngôn ngữ bạn muốn làm việc.
   - Để **cải thiện một ngôn ngữ hiện có**, chỉnh sửa trực tiếp tệp `strings.xml` của ngôn ngữ đó.
   - Để **thêm một ngôn ngữ mới**, sao chép `res/values-en/strings.xml` vào một thư mục mới có tên `values-<locale>` (ví dụ `values-nl` cho tiếng Hà Lan), sau đó dịch nội dung của nó.
3. Dịch giá trị của mỗi mục `<string>`. Luôn dùng `res/values/strings.xml` làm tham chiếu cho nghĩa gốc.
4. Giữ nguyên các placeholder (như `%1$s`, `%d`) và các thẻ định dạng (như `<b>`, `\n`) y như chúng vốn có — tuyệt đối không dịch hay xóa chúng.
5. Xóa các mục có `translatable="false"` hoặc để nguyên; chúng không nên được dịch.
6. Kiểm thử các thay đổi của bạn, sau đó mở một Pull Request mô tả ngôn ngữ bạn đã cập nhật.

Ví dụ:

```xml
<!-- res/values/strings.xml (source) -->
<string name="web_browsing_settings">网页浏览设置</string>

<!-- res/values-en/strings.xml (translation) -->
<string name="app_name">Browsing Settings</string>
```

Cảm ơn bạn đã giúp okmore tiếp cận được nhiều người hơn trên toàn thế giới!
