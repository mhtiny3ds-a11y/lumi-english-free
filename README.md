# Lumi English: bản miễn phí

Web app học tiếng Anh cho học sinh tiểu học, lớp 1 đến lớp 5, bám theo bộ sách **Global Success**. App miễn phí hoàn toàn, không quảng cáo, không cần máy chủ.

## Gồm những gì

- `index.html`: toàn bộ app, gồm giao diện, dữ liệu 92 Unit và mã chạy.
- `manifest.webmanifest`: cho phép "Thêm vào màn hình chính" trên điện thoại.
- `.nojekyll`: để GitHub Pages phục vụ file nguyên trạng.

## Đưa lên GitHub Pages

1. Tạo một repository mới trên GitHub, ví dụ `lumi-english`.
2. Tải 3 file trong thư mục này lên nhánh `main`: chọn **Add file → Upload files**, rồi kéo thả.
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
- Mỗi máy có dữ liệu riêng. Muốn chuyển sang máy khác, ba mẹ vào **Tài khoản → Sao lưu dữ liệu → Tải file sao lưu**, rồi trên máy mới chọn **Khôi phục từ file**.
- Nếu xóa lịch sử hoặc dữ liệu trang web trong trình duyệt, dữ liệu sẽ mất. Ba mẹ nên tải file sao lưu định kỳ.
- Mật khẩu được băm (SHA-256) trước khi lưu. Tuy vậy, đây là app dùng nội bộ trong gia đình hoặc lớp học, không phải hệ thống bảo mật nhiều người dùng.

## Tài khoản mẫu

Bấm **Mở gia đình mẫu** ở màn hình đầu để xem thử.

- Ba mẹ: `demo` / `123456`, mã PIN ba mẹ `0000`
- Bông (lớp 1): PIN `1111`
- Tí (lớp 3): PIN `2222`

## Sửa nội dung bài học

Nội dung nằm trong mã nguồn ở `src/data.js`, mỗi dòng là một Unit:

```
Tên Unit|Tên tiếng Việt|Biểu tượng|từ=nghĩa=hình;...|Mẫu câu=Nghĩa;...|Nhiệm vụ ở nhà
```

Sửa xong thì chạy `./build-free.sh` để tạo lại `free/index.html`.
