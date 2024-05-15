# Who is Software Tester?
5-W question and various advices:
+ what is the job goal?
+ what is the jobs of ST will be done in the SDLC process?
+ what skill does a ST must have?
+ what document does a ST need read?
+ what tool does s ST need study?
+ advices from experience ST.


## I. Software Tester(ST)
### 1. Define
+ là 1 cá nhân mà thực hiện `kiểm tra phần mềm như bugs, errors, khiếm khuyết hoặc bất kì các vấn đề nào` mà có thể ẢNH HƯỞNG TỚI HIỆU SUẤT của phần mềm tính toán hoặc của 1 ứng dụng.

+ là 1 phần của team phát triển phần mềm và thực hiện kiểm tra các functions or non-functions của phần mềm sử dụng các kĩ thuật kiểm tra phần mềm auto hoặc manual.

### 2. Overall picture
   Levels of application quality assurance: Quality assurance - QA, Quality Control - QC and Tesing.
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/1a930c3e-9ee4-44bb-b313-1430d6ed1d67)
Có 3 quá trình gồm QA, QC, Testing làm việc cùng nhau để đảm bảo chất lượng tổng thể của phần mềm và cung cấp sản phẩm đáng tin cậy tới các người dùng cuối.

#### a. QA - Quality Assurance
* xảy ra ở `tất cả các quá trình của software life cycle` và bao gồm `thiết lập các thủ tục` mà bao phủ tất cả các trạng giai đoạn từ giai đoạn requirement analyze tới tesing, release và post-release maintenance.

#### b. QC - Quality Control
* là 1 phần của quá trình QA chịu trách nhiệm cho việc `phân tích kiểm tra các kết quả, xác minh và sửa lỗi`. QC bắt đầu trong suốt giai đoạn `tesing phase của software life cycle` và `tập trung vào xác minh 1 sản phẩm cụ thể`. QC bao gồm nhiều quy trình như `code analysis, technical reviews, design analysis, testing ...`.

Ví dụ các tiến trình của QC:
=> Mục đích chính của QC là đảm bảo các sản phẩm được phát triển đáp ứng `mức độ chất lượng được công bố và yêu cầu của khách hàng`.
  + Kiểm tra xem sản phẩm có tuân thủ với các requirement được thiết lập.
  + Xác minh việc tuân thủ của sản phẩm với các tiêu chuẩn chất lượng được thiết lập.
  + Đánh giá xem liệu sản phẩm có sẵn sàng để release.
  + Xác định các khiếm khuyết nghiêm trọng.

#### c. Testing
+ Thực thi các test scenarios để xác minh các chức năng của ứng dụng.
+ Xác định các khiếm khuyết và ghi chúng vào giải pháp.
+ Kiểm tra hiệu năng của ứng dụng dưới nhiều điều kiện.
+ Đánh giá độ tin cậy và tính ổn định của sản phẩm.

### 3. Teamwork with other members of the development team
+ System Analyst - SA: a translator between the client's requirements and the developers.
+ Business Analyst - BA: uses business analysis methods to investigate business needs, identify business problems, and propose solutions to address them.
+ Product Owner - PO: responsible for envisioning the final product and understanding its value for users.
+ Developer: who masterfully create software by code sources.
+ Project Manager: The tester collaborates with project managers to understand the product requirements and ensure its quality by testing the functionality and fixing errors.

## II. How to ST join a SDLC development software process?

