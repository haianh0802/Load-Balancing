### Load Balancing là gì?

Load Balancing là tính năng giúp máy chủ ảo hoạt động đồng bộ và hiệu quả hơn thông qua việc phân phối đồng đều tài nguyên.

Load balancing (cân bằng tải) được định nghĩa là phân phối lưu lượng truy cập mạng hoặc ứng dụng một cách có hiệu quả trên nhiều server trong một cụm server farm.

Load balancing (cân bằng tải) phân phối đồng đều tài nguyên trên nhiều máy chủ. Kỹ thuật này giúp giảm thời gian phản hồi, tăng (throughput) năng suất truyền tải và nói chung tăng tốc độ truy xuất dữ liệu cho mỗi khách hàng. Bằng cách áp dụng giải pháp này, đem đến việc cân bằng khi lưu lượng truy cập được chia đều lên các server hoặc khi server gặp sự cố, server còn lại ngay lập tức là phương án hỗ trợ, không làm gián đoạn sự truy cập và hoạt động của doanh nghiệp.

### Load balancer hoạt động như thế nào?

Các website hiện đại có lưu lượng truy cập cao phải phục vụ hàng trăm nghìn, thậm chí hàng triệu các requests đồng thời từ người dùng hoặc khách hàng, đồng thời phải phản hồi chính xác lại các văn bản, hình ảnh, video hoặc dữ liệu ứng dụng, tất cả đều được thực hiện rất nhanh chóng và đáng tin cậy. Để đáp ứng hiệu quả khối lượng lớn các yêu cầu và phản hồi một cách tiết kiệm nhất, best practice tốt nhất thường sẽ là sử dụng thêm servers.

Một load balancer (Cân bằng tải) hoạt động như "traffic cop" (cảnh sát giao thông) ngồi ở phía trước server và routing các request của client trên tất cả các server có khả năng thực hiện các request đó, sao cho tối ưu về tốc độ và hiệu suất nhất và đảm bảo rằng không có server nào phải hoạt động quá mức.

Nếu một server đơn lẻ bị hỏng, cân bằng tải (load balancer) sẽ chuyển hướng lưu lượng truy cập đến các server trực tuyến còn lại. Khi một server mới được thêm vào nhóm máy chủ, bộ cân bằng tải sẽ tự động bắt đầu gửi yêu cầu đến máy chủ mới thêm này.

**Tóm lại, một load balancer sẽ thực hiện các chức năng chính sau đây:** 

- Phân phối lưu lượng đến các server khác nhau trong nhóm tài nguyên để đảm bảo rằng không có server nào bị quá tải. 

- Giảm thiểu thời gian phản hồi của server và tối đa hóa throughput. 

- Cung cấp hiệu suất và bảo mật cần thiết để duy trì các môi trường CNTT, cũng như các quy trình công việc phức tạp diễn ra trong chúng. 

- Khả năng mở rộng nhất để xử lý vô số yêu cầu từ quy trình làm việc đa ứng dụng, đa thiết bị hiện đại. 

- Cho phép truy cập liền mạch vào nhiều ứng dụng, tệp và máy tính để bản khác nhau trong không gian làm việc số ngày nay.

### Các loại Load balancer L4, L7, GSLB

Để thúc đẩy tính nhất quán cao hơn và theo kịp nhu cầu ngày càng tăng của người dùng, tài nguyên server phải có sẵn và cân bằng tải ở Layer 4 hoặc Layer 7 của mô hình Open Systems Interconnection (Liên kết hệ thống mở - OSI): 

- Cân bằng tải Layer 4 (L4) hoạt động ở cấp độ vận chuyển. Điều đó có nghĩa là chúng có thể đưa ra các quyết định định tuyến dựa trên các cổng TCP hoặc UDP mà các gói sử dụng cùng với địa chỉ IP nguồn và đích của chúng. L4 load balancers thực hiện Network Address Translation nhưng không kiểm tra nội dung thực tế từng gói. 

