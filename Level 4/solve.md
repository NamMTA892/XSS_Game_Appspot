# Solve  
Chúng ta có giao diện:  
![Imgur](https://i.imgur.com/3q47sWg.png)  
Và sau khoảng thời gian 3 giây:  
![Imgur](https://i.imgur.com/HymxcJf.png)  
Nếu chúng ta input character hay string thì sao:  
![Imgur](https://i.imgur.com/pzYsyYT.png)  
Setup mặc định là 3s.  
Cùng nhìn vào line 21 trong timmer.html:  
![Imgur](https://i.imgur.com/OgyKQJe.png)  
![Imgur](https://i.imgur.com/h3Hsy9n.png)  
Nó nhận biến timer đầu vào và Event onload sẽ gọi đến func Startime. Nhìn kĩ lại dòng 21, chúng ta sẽ thấy timer cho phép truyền untrusted data. (timer được truyền dưới dạng string)  
Chúng ta sẽ đóng lời gọi hàm Onload và thực thi lệnh JS theo ý muốn  
![Imgur](https://i.imgur.com/90wsXuz.png)  
'''  
timer = 1'); alert('XSS  
'''  
Khi truyền vào vào Startime:  
'''  
onload = "Startime('1'); alert('XSS');" />  
'''  
Decode payload:%31%27%29%3b%20%61%6c%65%72%74%28%27%58%53%53  
![Imgur](https://i.imgur.com/nEL89Rk.png)  
