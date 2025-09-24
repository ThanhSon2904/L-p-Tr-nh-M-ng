<h2 align="center">
    <a href="https://dainam.edu.vn/vi/khoa-cong-nghe-thong-tin">
    🎓 Faculty of Information Technology (DaiNam University)
    </a>
</h2>
<h2 align="center">
   Chat nhóm bằng RMI
</h2>
<div align="center">
    <p align="center">
      <img src="https://github.com/ThanhSon2904/LapTrinhMang/blob/main/RMIChat/%E1%BA%A3nh/z7026817800988_bd4f94fd23cb498776fdad1ad7b8fc7e.jpg?raw=true" alt="AIoTLab Logo" width="170"/>
      <img src="https://github.com/ThanhSon2904/LapTrinhMang/blob/main/RMIChat/%E1%BA%A3nh/z7026817704248_4ff8a524df07723a4f18bb38d1383399.jpg?raw=true" width="180"/>
      <img src="https://github.com/ThanhSon2904/LapTrinhMang/blob/main/RMIChat/%E1%BA%A3nh/z7026817718006_b7ad42aa92ae2479ae906d66dfcbaa90.jpg?raw=true" alt="DaiNam University Logo" width="200"/>
    </p>
[![AIoTLab](https://img.shields.io/badge/AIoTLab-green?style=for-the-badge)](https://www.facebook.com/DNUAIoTLab)
[![Faculty of Information Technology](https://img.shields.io/badge/Faculty%20of%20Information%20Technology-blue?style=for-the-badge)](https://dainam.edu.vn/vi/khoa-cong-nghe-thong-tin)
[![DaiNam University](https://img.shields.io/badge/DaiNam%20University-orange?style=for-the-badge)](https://dainam.edu.vn)

</div>

## 📖 1. Giới thiệu hệ thống


- Hệ thống được xây dựng theo mô hình Client – Server nhằm mục đích trao đổi dữ liệu và gửi/nhận tin nhắn giữa hai phía thông qua lập trình socket trong Java.  
- **Server**: đóng vai trò trung tâm, lắng nghe các kết nối từ client. Sau khi có kết nối, server nhận dữ liệu từ client và có thể phản hồi ngược lại.  
- **Client**: đóng vai trò gửi yêu cầu đến server, truyền dữ liệu/tin nhắn và chờ phản hồi.  
- Hệ thống này mô phỏng nguyên lý cơ bản của các ứng dụng chat, truyền tin hoặc trao đổi dữ liệu trong thực tế, giúp người học nắm vững cách xây dựng ứng dụng phân tán bằng Java.  

## 🔧 2. Công nghệ sử dụng
Ngôn ngữ lập trình: Java (JDK 8+)  
Mô hình mạng: Client–Server  

Kỹ thuật:  
- Java Socket API (`java.net.Socket`, `java.net.ServerSocket`) để thiết lập kết nối TCP  
- Luồng I/O (`InputStream`, `OutputStream`, `BufferedReader`, `PrintWriter`) để đọc/ghi dữ liệu qua mạng  

IDE khuyến nghị: Eclipse hoặc IntelliJ IDEA (có thể chạy bằng terminal)  
Hệ điều hành: Windows/Linux/macOS  

## 🚀 3. Hình ảnh các chức năng

<p align="center">
<img src="https://github.com/ThanhSon2904/LapTrinhMang/blob/main/RMIChat/%E1%BA%A3nh/giao%20di%E1%BB%87n.png?raw=true" alt="Chức năng đăng nhập" width="600"/>
</p>

<p align="center">
  <em>Hình 1: Ảnh giao diện  </em>
</p>

<p align="center">
<img src="https://github.com/ThanhSon2904/LapTrinhMang/blob/main/RMIChat/%E1%BA%A3nh/2%20ng%C6%B0%E1%BB%9Di%20chat%20v%E1%BB%9Bi%20nhau.png?raw=true" alt="Chức năng đăng ký" width="600"/>
</p>
<p align="center">
  <em> Hình 2: ảnh 2 người chat với nhau </em>
</p>


<p align="center">
  <img src="https://github.com/ThanhSon2904/LapTrinhMang/blob/main/RMIChat/%E1%BA%A3nh/%C4%91%C4%83ng%20k%C3%BD.png?raw=true" alt="Hệ thống thông báo tham gia thành công" width="400"/>
</p>
<p align="center">
  <em> Hình 3: đăng ký  .</em>
</p>

<p align="center">
  <img src="https://github.com/ThanhSon2904/LapTrinhMang/blob/main/RMIChat/%E1%BA%A3nh/%C4%91%C4%83ng%20nh%E1%BA%ADp.png?raw=true" alt="Giao diện hai người chat với nhau" width="400"/>
</p>
<p align="center">
  <em> Hình 4: đăng nhập </em>
</p>


## 📝 4. Hướng dẫn cài đặt và sử dụng

### 🔧 Yêu cầu hệ thống

## Yêu cầu hệ thống

- Java 8 trở lên
- MongoDB 4.0 trở lên
- Ant (để build project)

## Cài đặt và chạy

### 1. Cài đặt MongoDB

Tải và cài đặt MongoDB từ: https://www.mongodb.com/try/download/community
Khởi động MongoDB:
```bash
mongod
```

### 2. Download dependencies

```bash
ant download-deps
```

### 3. Build project

```bash
ant compile
```

### 4. Chạy Server

```bash
ant run-server
```

### 5. Chạy Client

Mở terminal mới và chạy:
```bash
ant run-client
```

Hoặc chạy nhiều client để test:
```bash
ant run-client
ant run-client
ant run-client
```



### Đăng ký/Đăng nhập
- Mở client, nhập tên đăng nhập và mật khẩu
- Chọn "Đăng ký" để tạo tài khoản mới
- Chọn "Đăng nhập" để đăng nhập với tài khoản có sẵn

### Chat
- Gõ tin nhắn và nhấn Enter hoặc nút "Gửi"
- Tin nhắn sẽ được gửi đến tất cả người dùng trong phòng hiện tại
- Lịch sử chat được tự động load khi vào phòng


### Thay đổi port server
Sửa trong `Server.java`:
```java
private static final int PORT = 8888; // Đổi port ở đây
```


### Thay đổi server host
Sửa trong `Client.java`:
```java
private static final String SERVER_HOST = "localhost";
```


### Lỗi kết nối Server
- Đảm bảo Server đã khởi động
- Kiểm tra port có bị chiếm không
- Kiểm tra firewall



## Thông tin liên hệ  
Họ tên: Nguyễn Thanh Sơn
Lớp: CNTT 16-01.  
Email: sonn29042004@gmail.com

© 2025 AIoTLab, Faculty of Information Technology, DaiNam University. All rights reserved.

---
