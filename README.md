# Sports-Center-Management-System
Sports Center Management System

REVIEW 1 DOCUMENT
Project: Sports Center Management System
1. Scope & Major Features
Dự án: Sports Center Management System (Hệ thống Quản lý Trung tâm Thể thao)
1.1 TỔNG QUAN PHẠM VI (SCOPE OVERVIEW) Dự án tập trung xây dựng một hệ thống Web Application nhầm số hóa quy trình vận hành của trung tâm thể thao. Hệ thống bao phủ 3 luồng nghiệp vụ cốt lõi: Quản lý Hồ sơ & Gói tập, Đặt lịch & Điểm danh, Thanh toán & Báo cáo. Hệ thống phục vụ 3 đối tượng người dùng chính với ranh giới phân quyền rõ ràng:
Center Manager: Quản lý toàn bộ hệ thống, nhân sự, gói tập, phê duyệt giao dịch và xem báo cáo thống kê.
Coach: Huấn luyện viên, quản lý lịch giảng dạy cá nhân, điểm danh và đánh giá học viên.
Member: Học viên, chủ động sử dụng dịch vụ đặt lớp, thanh toán trực tuyến và quản lý tài khoản cá nhân.
1.2 CHI TIẾT CÁC LUỒNG NGHIỆP VỤ BẮT BUỘC (MUST-HAVE FLOWS) Dự án cam kết hoàn thiện các module tính năng sau để đảm bảo hệ thống có thể vận hành cơ bản:
Flow 1: User & Membership Management (Quản lý Người dùng & Gói tập)
Quản lý người dùng & Phân quyền:
Manager: Quản lý danh sách thành viên và huấn luyện viên. Phân quyền truy cập hệ thống. Hỗ trợ tra cứu thông tin và tạo tài khoản trực tiếp cho thành viên mới nếu khách không tự đăng ký.
Member: Chủ động đăng ký tài khoản mới và cập nhật thông tin cá nhân.
Quản lý Gói tập (Membership Package):
Manager: Quản lý danh mục các gói thành viên (tạo mới, cập nhật giá, thiết lập thời hạn sử dụng). Kiểm tra trạng thái gói tập của toàn bộ hội viên.
Member: Xem danh sách các gói thành viên hiện có, tự thực hiện đăng ký hoặc gia hạn gói tập. Hệ thống tự động gửi thông báo khi gói tập sắp hết hạn.
Flow 2: Class Booking & Schedule Management (Quản lý Lịch & Đặt lớp)
Thiết lập Lịch hoạt động:
Manager: Quản lý danh sách các lớp học, bộ môn, phòng tập và lịch hoạt động chung. Phân công Huấn luyện viên phụ trách từng lớp học.
Nghiệp vụ Đặt lớp (Booking):
Member: Xem danh sách các lớp học và lịch học chung. Xem thông tin huấn luyện viên. Tiến hành đăng ký (Book) hoặc hủy đăng ký lớp học. Hệ thống sẽ kiểm tra tự động trạng thái thẻ và số lượng slot trống trước khi cho phép đặt.
Nghiệp vụ Theo dõi & Điểm danh:
Coach: Xem lịch dạy cá nhân và danh sách học viên trong các lớp mình phụ trách. Tiến hành điểm danh học viên trong từng buổi tập. Ghi nhận kết quả tập luyện và đánh giá tiến độ của học viên.
Member: Xem lịch tập cá nhân, lịch sử điểm danh. Xem kế hoạch tập luyện và nhận xét từ huấn luyện viên.
Flow 3: Payment & Report Management (Thanh toán & Báo cáo)
Nghiệp vụ Thanh toán:
Member: Chủ động thanh toán mua gói tập trực tuyến thông qua cổng thanh toán mô phỏng (hoặc chuyển khoản).
Manager: Ghi nhận, đối soát và phê duyệt các khoản thanh toán thủ công (tiền mặt/chuyển khoản) từ khách hàng. Thực hiện xuất hóa đơn trên hệ thống để kích hoạt gói tập.
Báo cáo Thống kê:
Manager: Xem Dashboard thống kê bao gồm: số lượng thành viên, tình trạng đăng ký lớp học (tỷ lệ lấp đầy), và báo cáo doanh thu theo thời gian.
Hỗ trợ Khách hàng:
Manager: Tiếp nhận và xử lý các yêu cầu hỗ trợ, khiếu nại từ thành viên.
Coach: Gửi thông báo chung hoặc bài tập về nhà cho học viên lớp mình phụ trách.
1.3 GIỚI HẠN DỰ ÁN (OUT-OF-SCOPE / OPTIONAL FLOWS)
Flow 4 (Training and attendance management): Các tính năng nâng cao về tạo kế hoạch tập luyện cá nhân cho Member.
Flow 5 (AI workout recommendation): Tích hợp AI để tự động gợi ý bài tập phù hợp dựa trên mục tiêu, trình độ và lịch sử tập luyện của học viên.
Flow 6 (AI assistant): Tích hợp chatbot AI để Member gửi câu hỏi về lịch tập, bài tập hoặc các dịch vụ của trung tâm.
Thiết bị phần cứng: Không tích hợp hệ thống phần cứng (như máy quẹt thẻ, cổng từ điểm danh).
2. Project Team
Roll Number
Full Name
Email
Group
Role
SE183405
Phạm Minh Hoàng
HoangPMSE183405@fpt.edu.vn
3
Frontend (FE)
SE181722
Phạm Hữu Tiến
TienPHSE181722@fpt.edu.vn
3
Backend (BE)
SE184478
Võ Tấn Triều
TrieuVTSE184478@fpt.edu.vn
3
Frontend (FE)
SE193478
Nguyễn Anh Khoa
nguyenanhkhoa20055@gmail.com
3
Backend (BE)
SE192928
Tô Trọng Tuấn
totrongtuan11b6@gmail.com
3
Backend (BE)



