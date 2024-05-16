# JMeter
1. What is JMeter?
2. What is Element in JMeter?
3. How to use JMeter?
4. Output of JMeter.

## I. What is JMeter?
JMeter là 1 phần mềm mô phỏng 1 nhóm người dùng gửi yêu cầu tới 1 máy chủ, trả về trạng thái thông tin của máy chủ thông qua các luồng graphic và tạo test report trong các format khác.<br/>
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/c7128dbb-eb3f-498a-baa2-77123e4a3453)

## II. What is Element in JMeter?
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

## III. How to use JMeter?
GUI của JMeter gồm 2 thành phần chính là Test plan - là nơi thêm/lưu trữ các thành phần được yêu cầu cho JMeter test  như requests, results, ...
và Workbench - là nơi lưu trữ các thành phần test tạm thời, không liên quan gì tới test plan.<br/>
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/6ded060e-1529-44c3-b0fd-e4f4f8d8a15b)

### 1. JMeter Performance Testing
Performance Testing bao gồm 2 việc:<br/>
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/35fa47a1-a4dc-4177-b624-2d09cdaca4d9)

+ Load testing thực hiện mô phỏng nhiều truy cập của người dùng với lượng truy cập `mong đợi` - tải trọng mong muốn.
+ Stress testing thực hiện mô phỏng khả năng load tối đa mà server có thể xử lý được.

### 2. Create a Performance Test Plan in JMeter

Trước khi thực hiện kiểm tra hiệu năng của ứng dụng cần xác định:
+ Normal Load: số người dùng trung bình truy cập website
+ Heavy Load: số lượng tối đa người dùng truy cập
+ Mục đích test của ta là gì trong bài test này?<br/>
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/73384194-9a89-4e72-ae4b-814733f3790e)

#### Add thread group
Right click on the “Test Plan” and add a new thread group: Add -> Threads (Users) -> Thread Group <br/>
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/5365002e-3c45-421e-8598-109e6e31b209)

In the Thread Group control panel, enter Thread Properties as follows:<br/>
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/efcdb6fb-e5b3-4709-9913-3556c4a36d7f)

Number of Threads: 100 (Number of users connects to the target website: 100)<br/>
Loop Count: 10 (Number of time to execute testing)<br/>
Ramp-Up Period: 100<br/>

Nếu có 100 user và Ramp-Up period là 100 thì thời gian delay giữa các người dùng liên tiếp là 100/100=1s.<br/>
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/3bab2477-b747-465d-86ef-b2b1243d202f)

#### Add JMeter elements
Ví dụ: Element là HTTP request default.<br/>
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/f81ede20-6639-45d3-9811-d16f66507757)
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/f4c8642f-ecf3-4d5e-8799-0d57fb0c770d)

Add sampler HTTP Request:<br/>
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/15d7c4db-4fb4-49dc-a3d5-34173f52b36c)

In HTTP Request Control Panel, the Path field indicates which URL request you want to send to Google server. ví dụ: if you enter “calendar” in Path field. JMeter will create the URL request http://www.google.com/calendar to Google server.<br/>
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/fc5902de-9a33-499d-9149-8783ce846179)

#### Adding Graph result
JMeter can show the test result in Graph format.
Right click Test Plan, Add -> Listener -> Graph Results<br/>
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/aec69598-52e2-4ab5-8d49-cbce6c4e7fd5)

#### Run Test and get the test result
Nhấn nút run để chạy và kết quả trả về hiển thị trên Graph theo thời gian thực.

Kết quả đồ thị được biểu diễn bởi 4 đường màu như sau:
Black: The total number of current samples sent.
Blue: The current average of all samples sent.
Red: The current standard deviation.
Green: Throughput rate that represents the number of requests per minute the server handled

![image](https://github.com/7gr4g0n338/Tester/assets/95563870/577fc0d3-8a47-4eb2-9b06-e532b45c1281)

Để phân tích hiệu năng của web server thì nên tập trung vào 2 tham số là throughput và deviation.

throughput đại diện cho khả năng mà máy chủ xử lý tải nặng. throughput càng cao thì hiệu năng càng tốt.
deviation là độ lệch, độ lệch càng nhỏ càng tốt.

