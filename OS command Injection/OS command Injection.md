# OS Command Injection

Là một lỗi trong các chủng lỗi Injection, nối dài câu query khiến cho hệ thống nhầm lẫn `User Input` và `Instruction`

## Dấu hiệu nhận biết

**Chương trình sử dụng các chức năng của tầng Kernel**

**Error/Time-Base (Dựa vào việc Response không rõ ràng)**

**Kiểm tra có Proxy hay không? Có kết nối Internet được không? Ngoài ra còn có chức năng nào khác không? (Chẳng hạn như Writable)**

**Chuẩn bị Chương trình để Brute-Force:**

*Những thông tin cần thiết:*

- Cần phải biết hệ điều hành này sử dụng Bash hay Shell
- `head -n` + numeric : Lấy dòng bao nhiêu ? Giống LIMIT bên SQL
- `cut -c` + numeric : Lấy kí tự thứ bao nhiêu ?
- sleep + numeric : Dành cho Time-Base/Blind
- Xem thử có bị giới hạn độ dài không ?
- Phải kiểm tra tất cả các kí tự được phép và các kí tự không được phép để loại suy

*Nói chung cái này còn khá mông lung về dấu hiệu nhận biết, bởi vì website ít khi sử dụng các chức năng ở tầng Kernel*

*Nhưng không phải là không có. Tốt nhất không nên để sót bất cứ `thông tin` gì!*