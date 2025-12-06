# TInHocBai12
<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>BÀI 12: Tạo Biểu Mẫu</title>
  <style>
    body { font-family: Arial, sans-serif; background:#f7f7f7; color:#111; padding:20px; }
    .container { max-width:900px; margin:0 auto; background:#fff; padding:24px; border-radius:8px; box-shadow:0 6px 20px rgba(0,0,0,0.08);} 
    pre { white-space:pre-wrap; word-wrap:break-word; background:#f0f0f0; padding:12px; border-radius:6px; overflow:auto; }
    h1{ text-align:center }
  </style>
</head>
<body>
  <div class="container">
    <h1>BÀI 12</h1>

<pre>
Câu hỏi 1 trang 69 Tin học 12: Điểm khác biệt giữa radio, checkbox và select là gì
Lời giải:
*Radio (nút radio):
- Nút radio cho phép người dùng chọn một lựa chọn từ một danh sách các lựa chọn.
- Chỉ có một lựa chọn có thể được chọn trong một nhóm các nút radio.
Khi một nút radio được chọn, các nút radio khác trong cùng nhóm sẽ được tự động bỏ chọn.
- Được sử dụng khi chỉ có một lựa chọn duy nhất được phép.
*Checkbox (hộp kiểm):
- Checkbox cho phép người dùng chọn một hoặc nhiều lựa chọn từ một danh sách các lựa chọn.
- Nhiều checkbox có thể được chọn cùng một lúc.
- Mỗi checkbox hoạt động độc lập với các checkbox khác.
- Thường được sử dụng khi nhiều lựa chọn có thể được chọn hoặc bỏ chọn.
*Select (danh sách thả xuống):
- Select cho phép người dùng chọn một lựa chọn từ một danh sách thả xuống.
- Chỉ có một lựa chọn có thể được chọn tại một thời điểm.
- Người dùng có thể mở danh sách và chọn một mục từ danh sách.
- Thường được sử dụng khi có một danh sách lựa chọn dài hoặc khi không gian trên trang web hạn chế và muốn giữ giao diện gọn gàng.
-> Tóm lại, radio được sử dụng khi chỉ có một lựa chọn được phép, checkbox khi nhiều lựa chọn được phép, và select khi có một danh sách dài các lựa chọn hoặc khi giao diện cần được tối ưu hóa.


Câu hỏi 2 trang 69 Tin học 12: Hãy viết câu lệnh để thêm một nút có tên “Quên mật khẩu” vào biểu mẫu.
Lời giải:

<form>

  <!-- Các trường nhập dữ liệu khác trong biểu mẫu -->

  <!-- Nút "Quên mật khẩu" →

<button type="button" onclick="forgotPassword()">Quên mật khẩu</button>

</form>

Luyện tập trang 70 Tin học 12: Lần lượt tạo các loại phần tử form và các phần tử input với những loại dữ liệu khác nhau và liệt kê ra ba ví dụ có thể sử dụng của từng loại.

Lời giải:

*Phần tử Form:

-Form cơ bản:

Ví dụ: Một biểu mẫu đăng ký tài khoản.
<<form action="/register" method="post">

  <!-- Các phần tử input và nút gửi dữ liệu sẽ được thêm vào đây -->

</form>

-Form có phần tử select:

Ví dụ: Form chọn quốc gia.

<form>

  <label for="country">Quốc gia:</label>

  <select id="country" name="country">

    <option value="vietnam">Việt Nam</option>

    <option value="usa">United States</option>

    <option value="uk">United Kingdom</option>

    <!-- Các quốc gia khác có thể được thêm vào đây -->

  </select>

</form>

- Form với textarea:

Ví dụ: Một ô nhập văn bản lớn cho người dùng nhập ý kiến hoặc phản hồi.

<form>

  <label for="feedback">Phản hồi:</label><br>

  <textarea id="feedback" name="feedback" rows="4" cols="50"></textarea>

</form>

*Phần tử Input:

-Input kiểu text:

Ví dụ: Ô nhập tên người dùng.

<form>

  <label for="username">Tên người dùng:</label>

  <input type="text" id="username" name="username">

</form>

- Input kiểu email:

Ví dụ: Ô nhập địa chỉ email.

<form>

  <label for="email">Email:</label>

  <input type="email" id="email" name="email">

</form>

-Input kiểu date:

Ví dụ: Ô chọn ngày sinh.

<form>

  <label for="birthdate">Ngày sinh:</label>

  <input type="date" id="birthdate" name="birthdate">

</form>




Vận dụng 1 trang 70 Tin học 12: Tạo một biểu mẫu đăng kí thành viên câu lạc bộ.
Lời giải:

<!DOCTYPE html>

<html lang="en">

<head>
<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Biểu mẫu đăng ký thành viên</title>

</head>

<body>

<h2>Đăng ký thành viên</h2>

<form action="/submit_registration" method="post">

  <label for="fullname">Họ và tên:</label><br>

  <input type="text" id="fullname" name="fullname" required><br>

  <label for="email">Email:</label><br>

  <input type="email" id="email" name="email" required><br>

  <label for="birthdate">Ngày sinh:</label><br>

  <input type="date" id="birthdate" name="birthdate" required><br>

  <label for="membership">Loại hình thành viên:</label><br>

  <select id="membership" name="membership">

    <option value="basic">Thành viên cơ bản</option>

    <option value="premium">Thành viên cao cấp</option>

  </select><br>

  <input type="submit" value="Đăng ký">

</form>

</body>

</html>


Vận dụng 2 trang 70 Tin học 12: Sửa lại mã nguồn của trang web đã viết trong Nhiệm vụ 2, Bài 11 để thêm một liên kết cho cụm từ Đăng kí. Khi nháy chuột vào liên kết, trang web đã viết ở câu 1 sẽ được hiển thị trong iframe.
Lời giải:

<!DOCTYPE html>

<html lang="vi">

<head>
<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Trang web nghệ thuật</title>

<style>

  /* CSS để định dạng iframe */

  iframe {

    width: 100%;

    height: 500px;

    border: 1px solid #ccc;

  }
</style>

</head>

<body>

<h1>Nghệ thuật</h1>

<!-- Chèn ảnh minh họa -->

<img src="link_den_anh_minh_hoa.jpg" alt="Hình ảnh minh họa" width="500" height="300">

<!-- Chèn bài hát Quốc ca -->

<audio controls>
src="link_den_bai_hat_quoc_ca.mp3" type="audio/mpeg">

  Trình duyệt của bạn không hỗ trợ phát audio.

</audio>

<!-- Thêm liên kết "Đăng kí" -->

<p><a href="link_den_trang_web.html" target="iframe_content">Đăng ký</a></p>

<!-- iframe để hiển thị trang web đã viết ở câu 1 -->

<iframe name="iframe_content" frameborder="0"></iframe>

</body>

</html>
</pre>

  </div>
</body>
</html>