- Cân bằng tải Layer 7 (L7) hoạt động ở cấp ứng dụng, cao nhất trong mô hình OSI. Chúng có thể đánh giá phạm vi dữ liệu rộng hơn so với các đối tác L4, bao gồm các tiêu đề HTTP và ID phiên SSL, khi quyết định cách phân phối các yêu cầu trên toàn bộ cụm máy chủ. Load balancing chuyên sâu hơn về mặt tính toán tại L7 hơn so với L4 và nó cũng có thể hoạt động hiệu quả hơn ở L7, do cấu hình được thêm vào để hiểu và xử lý các yêu cầu của máy khách đến máy chủ. 

Ngoài load balancing L4 và L7 cơ bản, Global server load balancing (cân bằng tải máy chủ toàn cầu – GSLB) có thể mở rộng khả năng của một trong hai loại trên nhiều trung tâm dữ liệu để có thể phân phối lưu lượng lớn một cách hiệu quả.

Khi các ứng dụng ngày các được lưu trữ trong các trung tâm dữ liệu đám mây nằm ở nhiều khu vực địa lý, GSLB cho phép các tổ chức CNTT cung cấp các ứng dụng có độ tin cậy cao hơn và độ trễ thấp hơn cho bất kỳ thiết bị hoặc vị trí nào. Làm như vậy đảm bảo trải nghiệm nhất quán hơn cho end user khi họ đang điều hướng nhiều ứng dụng và dịch vụ trong không gian làm việc số. 

**Một số thuật toán Load balancer (cân bằng tải) phổ biến**

- Round Robin: Round robin là một kỹ thuật vòng tròn đơn giản, giúp đảm bảo rằng các truy vấn dịch vụ sẽ lần lượt được gửi tới các máy chủ theo thứ tự sắp xếp. 

- Least Connection: Load balancer sẽ tìm cách gửi yêu cầu đến server có số lượng kết nối hoạt động ít nhất. Thuật toán này được coi như thuật toán động, vì nó phải đếm số kết nối đang hoạt động của server.

- Least Response Time: Đây là thuật toán dựa trên tính toán vào thời gian mà server thực hiện để đáp ứng cầu nhanh nhất.

- Least Packets: Load balancer sẽ chọn server đã nhận được ít gói tin nhất trong một khoảng thời gian nhất định.

- Hashing: Thuật toán xác định kết nối chính xác từ một IP nguồn/ đích, port number, URL hoặc domain name của máy khách sẽ được kết nối trực tiếp đến một server backend.

- Custom Load: Thuật toán này cho phép bộ cân bằng tải truy vấn tải trên các máy chủ riêng lẻ thông qua SNMP.

**Lợi ích của việc sử dụng load balancer cho server?**

- Uptime 99.9%: Với Load Balancing, khi máy chủ gặp sự cố, lưu lượng truy cập sẽ được tự động chuyển đến máy chủ còn lại. Nhờ đó, trong hầu hết mọi trường hợp, sự cố bất ngờ có thể được phát hiện và xử lý kịp thời, không làm gián đoạn các truy cập của người dùng.

- Datacenter linh hoạt: Khả năng linh hoạt trong việc điều phối giữa các máy chủ cũng là một ưu điểm khác của Load Balancing. Tự động điều phối giữa các máy chủ cũ và mới để xử lý các yêu cầu dịch vụ mà không làm gián đoạn các hoạt động chung của hệ thống.

- Tăng bảo mật cho Datacenter: Bằng cách sử dụng Load Balancing, những yêu cầu từ người dùng sẽ được tiếp nhận và xử lý trước khi phân chia đến các máy chủ. Đồng thời, quá trình phản hồi cũng được thông qua Load Balancing, ngăn cản việc người dùng giao tiếp trực tiếp với máy chủ, ẩn đi thông tin và cấu trúc mạng nội bộ, từ đó chặn đứng những cuộc tấn công mạng hay truy cập trái phép…
Load balancer luôn đóng một vai trò quan trọng trong quá trình hoạt động hiệu quả và giảm thiểu những rủi ro cho doanh nghiệp. Đây một trong những thành phần cơ sở hạ tầng quan trọng nhất của ngành mạng máy tính hiện nay. Hãy đảm bảo sự hài lòng của khách hàng truy cập website bằng cách sử dụng giải pháp Load Balancing này.

**Có 4 loại giao thức chính mà quản trị Load Balancer có thể tạo quy định chuyển tiếp:**