### Model-V framework
![image](https://github.com/7gr4g0n338/Tester/assets/95563870/55e53e1f-be0b-4018-90db-c21dec722417)

Chi tiết:
+ The test cases for User Acceptance Testing (UAT) are created based on the `business requirements`.
+ The test cases for the System Integration Testing (SIT) are based on the `functional requirements`. Normally, this can be done while progammers are busy coding.
+ The test cases for the Unit Testing (done by the developers themselves) are based on the `technical specifications`.

Các việc mà ST cần làm trong các giai đoạn của SDLC ( các giai đoạn SDLC gồm: Requirement Analysis - Design - Development - Testing - Maintenance):

referrence: https://hyperskill.org/learn/step/31958
### 1. Requirement Analysis - ứng với giai đoạn initial stage of development in SDLC.
=> mục đích để xác định các `mâu thuẫn và sự xung đột tiềm năng` trong các yêu cầu để tránh các hiểu lầm về sau:
  + đọc tài liệu, thông số kĩ thuật và giao tiếp với development team để hiểu những gì cần để triển khai.

ví dụ: nếu phát triển 1 ứng dụng cửa hàng online thì ST cần đảm bảo rằng các yêu cầu chứng năng như `thêm mặt hàng` hoặc `thanh toán` phải rõ ràng và được định nghĩa tốt.

### 2. Test Planning - ứng với giai đoạn Testing in SDLC
=> Mục đích test plan để định nghĩa các `chiến lược và hướng tiếp cận` cho việc kiểm tra:
  + xác định các loại kiểm tra sẽ được thực hiện.
  + các khía cạnh nào của ứng dụng sẽ được verify.
  + thiết lập các tiêu chí để hoàn thành kiểm tra thành công.

ví dụ: Kiểm tra function để check các hoạt động đúng đắn của các loại tính năng lưu trữ khác nhau và kiểm tra performance để đánh giá làm như thế nào hệ thống sử lí lượng lớn các người dùng đồng thời.

### 3. Creating Test Scenarios - ứng với giai đoạn Testing in SDLC
=> Mục đích để phát triển `chi tiết các hướng dẫn và kịch bản` để test:
  + định nghĩa các bước để thực thi xác minh mỗi chức năng và khía cạnh của ứng dụng.

ví dụ: với chức năng user register, ST tạo kịch bản test mà liên quan tới dữ liệu đầu vào, nút bấm và xác minh rằng thông tin được lưu trữ đúng trong database.

### 4. Test Execution - ứng với giai đoạn Testing in SDLC
=> Mục đích để `chạy các kịch bản test và ghi lại kết quả`:
  + Tích cực tìm kiếm các khiếm khuyết và vấn đề trong ứng dụng, tài liệu để sửa lỗi.

ví dụ: với chức năng của nút bấm add to cart không hoạt động, ST cần log lại khiếm khuyết này và thông báo tới development team để fix bug.

### 5. Results Analysis - ứng với giai đoạn Testing in SDLC
=> Mục đích để `phân tích và so sánh` kết quả thực thi test với đầu ra mong đợi từ requirements và test plan:
  + Xác định các khiếm khuyết và phân loại mức độ ưu tiên và quan trọng của chúng đối với sự phát triển
  + Nếu phát hiện 1 khiếm khuyết nghiêm trọng mà cản trở việc hoàn thành dự án thì ST chủ động thảo luận vấn đề này với development team và giúp ưu tiên fix nó.


## III. What skill does a ST must have?
### 1. Automation Testing
=> Mục đích: thời gian phản hồi nhanh, giảm thiểu các tác vụ lặp đi lặp lại, nâng cao độ chính xác và loại bỏ lỗi của con người.
+ các công cụ tự động: Selenium, Apache Jmeter, RFT, Appium, Perfecto, Katalon Studio.
+ Các automation tester phải quen thuộc với:
  * ngôn ngữ lập trình được dùng để phát triển ứng dụng
  * các trình duyệt và các yêu cầu thiết bị
  * APIS hoặc bẩt kì dịch vụ web kết nối tới application
  * database được sử dụng để lưu trữ backend
  * làm việc với tất cả các module và tính năng trong application
  * xác định các khu vực mà không thể automatic testing mà cần phải manual testing
  * lên kế hoạch quản lí thời gian hiệu quả
  * liệu có bất kì khiếm khuyết nào trong lần cuối phát hành hoặc được mong đợi sửa trong lần release này không?

### 2. Proficiency in Programming Languages
Có kiến thức lập trình giúp nâng cao kỹ năng kiểm tra tự động và giao tiếp hiệu quả với developer.

### 3. Knowledge of Test Management Tools
=> Mục đích: giúp tránh các lỗi bắt gặp trong quá trình sản xuất.
các công cụ quản lí kiểm thử:
+ TestRail
+ TestPad
+ QADeputy
+ TestLink

### 4. Knowledge of SDLC and Agile Methodology
SDLC gồm 1 số phương thức phát triển như: Scrum, Kanban, Waterfall.

Agile methodology là 1 phương thức quản lí dự án nhằm chia các bước nhỏ hơn nhằm thúc đẩy sự linh hoạt và hợp tác trong kiểm tra phần mềm.
các công cụ Agile testing:
+ Selenium web driver
+ JunoOne
+ JIRA
+ Appium

### 5. Analytical Skills Critical 
Giúp các ST chia 1 hệ thống phức tạp thành các phần nhỏ, quản lí các thành phần, hiểu rõ code và xác định các rủi ro tiềm năng. Giúp việc thiết kế các test case tốt hơn và nâng cao toàn bộ năng suất của hệ thống.

### 6. Excellent Communication Skills
giao tiếp rõ ràng và mạch lạc để khảo sát các developer, PM, BA và đồng nhất các ý tưởng, ý kiến.

### 7. Project management skills

## IV. What document does a ST need read?
Tầm quan trọng của tài liệu cho các tester và việc kiểm tra:
+ là 1 phần quan trọng trong việc định nghĩa của ta về sự hoàn thành công việc.
+ loại bỏ những hiểu lầm và sự bối dối giữa các testing phase
+ giúp tiết kiệm thời gian bằng sự rõ ràng của các task cần hoàn thành
+ ghi lại được các sự thay đổi đã làm
+ các thành viên mới của team có thể tăng tốc độ test với từng giai đoạn
+ cung cấp tài liệu khi được khách hàng yêu cầu

### 1. What documentation do QA teams use?
* Test case:
   * là 1 bản mô tả chi tiết chính xác các bước mà 1 tester cần để thông qua đánh giá các function của 1 tính năng cụ thể. Ví dụ như các tiêu chí để đạt được yêu cầu pass. 
   * là 1 bản chuẩn hóa cho các tester khác nhau tiến hành kiểm tra cùng phần mềm.

* Test plan:
   * là việc tổng quát hóa tất cả các hành động liên quan tới giai đoạn kiểm thử: bao gồm các scope kiểm thử, kế hoạch, các tài nguyên để cung cấp cái nhìn high-level cho việc tiến hành kiểm thử.

* Test scenario:
   * làm rõ các phương thức kiểm thử phần mềm sẽ được sử dụng để đưa ra các test case phù hợp. Ví dụ: xác định việc làm như thế nào mà người dùng có thể lạm dụng hệ thông và lên kế hoạch test đầu ra phù hợp.

* Test report:
   * là bản ghi trạng thái của mỗi test case đã được chạy, do đó ta có thể quay trở lại đầu ra của mỗi lần test >< defect report ghi lại các tính năng phần mềm bị lỗi.
 
* Checklist:
   *  tương tự/thay thế cho test case, chúng cung cấp 1 danh sách các tính năng phần mềm mà các tester cần phân tích, cùng với mô tả về chức năng và đầu ra của việc kiểm thử.

* Bug report:
   * là bản ghi của bất kì lỗi nào được phát hiện trong quá trình kiểm thử. Nó ghi rõ chi tiết các ảnh hưởng của bug lên hệ thống và gợi ý ưu tiên fix chúng.
 
* Requirements:
   * là 1 bản mô tả đầy đủ các chức năng và tính năng của phần mềm được xây dựng để đảm bảo rằng tất cả các team nắm được thông tin đầy đủ về product.



## Some advices of experience ST:
+ build good relationship with developer to aske them: họ đang cố gắng làm gì, hiểu các bước và đặt thêm cho họ các câu hỏi => giúp fix bug 1 cách nhanh chóng.
+ xây dựng 1 sở thích chung để upgrade mối quan hệ, từ đó có sự tin tưởng và gắn kết trong cả công việc và cuộc sống.

  
