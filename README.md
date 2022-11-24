# CNPM_QuanLyDeTai_N6

Nguyễn Duy Đăng - 20110632
Mai Bảo Huy - 20110649
Đặng Văn Tuấn – 20110300


ĐỀ TÀI: Xây dựng "Website Đăng ký đề tài khoa CNTT" dựa trên nền tảng ASP.NET MVC


Ngày 1: Tìm hiểu Mô hình MVC và ASP.NET
1. Tìm hiểu mô hình MVC là gì?
MVC là viết tắt của cụm từ “Model-View-Controller“. Đây là mô hình thiết kế được sử dụng trong kỹ thuật phần mềm. MVC là một mẫu kiến trúc phần mềm để tạo lập giao diện người dùng trên máy tính. MVC chia thành ba phần được kết nối với nhau và mỗi thành phần đều có một nhiệm vụ riêng của nó và độc lập với các thành phần khác. Tên gọi 3 thành phần:
• Model (dữ liệu): Quản lí xử lí các dữ liệu.
• View (giao diện): Nới hiển thị dữ liệu cho người dùng.
• Controller (bộ điều khiển): Điều khiển sự tương tác của hai thành phần Model và View.
Model (M)
Model chứa một cấu trúc dữ liệu có chức năng lưu trữ toàn bộ các thông tin dữ liệu của một ứng dụng. Trong mô hình MVC thì Model đóng vai trò kết nối cho 2 thành phần View và Controller. 
Đối với Model được thiết lập như một cơ sở dữ liệu hoặc đơn giản hóa như một file XML thông thường. Khi thiết lập thành phần model thì lập trình viên cần đảm bảo các thao tác với cơ sở dữ liệu như các hoạt động xem, truy xuất hoặc xử lý dữ liệu trong ứng dụng.
View (V)
View là thành phần liên quan đến giao diện của ứng dụng khi người dùng trải nghiệm. Thông qua dữ liệu của MVC , người dùng sẽ thực hiện các thao tác tìm kiếm, sử dụng thông tin website, ứng dụng.
Thành phần View được ứng dụng nhiều trong quá trình lập trình website và đây cũng là nơi mà các thành HTML tạo ra. Chức năng khác của thành phần View này chính là khả năng ghi nhận hành vi của người dùng để tương tác được với Controller. View sẽ có nhiệm vụ hiển thị yêu cầu chuyển đến cho Controller xử lý thông tin.
Controller (C)
Controller là bộ phận sẽ xử lý các yêu cầu khi người dùng thao tác trên ứng dụng thông qua thành phần view. Lúc này, Controller sẽ thực hiện truy vấn và xuất dữ liệu phù hợp với yêu cầu của người dùng. Và để làm được điều đó controller còn có cần phải nối được với model để lấy dữ liệu.
• Luồng đi trong mô hình MVC
Khi người dùng thực hiện thao tác trên ứng dụng hoặc website thì từ máy Client sẽ gửi yêu cầu đến server (máy chủ). Lúc này, controller sẽ tiến hành tiếp nhận và xử lý yêu cầu. Một vài trường hợp cần truy xuất dữ liệu thì controller sẽ kết nối với Model để hỗ trợ database.

Sau khi Controller xử lý xong các yêu cầu thì kết quả sẽ được chuyển về View. Lúc này View sẽ tiến hành tạo các mã HTML để trả về giao hiện của trình duyệt kết quả theo yêu cầu của người dùng.