HTTP: dựa trên cơ chế HTTP chuẩn, HTTP Balancing đưa ra yêu cầu tác vụ. Load Balancer đặt X-Forwarded-For, X-Forwarded-Proto và tiêu đề X-Forwarded-Port cung cấp các thông tin backends về những yêu cầu ban đầu.

HTTPS: các chức năng tương tự HTTP Balancing. HTTPS Balancing được bổ sung mã hóa và nó được xử lý bằng 2 cách: passthrough SSL duy trì mã hóa tất cả con đường đến backend hoặc: chấm dứt SSL, đặt gánh nặng giải mã vào load balancer và gửi lưu lượng được mã hóa đến backend.

TCP: trong một số trường hợp khi ứng dụng không sử dụng giao thức HTTP hoặc HTTPS, TCP sẽ là một giải pháp để cân bằng lưu lượng. Cụ thể, khi có một lượng truy cập vào một cụm cơ sở dữ liệu, TCP sẽ giúp lan truyền lưu lượng trên tất cả các máy chủ

UDP: trong thời gian gần đây, Load Balancer đã bổ sung thêm hỗ trợ cho cân bằng tải giao thức internet lõi như DNS và syslogd sử dụng UDP.
Các quy tắc chuyển tiếp sẽ xác định loại giao thức và cổng vào Load Balancer để di chuyển đến các giao thức. Cổng Load Balancer lúc này được sử dụng để định tuyến lưu lượng trên backend.

### Khi nào sử dụng Load balancer (Cân bằng tải)?
Load balancer (Cân bằng tải) đước sử dụng khi website của bạn được triển khai trên nhiều hơn một cloud server.

**Sau đây là 2 khó khăn chính bạn sẽ gặp phải nếu chỉ triển khai website của mình trên một server duy nhất:**

- Không thể đảm bảo xử lý được lượng traffic của một khối lượng user lớn truy cập vào website (đủ lớn để 1 cloud server không thể tải nổi).

Cụ thể, khi hệ thống của bạn có quá nhiều người sử dụng, một server đơn lẻ không thể đáp ứng được lượng requests khổng lồ được gửi đến cùng lúc. Bạn cần chia sẻ công việc của server hiện tại với một hoặc nhiều server khác nữa. Tức là sử dụng nhiều server một lúc, khi này, việc tải dữ liệu từ server nào sẽ do bộ Load balancer (Cân bằng tải)  quyết định.

- Không đảm bảo tính sẵn sàng của dịch vụ doanh nghiệp (nếu chỉ sử dụng duy nhất 1 cloud server, khi cloud server này gặp sự cố, không hề có server nào có thể thay thế tiếp tục các tiến trình đang dang dở, đấn đến website rơi vào tình trạng downtime theo). Gây tổn thất và ảnh hưởng to lớn đến trải nghiệm người dùng, doanh thu, uy tín và hiệu quả hoạt động của doanh nghiệp.

Đó chính là lý do mà chúng ta phải triển khai website trên nhiều cloud server cùng một lúc, bởi vì không có gì đảm bảo cho việc một server sẽ luôn hoạt động trơn tru và hoàn hảo mãi mãi. Bằng cách triển khai nhiều, khi server gặp sự cố, server còn lại ngay lập tức là phương án hỗ trợ, không làm gián đoạn hoạt động của doanh nghiệp. Trên thực tế, những tổn thất do hệ thống thông tin ngừng hoạt động là cực kỳ to lớn và không thể lường trước được.

**Tuy nhiên, khi triển khai website lên nhiều server, hiệu quả là vậy nhưng bạn vẫn chắc chắn sẽ gặp phải các khó khăn tiếp theo sau đây:**

Triển khai nhiều cloud servers, tức đồng thời bạn sẽ sở hữu nhiều địa chỉ của các cloud servers. Trong khi đó, một domain website lại không thể trỏ về nhiều địa chỉ cùng một lúc.

Bạn càng sở hữu nhiều servers, việc quản trị, triển khai và bảo trì càng trở nên phức tạp và khó khăn gấp nhiều lần. Đòi hỏi tính chuyên môn và kĩ thuật cao, chưa kể chi phí cho các thao tác này.

Lúc này, Load balancer (Cân bằng tải) chính là câu trả lời và là giải pháp tuyệt vời có thế giải quyết hoàn hảo triệt để các vấn đề kể trên.
