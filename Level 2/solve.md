# Solve  
![Imgur](https://i.imgur.com/7xUYC0I.png)  
Cho phép ta nhập đầu vào ở trong textarea và tạo ra 1 bài post  
![Imgur](https://i.imgur.com/FqzA49v.png)  
Thử đầu vào với dòng '''<h1>Nam</h1>'''  
![Imgur](https://i.imgur.com/X4OixJ8.png)  
Vậy chúng ta có thể nhập untrusted data  
Check source:  
![Imgur](https://i.imgur.com/cP5TLpP.png)  
Vùng textarea có id là "post-content" có hàm nhận id là:  
![Imgur](https://i.imgur.com/8embp3T.png)  
Sau khi đưa vào DB để lưu trữ thì sẽ có hàm xuất ra màn hình:  
![Imgur](https://i.imgur.com/5eRr4El.png)  
Nhìn vào đoạn code trên, chúng ta có thể thấy, đoạn html được cộng từng phần lại sau đó mới đưa vào trong trang chính với innerHTML method. Vì vậy khi ta nhập '''<script>alert('XSS')</script>'''  
![Imgur](https://i.imgur.com/adZMDoU.png)  
Vì vậy solution sẽ là sử dụng các Event trong HTML như Onmouseover, Onerror, ...  
![Imgur](https://i.imgur.com/9RiTbgu.png)  
![Imgur](https://i.imgur.com/FWpNmY7.png)  
