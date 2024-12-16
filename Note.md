## Bạn có thể mô tả chi tiết quy trình bạn sử dụng khi thực hiện một cuộc tấn công Penetration Testing trên một ứng dụng web không?

- Tìm hiểu về ứng dụng - chức năng của ứng dụng
- Do thám bằng các công cụ - Indexed, nếu nghi ngờ, có thể đưa những test case trước
- Đặt giả thuyết -> Đưa các test case -> Quan sát ứng dụng phản hồi : 
- Error Messsages
- Unexpected Data
- Time Response
- Unexpected Behavior

- Tiếp tục đưa các test-case cho đến bước kết luận sơ bộ -> Payload hoàn chỉnh.

## Trong các công cụ bạn đã sử dụng như BurpSuite, nmap, amass, bạn thấy công cụ nào hữu ích nhất trong quá trình tấn công web và tại sao?

Công cụ BurpSuite:
- Vì đây là công cụ giúp em quan sát tất cả quá trình ứng dụng xử lý và phản hồi một cách chi tiết hơn so với việc `nhìn thấy` ở Client. Đây cũng là một công cụ giúp đưa các test-case và quan sát dễ dàng hơn.
Ngoài ra còn có công cụ FFuF:
- Đây là một công cụ brute-force mạnh mẽ, em thường dùng nó để scan directory, hoặc test các trường hợp rate-limit vulnerability

## Bạn có thể giải thích rõ hơn về cách bạn khai thác lỗ hổng File Upload để thực hiện Remote Code Execution (RCE)? Cụ thể bạn đã sử dụng phương pháp gì?

Về việc khai thác lỗi File Upload, em thường khai thác bằng Webshell, ở các ngôn ngữ lập trình file-based chẳng hạn như PHP. 
Trong quá trình sử dụng thử ứng dụng, và Do thám. Nhận thấy có các trường cho phép upload, từ đó đưa ra các test case và quan sát cách ứng dụng xử lý. Sau đó sẽ kết luận sơ bộ.

## Khi thực hiện tấn công XSS, bạn thường gặp phải những vấn đề gì và bạn đã giải quyết chúng như thế nào?

