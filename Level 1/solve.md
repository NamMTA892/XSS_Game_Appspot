# Solve  
Ta có giao diện như sau:  
![Imgur](https://i.imgur.com/hbAYMHn.png)  
Bài cho phép ta truyền dữ liệu vào cho biến 'query'  
![Imgur](https://i.imgur.com/P23dtt5.png)  
Nhưng không kiểm tra đầu vào, vì vậy với đoạn code trên ta có thể thực thi XSS bằng payload đơn giản:  

'''
<script>alert('XSS')</script>  
'''  

![Imgur](https://i.imgur.com/BKjjZy1.png)  
