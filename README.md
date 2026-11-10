# Lumi English: bản miễn phí

Web app học tiếng Anh cho học sinh tiểu học, lớp 1 đến lớp 5, **bám sát khung chương trình chuẩn** môn Tiếng Anh tiểu học. App miễn phí hoàn toàn, không quảng cáo, không cần máy chủ.

> **Lưu ý:** Lumi English là ứng dụng độc lập, **không phải ứng dụng chính thức** của bất kỳ nhà xuất bản, bộ sách giáo khoa hay cơ quan quản lý giáo dục nào, và không có liên kết với các đơn vị này. Từ vựng, mẫu câu, bài tập, nhân vật và hình ảnh do Lumi tự biên soạn.

## Gồm những gì

- `index.html`: toàn bộ app, gồm giao diện, dữ liệu 92 Unit và mã chạy.
- `manifest.webmanifest`: cho phép "Thêm vào màn hình chính" trên điện thoại.
- `.nojekyll`: để GitHub Pages phục vụ file nguyên trạng.
- `OFL-fonts.txt`: giấy phép SIL Open Font License 1.1 của hai font Baloo 2 và Nunito, đã nhúng sẵn trong `index.html`.
- `apple-touch-icon.png`, `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `favicon.png`, `lumi-owl.svg`: icon cú Lumi, dùng khi "Thêm vào màn hình chính" trên iPhone và Android, và làm icon tab trình duyệt.

## Đưa lên GitHub Pages

1. Tạo một repository mới trên GitHub, ví dụ `lumi-english`.
2. Tải tất cả các file trong thư mục này lên nhánh `main`: chọn **Add file → Upload files**, rồi kéo thả.
3. Vào **Settings → Pages**. Ở mục **Source**, chọn **Deploy from a branch**, nhánh `main`, thư mục `/ (root)`, rồi bấm **Save**.
4. Sau khoảng 1 phút, app chạy tại `https://<tên-tài-khoản>.github.io/lumi-english/`.

Dùng dòng lệnh thì làm như sau:

```bash
git init && git add . && git commit -m "Lumi English" && git branch -M main
git remote add origin https://github.com/<tên-tài-khoản>/lumi-english.git
git push -u origin main
```

## Dữ liệu được lưu ở đâu

- Tài khoản, tiến độ và sao được lưu trong **trình duyệt của từng máy** (localStorage). Không có máy chủ nào nhận dữ liệu.
- Mỗi máy có dữ liệu riêng. Muốn chuyển sang máy khác, ba mẹ vào **Tài khoản → Sao lưu dữ liệu → Tải file sao lưu**, rồi trên máy mới bấm **Khôi phục từ file sao lưu** ngay ở màn hình đầu hoặc màn đăng nhập.
- Nếu xóa lịch sử hoặc dữ liệu trang web trong trình duyệt, dữ liệu sẽ mất. Ba mẹ nên tải file sao lưu định kỳ.
- Mật khẩu được băm (SHA-256) trước khi lưu. Tuy vậy, đây là app dùng nội bộ trong gia đình hoặc lớp học, không phải hệ thống bảo mật nhiều người dùng.

## Chọn lớp

Sau khi nhập mã PIN, con chọn lớp muốn học (lớp 1 đến lớp 5), dù đang học lớp mấy. Ví dụ, một bạn lớp 4 vẫn có thể ôn lại lớp 1, 2, 3. Lớp của con được đánh dấu ⭐, lớp học gần nhất được ghi nhớ. Trong mỗi lớp, các Unit mở lần lượt theo đúng thứ tự sách. Ba mẹ có thể bật "Mở khóa toàn bộ bài học" để con vào bất kỳ Unit nào.

## Bảo vệ khu vực ba mẹ

- Khu vực ba mẹ **tự khóa** khi mở lại app hoặc sau **10 phút** không thao tác. Muốn vào lại phải nhập mật khẩu hoặc mã PIN ba mẹ, nên con không tự duyệt nhiệm vụ hay tặng sao được.
- Nút **🎒 Cho con học** ở đầu khu vực ba mẹ chuyển về màn chọn hồ sơ để con nhập PIN.
- **Quên mật khẩu:** ở màn đăng nhập, nhập số điện thoại/email và mã PIN ba mẹ để đặt mật khẩu mới. Nhập sai PIN 5 lần sẽ bị khóa 1 phút.

## Giọng đọc

App dùng giọng đọc tiếng Anh có sẵn trong máy. Nếu máy chưa có, bài học sẽ hiện hướng dẫn cài cho Android, iPhone và Windows. Trong lúc chờ cài, bài nghe hiện chữ để con vẫn làm được.

## Tài khoản mẫu

Khung "Mở gia đình mẫu" tự ẩn khi máy đã có tài khoản thật.

Bấm **Mở gia đình mẫu** ở màn hình đầu để xem thử.

- Ba mẹ: `demo` / `123456`, mã PIN ba mẹ `0000`
- Bông (lớp 1): PIN `1111`
- Tí (lớp 3): PIN `2222`

## Quyền riêng tư và điều khoản

- Trang **Chính sách quyền riêng tư & Điều khoản sử dụng** mở từ link cuối màn hình đầu, hoặc từ **Khu vực ba mẹ → Tài khoản**.
- Không quảng cáo, không cookie theo dõi, không công cụ phân tích.
- Font chữ nhúng sẵn trong app, nên khi học app không kết nối tới máy chủ nào bên ngoài.

## Ủng hộ Lumi

Ở màn **Ba mẹ đăng nhập** và cuối tab **Khu vực ba mẹ → Tổng quan** có mục "Donate Lumi ly cafe cho tỉnh táo nếu ba mẹ thấy ổn nè ☕", kèm mã VietQR (MB Bank · TAO MINH HIEN · 141431319191). Mọi sự ủng hộ Lumi là hoàn toàn tự nguyện để duy trì và phát triển ứng dụng miễn phí, không đi kèm nghĩa vụ hay dịch vụ thương mại. Mã QR nằm trong `src/donate.js` ở mã nguồn.

## Sửa nội dung bài học

Nội dung nằm trong mã nguồn ở `src/data.js`, mỗi dòng là một Unit:

```
Tên Unit|Tên tiếng Việt|Biểu tượng|từ=nghĩa=hình;...|Mẫu câu=Nghĩa;...|Nhiệm vụ ở nhà
```

Sửa xong thì chạy `./build-free.sh` để tạo lại `free/index.html`.
