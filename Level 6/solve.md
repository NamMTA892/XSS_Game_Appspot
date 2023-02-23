# Solve  
Chúng ta có giao diện:  
![Imgur](https://i.imgur.com/ASjZpCw.png)  
Kiểm tra source:  
![Imgur](https://i.imgur.com/F52o3xN.png)  
Lấy url sau dấu thăng # làm gadget, không thì lấy giá trị mặc định  
![Imgur](https://i.imgur.com/kk4LBPw.png)  
Tạo Element 'script'
Đầu tiên là check url có http không, chúng ta có thể bypass bằng HTTP  
Truyền url vào src biến và sau đó truyền dữ liệu vào cho biến log và thêm vào trong trang  
Bài này là bài cuối nhưng khá dễ :v  
![Imgur](https://i.imgur.com/JwXY9po.png)  
Payload: data:text/html,alert('XSS')  
![Imgur](https://i.imgur.com/N3CDf5u.png)