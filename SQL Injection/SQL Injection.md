# SQL Injection

Thuộc chủng lỗi Injection. SQL là một kiểu ngôn ngữ giao tiếp với cơ sở dữ liệu.

## Dấu hiệu nhận biết

**Chương trình nhận vào một tham số chứa kết quả là một `id`,`name`,... Hay bất kì thứ gì**

**Thường hay tồn tại ở các chức năng như đăng nhập-đăng ký, search, profile, view,...** 

**Nói chung là các chức năng liên quan đến việc display cho người dùng các thông tin abcxyz**

**Lưu ý có dạng Second-Order**

**Để ý phản ứng của các dấu Backslash, vì Mysql vẫn xử lý backslash như thường**

----

*Hãy sử dụng các test case và quan sát phản hồi để đưa ra giả thuyết tiếp theo hoặc kết luận*