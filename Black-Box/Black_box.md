# Black Box Testing

## Các đặc điểm khi Pentest Black Box

Black Box là khi bạn `mơ hồ` về hệ thống. Không có thông tin cụ thể và tất cả thông tin đều là `điểm mù`.

Giống như việc `tự học`. Chúng ta phải tìm hiểu các thông tin của một hệ thống theo cách của cá nhân chúng ta.

*Không nên bỏ sót bất cứ thông tin gì trong quá trình kiểm thử Black Box*

*Phải đặt giả thuyết cho tất cả trường hợp*

**Quy trình gồm 4 bước sau :**

```
1/ Đánh giá sơ bộ
2/ Đặt giả thuyết và quan sát dấu hiệu
3/ Kiểm tra chi tiết + Xét nghiệm (Test)
4/ Kết luận sơ bộ
```


-----
### 1/ Do thám - Recon : 

- Phải Do thám thật kĩ, tìm ra các Attack Surface khác mà các Hacker ít khi lui đến, coi như cũng né được vài đối thủ
- Noting tất cả những thông tin nhận được khi Recon, tránh việc bỏ quên thông tin dẫn đến bỏ quên Bug
- Sử dụng Wordlists thật hiệu quả đối với từng trường hợp Pentest
- Sử dụng các công cụ một cách đúng đắn, trong phạm vi ứng dụng cho phép
### 2/ Nhận biết các tính năng này, sẽ dẫn đến các lỗi bảo mật gì ..

- Upload File -> File Upload Vuln | Path Traversal | ...
- Search -> XSS Reflected/DOM | SQL Injection | ... 
- Comment -> XSS Store | SQL Injection | ....
- Sign In/ Sign Up -> SQL Injection
- Disclosure Resource -> RCE | Disclosure API Key | user/password | ...
 
### 3/ Phản hồi 

- Error Messsages
- Unexpected Data
- Time Response
- Unexpected Behavior
### 4/ Xây dựng các Test-case cho các function/lỗi bảo mật

- Xây dựng và sử dụng những test case đơn giản để quan sát dấu hiệu trả về là gì. Từ đó đặt giả thuyết tiếp theo.
- Hãy chậm rãi đi từng bước, đừng vội vàng ồ ập vào một thứ gì đó quá, Blue team sẽ dễ nghi ngờ.