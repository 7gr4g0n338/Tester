# Who is Software Tester?
5-W question and various advices:
+ what is the job goal?
+ what is the jobs of ST will be done in the SDLC process?
+ what skill does a ST must have?
+ what document does a ST need read?
+ what tool does s ST need study?
+ advices from experience ST.


## I. Software Tester(ST)
1. là 1 cá nhân mà thực hiện `kiểm tra phần mềm như bugs, errors, khiếm khuyết hoặc bất kì các vấn đề nào` mà có thể ẢNH HƯỞNG TỚI HIỆU SUẤT của phần mềm tính toán hoặc của 1 ứng dụng.

2. ST là 1 phần của team phát triển phần mềm và thực hiện kiểm tra các functions or non-functions của phần mềm sử dụng các kĩ thuật kiểm tra phần mềm auto hoặc manual.

3. 1 số các kĩ thuật mà ST có kinh nghiệm bao gồm:
  + Unit testing
  + System testing
  + Black box testing
  + Load testing
  + User acceptance testing (UAT)
  + Scalability testing

4. Overall picture
   
Levels of application quality assurance: Quality assurance - QA, Quality Control - QC and Tesing.
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/1a930c3e-9ee4-44bb-b313-1430d6ed1d67)
Có 3 quá trình gồm QA, QC, Testing làm việc cùng nhau để đảm bảo chất lượng tổng thể của phần mềm và cung cấp sản phẩm đáng tin cậy tới các người dùng cuối.

a. QA - Quality Assurance: xảy ra ở `tất cả các quá trình của software life cycle` và bao gồm `thiết lập các thủ tục` mà bao phủ tất cả các trạng giai đoạn từ giai đoạn requirement analyze tới tesing, release và post-release maintenance.

b. QC - Quality Control: là 1 phần của quá trình QA chịu trách nhiệm cho việc `phân tích kiểm tra các kết quả, xác minh và sửa lỗi`. QC bắt đầu trong suốt giai đoạn `tesing phase của software life cycle` và `tập trung vào xác minh 1 sản phẩm cụ thể`. QC bao gồm nhiều quy trình như `code analysis, technical reviews, design analysis, testing ...`.

Ví dụ các tiến trình của QC:
=> Mục đích chính của QC là đảm bảo các sản phẩm được phát triển đáp ứng `mức độ chất lượng được công bố và yêu cầu của khách hàng`.
  + Kiểm tra xem sản phẩm có tuân thủ với các requirement được thiết lập.
  + Xác minh việc tuân thủ của sản phẩm với các tiêu chuẩn chất lượng được thiết lập.
  + Đánh giá xem liệu sản phẩm có sẵn sàng để release.
  + Xác định các khiếm khuyết nghiêm trọng.

c. Testing bao gồm các hành động sau:
+ Thực thi các test scenarios để xác minh các chức năng của ứng dụng.
+ Xác định các khiếm khuyết và ghi chúng vào giải pháp.
+ Kiểm tra hiệu năng của ứng dụng dưới nhiều điều kiện.
+ Đánh giá độ tin cậy và tính ổn định của sản phẩm.


## II. How to ST join a SDLC development software process?

Model-V framework
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/55e53e1f-be0b-4018-90db-c21dec722417)

Chi tiết:
+ The test cases for User Acceptance Testing (UAT) are created based on the `business requirements`.
+ The test cases for the System Integration Testing (SIT) are based on the `functional requirements`. Normally, this can be done while progammers are busy coding.
+ The test cases for the Unit Testing (done by the developers themselves) are based on the `technical specifications`.

Các việc mà ST cần làm trong các giai đoạn của SDLC ( các giai đoạn SDLC gồm: Requirement Analysis - Design - Development - Testing - Maintenance):

1. Requirement Analysis - ứng với giai đoạn initial stage of development in SDLC.
=> mục đích để xác định các `mâu thuẫn và sự xung đột tiềm năng` trong các yêu cầu để tránh các hiểu lầm về sau:
  + đọc tài liệu, thông số kĩ thuật và giao tiếp với development team để hiểu những gì cần để triển khai.

ví dụ: nếu phát triển 1 ứng dụng cửa hàng online thì ST cần đảm bảo rằng các yêu cầu chứng năng như `thêm mặt hàng` hoặc `thanh toán` phải rõ ràng và được định nghĩa tốt.

2. Test Planning - ứng với giai đoạn Testing in SDLC
=> Mục đích test plan để định nghĩa các `chiến lược và hướng tiếp cận` cho việc kiểm tra:
  + xác định các loại kiểm tra sẽ được thực hiện.
  + các khía cạnh nào của ứng dụng sẽ được verify.
  + thiết lập các tiêu chí để hoàn thành kiểm tra thành công.

ví dụ: Kiểm tra function để check các hoạt động đúng đắn của các loại tính năng lưu trữ khác nhau và kiểm tra performance để đánh giá làm như thế nào hệ thống sử lí lượng lớn các người dùng đồng thời.

3. Creating Test Scenarios - ứng với giai đoạn Testing in SDLC
=> Mục đích để phát triển `chi tiết các hướng dẫn và kịch bản` để test:
  + định nghĩa các bước để thực thi xác minh mỗi chức năng và khía cạnh của ứng dụng.

ví dụ: với chức năng user register, ST tạo kịch bản test mà liên quan tới dữ liệu đầu vào, nút bấm và xác minh rằng thông tin được lưu trữ đúng trong database.

4. Test Execution - ứng với giai đoạn Testing in SDLC
=> Mục đích để `chạy các kịch bản test và ghi lại kết quả`:
  + Tích cực tìm kiếm các khiếm khuyết và vấn đề trong ứng dụng, tài liệu để sửa lỗi.

ví dụ: với chức năng của nút bấm add to cart không hoạt động, ST cần log lại khiếm khuyết này và thông báo tới development team để fix bug.

5. Results Analysis - ứng với giai đoạn Testing in SDLC
=> Mục đích để `phân tích và so sánh` kết quả thực thi test với đầu ra mong đợi từ requirements và test plan:
  + Xác định các khiếm khuyết và phân loại mức độ ưu tiên và quan trọng của chúng đối với sự phát triển
  + Nếu phát hiện 1 khiếm khuyết nghiêm trọng mà cản trở việc hoàn thành dự án thì ST chủ động thảo luận vấn đề này với development team và giúp ưu tiên fix nó.


## III. What skill does a ST must have?
1. 


## Some advices of experience ST:
+ build good relationship with developer to aske them: họ đang cố gắng làm gì, hiểu các bước và đặt thêm cho họ các câu hỏi => giúp fix bug 1 cách nhanh chóng.
+ xây dựng 1 sở thích chung để upgrade mối quan hệ, từ đó có sự tin tưởng và gắn kết trong cả công việc và cuộc sống.

  