3. Technology
Category
Technology / Tools
Purpose
Frontend
ReactJS, HTML/CSS, Tailwind CSS
Build User Interface (Single Page App) for all user roles.
Backend
Java Spring Boot (or Node.js/C#)
Handle business logic, build RESTful APIs, and connect to the database.
Database
MySQL (or SQL Server)
Store structured system data (Accounts, Memberships, Bookings, etc.).
Version Control
Git, GitHub / GitLab
Store source code and support teamwork/collaboration.
Deployment
Vercel (FE), Render/Railway (BE)
Host the application on a live internet environment for Demo purposes.



4. System Reference
System Name
Platform Type
Area of Reference
Mindbody
Global Web/App
Tham khảo quy trình đặt lịch, quản lý gói hội viên và luồng vận hành chuẩn quốc tế. 
GymMaster
Gym Management Software
Tham khảo phân quyền vai trò và tính năng quản lý khách hàng tại quầy. 
California Fitness & Yoga
Commercial App
Tham khảo trải nghiệm người dùng (UX/UI) và dịch vụ hội viên thực tế tại Việt Nam. 



5. Business Process - Core Flows
A. Quy trình bắt buộc (Must Have - Core Flows)
5.1 Quản lý Người dùng & Gói hội viên (User & Membership Management)
Bước 1 - Khởi tạo tài khoản: Hội viên truy cập trang web và tự đăng ký tài khoản (Hoặc Manager cấp tài khoản nếu khách có yêu cầu).
Bước 2 - Chọn & Đăng ký gói tập: Hội viên xem danh sách dịch vụ, chọn gói tập phù hợp và tiến hành tạo đơn hàng đăng ký/gia hạn.
Bước 3 - Kích hoạt dịch vụ: Sau khi thanh toán thành công (online hoặc được Manager phê duyệt thủ công), hệ thống tự động kích hoạt trạng thái gói hội viên để người dùng bắt đầu sử dụng.
5.2 Quản lý Đặt lịch & Lớp học (Class Booking & Schedule Management)
Bước 1 - Lập lịch lớp (Manager): Quản lý tạo lớp học mới, gán bộ môn, phân công HLV phụ trách và cài đặt giới hạn số lượng người tham gia (Slot).
Bước 2 - Tra cứu lịch học: Hội viên đăng nhập, xem danh sách các lớp học đang mở trên hệ thống.
Bước 3 - Đặt chỗ (Booking):
Hội viên chủ động bấm "Đặt chỗ" trên hệ thống.
Hệ thống kiểm tra thẻ (còn hạn) và slot trống. Nếu hợp lệ, ghi nhận thành công và giảm đi 1 suất của lớp đó.
Bước 4 - Hủy đặt chỗ (Cancellation): Hội viên có thể tự hủy đặt lớp trước thời gian quy định, hệ thống tự động nhượng lại chỗ trống cho người khác đăng ký.
5.3 Quản lý Thanh toán & Báo cáo (Payment & Report Management)
Bước 1 - Tạo hóa đơn: Hệ thống tự động sinh hóa đơn chờ thanh toán khi hội viên đăng ký mua/gia hạn gói tập.
Bước 2 - Xác nhận thanh toán: Hội viên thanh toán online (tự động cập nhật), hoặc nếu thanh toán tiền mặt/chuyển khoản, Manager sẽ kiểm tra đối soát và bấm xác nhận "Đã thanh toán" trên hệ thống.
Bước 3 - Lưu trữ đối soát: Toàn bộ lịch sử giao dịch được lưu trữ an toàn, minh bạch.
Bước 4 - Thống kê & Báo cáo (Manager): Quản lý theo dõi tổng doanh thu, tình hình hội viên mới và tỷ lệ lấp đầy các lớp qua biểu đồ trực quan trên Dashboard.
B. Quy trình nâng cao & Tích hợp AI (Nice to Have - Optional Flows)
5.4 Quản lý Điểm danh & Tiến trình Tập luyện (Training & Attendance Management)
Điểm danh lớp học (Coach): Khi đến giờ học, HLV mở danh sách lớp trên hệ thống và tiến hành điểm danh thực tế hội viên có mặt.
Ghi nhận & Đánh giá (Coach): Sau buổi tập, HLV cập nhật nhận xét, giao bài tập về nhà và nhập chỉ số cơ thể cho hội viên.
Theo dõi kết quả (Member): Hội viên truy cập để xem đánh giá từ HLV và theo dõi biểu đồ tiến trình thay đổi cơ thể của mình.
5.5 Gợi ý bài tập thông minh (AI Workout Recommendation)
Phân tích thông tin: HLV chọn thông tin hội viên (mục tiêu tập luyện, trình độ hiện tại, lịch sử tập).
Sinh kế hoạch tập (AI): Hệ thống gọi API AI tự động phân tích và đề xuất lịch trình/bài tập cá nhân hóa.
Duyệt & Áp dụng (Coach): HLV kiểm tra, tùy chỉnh kế hoạch nếu cần và lưu lại để hội viên thực hiện.
5.6 Trợ lý ảo Hội viên (AI Assistant)
Gửi câu hỏi (Member): Hội viên nhắn tin vào khung chat hỏi AI về lịch học, hướng dẫn bài tập hoặc giá dịch vụ.
Phản hồi tự động (AI): Trợ lý ảo AI trả lời tự động ngay lập tức 24/7, thay thế nhân sự tư vấn.
