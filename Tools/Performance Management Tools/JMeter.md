# JMeter
1. What is JMeter?
2. What is Element in JMeter?
3. How to use JMeter?
4. Output of JMeter.

## 1. What is JMeter?
JMeter là 1 phần mềm mô phỏng 1 nhóm người dùng gửi yêu cầu tới 1 máy chủ, trả về trạng thái thông tin của máy chủ thông qua các luồng graphic và tạo test report trong các format khác.<br/>
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/c7128dbb-eb3f-498a-baa2-77123e4a3453)

## 2. What is Element in JMeter?
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/e741cbbf-ad1c-4e5f-b37f-3dacf8cdfc56)

* Thread Group
là mô phỏng các thread mà mỗi thread ứng với 1 người dùng được mô phỏng.
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/e418a175-43c8-452c-8af3-9f72d553d536)

* Samplers
cho phép các thread group biết chúng cần dùng giao thức gì để kết nối tới server. ví dụ như HTTP, FTP, JDBC ...
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/ff7bc885-c922-4f53-a869-5e4e5e04458e)

  * Dùng FTP để gửi request tới máy chủ FTP:<br/>
  ![image](https://github.com/7gr4g0n338/Tester/assets/95563870/769c871b-4ff1-4408-8991-44084a3e7200)
  ![image](https://github.com/7gr4g0n338/Tester/assets/95563870/4710fad5-f923-4799-8d59-b52d0ca6de4f)

  * Dùng HTTP request:<br/>
  ![image](https://github.com/7gr4g0n338/Tester/assets/95563870/372de0de-1ea0-4cb0-a7ba-b44f10b2697d)

  * Dùng JDBC request để gửi request tới máy chủ DB:<br/>
  ![image](https://github.com/7gr4g0n338/Tester/assets/95563870/7efec0cb-e151-4d27-b0bf-477953ed9e35)
  ![image](https://github.com/7gr4g0n338/Tester/assets/95563870/cb356a4d-46b9-4101-8ce6-aabbccf2b0b9)

  * BSF sampler cho phép ghi các sampler sử dụng BSF scripting language:<br/>
  ![image](https://github.com/7gr4g0n338/Tester/assets/95563870/702b5de3-830e-4f52-bef9-b066f510ed76)

  * Access Log Sampler cho phép đọc access logs và tạo các yêu cầu HTTP:<br/>
  ![image](https://github.com/7gr4g0n338/Tester/assets/95563870/ced8342e-479c-4707-aa8d-ecdb7142be73)

  * SMTP Sampler dùng để gửi email message bằng giao thức SMTP:<br/>
  ![image](https://github.com/7gr4g0n338/Tester/assets/95563870/3c16225f-50f9-45de-9bfc-85753028b8d5)

* Listeners
Hiển thị các kết quả của test execution ở những định dạng format khác nhau như dạng tree, table, graph hoặc log file.<br/>
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/c4d78c00-ab46-44d7-ab18-3f13c915257a)

  * Graph:<br/>
  ![image](https://github.com/7gr4g0n338/Tester/assets/95563870/2177e6b1-e3f9-4da4-84e5-cf4daa52eb5c)

  * Tree:<br/>
  ![image](https://github.com/7gr4g0n338/Tester/assets/95563870/1c5905b9-2654-44ce-bd02-79b1a01241f1)

  * Table:<br/>
  ![image](https://github.com/7gr4g0n338/Tester/assets/95563870/5ba9ee15-260d-43c7-acd5-ee88888ba325)

  * Text:<br/>
  ![image](https://github.com/7gr4g0n338/Tester/assets/95563870/2b12bbdf-3316-476c-983e-ec8c2121e65f)