• Ưu điểm
Kiểm tra dễ dàng: Các thành phần độc lập giúp người lập trình dễ kiểm soát và khắc phục các vấn đề, lỗi phát sinh trước khi hoàn thiện sản phẩm đến người dùng.
Chức năng control: Khi kết hợp với các loại ngôn ngữ lập trình thông dụng như CSS<HTML, Javascript thì mô hình MVC là sự hỗ trợ đóng vai trò tối ưu bộ control trên nền tảng ngôn ngữ lập trình.
View và size: MVC giúp tối ưu diện tích băng thông khi sử dụng tránh trường hợp khi nhiều yêu cầu được thực hiện cùng lúc sẽ tạo ra nhiều tệp với dung lượng lớn ảnh hưởng trực tiếp đến đường truyền mạng.
Chức năng Soc (Separation of Concern): Cho phép phân loại các thành Model, View, Database,… để dễ quản lý và kiểm soát hơn.
Tính kết hợp: Người lập trình có thể kết hợp mô hình MVC trên nhiều nền tảng website/ ứng dụng khác nhau giúp tiện lợi hơn khi viết code và giảm tải dung lượng.
Kết cấu khá đơn giản: Phù hợp cho nhiều đối tượng sử dụng khi có nhu cầu lập trình website hoặc các loại ứng dụng.
• Nhược điểm
Đối với mô hình MVC có tính phân tách cao giữa các thành phần nên phù hợp để ứng dụng trong các dự án lớn. Nếu ứng dụng MVC trong các dự án nhỏ sẽ dễ gặp tình trạng cồng kềnh, tốn nguồn lực khi phát triển dự án. Đồng thời, thời gian trung chuyển dữ liệu cũng là điều cần cân nhắc khi thực hiện dự án nhỏ.
Ứng dụng của mô hình MVC trong lập trình
Đối với mỗi mục đích nghề nghiệp của người lập trình viên sẽ có những lựa chọn về ngôn ngữ lập trình cũng như framework lập trình khác nhau. 
Tuy nhiên theo nhận định và đánh giá từ chuyên môn thì nếu các người lập trình có mong muốn phát triển nghề nghiệp của mình thì MVC dưới dạng kiến trúc là một lựa chọn đáng để cân nhắc sử dụng.
• Cách sử dụng mô hình MVC hiệu quả
Vậy cách sử dụng hiệu quả mô hình MVC là gì? Dưới đây là ví dụ hiển thị của một website sử dụng mô hình MVC hiệu quả.
Ví dụ: Ứng dụng Car Clicker được thiết lập để dành cho những cuộc bình chọn về xe hơi. Trên website này các thành phần được thể hiện rõ và hoạt động độc lập với nhau. 
Đại diện cho Model( M) là dữ liệu nhiều mẫu xe hơi được liệt kê.
Controller: là các bộ đếm click chuột có trên website.
View: Hiển thị hình ảnh chiếc xe mà người dùng chọn.
2. ASP.NET
2.1. ASP.NET là gì?
     ASP. NET là một mã nguồn mở dành cho web được tạo bởi Microsoft. Hiện mã nguồn này chạy trên nền tảng Windows và được bắt đầu vào đầu những năm 2000.
     ASP.NET cho phép các nhà phát triển tạo các ứng dụng web, dịch vụ web và các trang web động.
     Phiên bản ASP.NET đầu tiên được triển khai là 1.0 được ra mắt vào tháng 1 năm 2002 và hiện nay, phiên bản ASP.NET mới nhất là 4.6. ASP.NET được phát triển để tương thích với giao thức HTTP. Đó là giao thức chuẩn được sử dụng trên tất cả các ứng dụng web.
     
     ASP.NET được biên dịch dưới dạng Common Language Runtime (CLR), có khả năng hỗ trợ các lập trình viên viết mã ASP.NET với bất kỳ ngôn ngữ nào được hỗ trợ bởi.NET language, ví dụ: C#, VB.Net và J#,...
2.2. ASP.NET core là gì?
     ASP.NET Core là một phiên bản mới của ASP.NET chạy trên mọi nền tảng mọi máy tính, bao gồm Windows, MacOS và Linux. Giống như ASP.NET, nó là mã nguồn mở, được tạo bởi Microsoft. Mã nguồn cho phép các nhà phát triển tạo app, dịch vụ web và các trang web động.
     
     Được phát hành lần đầu tiên vào năm 2016, ASP.NET Core tương đối mới, nhưng đã nhận được cập nhật bản 2.0. Hiện là một giải pháp thay thế ổn định cho các ứng dụng web ASP.NET được lưu trữ trên Windows. 
     
     Các nhà phát triển cho biết, ngôn ngữ ASP.NET có thể tận dụng kiến ​​thức hiện có về C#. Nó có thể nhanh chóng nhận ra những khác biệt về mã nguồn được giới thiệu trong ASP.NET Core.
     
2.3. Cấu trúc và những thành phần của ASP.NET
Dưới đây là những phân tích về cấu trúc thành phần của ASP.NET là gì, nó bao gồm những yếu tố: Ngôn ngữ, thư viện và thời gian chạy CLR. 
• Language/Ngôn ngữ: Là tập con của .NET Framework, tại đây có rất nhiều ngôn ngữ lập trình khác nhau phải kể đến như C#, VB.net, PHP, JavaScript,… Trong đó C# và VB.net được sử dụng phổ biến nhất trong ứng dụng phát triển ứng dụng web. 
• Library/Thư viện: .ASP. NET Framework gồm có một bộ các lớp library chuẩn. Web library là thư viện được dùng phổ biến nhất cho các ứng dụng web. Web library bao gồm tất cả các thành phần cần thiết sử dụng trong phát triển các ứng dụng web-based.
• Common Language Runtime/Thời gian chạy CLR: CLR là một trong các cơ sở hạ tầng của phần đông các kiểu ngôn ngữ lập trình phổ thông. Trong đó, CLR thực hiện các tác vụ chính để xử lý các trường hợp đặc biệt và thu gom rác.
     

     Ngày 2. Làm giao diện
     1. Header
     2. Home
     3. Login
