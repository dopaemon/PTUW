# Web back-end - Web server

## Web server
### Web server là gì
Chúng ta đã biết có 3 cách để tạo ra **một ứng dụng web** là:
* viết thuần từ đầu
* dùng framework
* sử dụng CMS
Dù bạn lựa chọn phương pháp nào thì cũng cần phải có những hiểu biết căn bản về hạ tầng của một ứng dụng web.
Web server là một thành phần của hạ tầng ứng dụng web. Chúng ta cùng tìm hiểu về chủ đề này.

### Web server là gì
**Web server (máy chủ web)** là một thành phần quan trọng trong hạ tầng ứng dụng web, được hiểu theo hai khía cạnh: **phần mềm** chuyên dụng hoặc **máy tính vật lý (phần cứng)** có cài đặt các phần mềm đó để lưu trữ và cung cấp nội dung cho website,.

#### 1. Chức năng cốt lõi
Web server đóng vai trò là trung tâm lưu trữ và điều phối thông tin của ứng dụng web. Các nhiệm vụ chính bao gồm:
*   **Lưu trữ dữ liệu:** Lưu trữ toàn bộ các tập tin cấu thành ứng dụng web như mã nguồn HTML, hình ảnh, video và các dữ liệu khác,.
*   **Tiếp nhận yêu cầu (Request):** Khi người dùng nhập địa chỉ web vào trình duyệt, một yêu cầu sẽ được gửi đến và web server có nhiệm vụ tiếp nhận yêu cầu này,.
*   **Xử lý yêu cầu:** Web server phân tích yêu cầu, thực hiện các tác vụ như đọc tập tin, thực thi mã nguồn hoặc kết nối với cơ sở dữ liệu để lấy thông tin cần thiết,.
*   **Gửi phản hồi (Response):** Sau khi xử lý xong, server gửi kết quả (thường là trang HTML đã có dữ liệu) trở lại trình duyệt để hiển thị cho người dùng,.

#### 2. Quy trình hoạt động của Web server
Quá trình xử lý một yêu cầu từ người dùng diễn ra theo trình tự các bước sau,:
1.  **Nhận request** từ trình duyệt.
2.  **Phân tích request** và gửi tới ứng dụng web để xử lý.
3.  **Truy xuất dữ liệu** từ cơ sở dữ liệu (nếu có yêu cầu).
4.  **Đổ dữ liệu** vào các trang mẫu (template HTML).
5.  **Gửi phản hồi (response)** là trang HTML hoàn chỉnh về trình duyệt.
6.  Trình duyệt **hiển thị nội dung** và có thể gửi thêm các yêu cầu riêng biệt để lấy nội dung tĩnh (CSS, JavaScript, hình ảnh).

#### 3. Đặc điểm về phần cứng và phần mềm
*   **Về phần mềm:** Các phần mềm web server phổ biến hiện nay bao gồm **Apache, Nginx, Nodejs, IIS, Tomcat và Lighttpd**. Các phần mềm này có thể được cấu hình để lắng nghe yêu cầu qua các cổng (port), trong đó cổng mặc định thường là **80**.
*   **Về phần cứng:** Một máy chủ vật lý cần là **máy server chuyên dụng** với cấu hình mạnh mẽ, khả năng chịu lỗi cao và có thể hoạt động liên tục 24/7. Nó sử dụng các hệ điều hành dành riêng cho máy chủ và cài đặt sẵn các trình dịch mã nguồn cũng như hệ quản trị cơ sở dữ liệu.

#### 4. Ví dụ về Nginx
Nginx là một phần mềm web server mã nguồn mở phổ biến. Nó thường chạy dưới dạng một chương trình chạy ngầm (master process và worker process),. Người phát triển có thể cấu hình Nginx thông qua tệp `nginx.conf` để thay đổi cổng lắng nghe hoặc chỉ định thư mục gốc (web root) – nơi chứa các tập tin của ứng dụng web,.

***

Để dễ hình dung, bạn có thể coi **Web server giống như một thủ thư trong một thư viện lớn**:
*   **Thư viện (Phần cứng)** là tòa nhà kiên cố, hoạt động suốt ngày đêm để bảo vệ sách.
*   **Thủ thư (Phần mềm)** là người đứng ở quầy tiếp tân.
*   Khi bạn (Trình duyệt) đến hỏi mượn một cuốn sách (Request), thủ thư sẽ đi tìm sách trên kệ, có khi phải photo hoặc tổng hợp tài liệu từ nhiều nguồn (Xử lý), sau đó mang cuốn sách đó ra giao cho bạn (Response) để bạn đọc.

### Nginx
**Nginx là một phần mềm web server (máy chủ web) mã nguồn mở phổ biến**, được sử dụng rộng rãi để lưu trữ và cung cấp nội dung cho các ứng dụng web,. Cùng với Apache, IIS hay Nodejs, Nginx đóng vai trò là một thành phần quan trọng trong hạ tầng của ứng dụng web.

#### 1. Đặc điểm vận hành
*   **Cơ chế hoạt động:** Nginx chạy dưới dạng một **chương trình (program) chạy ngầm** chứ không phải là một dịch vụ (service). Khi khởi chạy, trong hệ thống sẽ xuất hiện hai tiến trình song song là **master process** và **worker process**.
*   **Cài đặt:** Đối với Windows, Nginx không cần cài đặt phức tạp, người dùng chỉ cần giải nén tập tin vào ổ đĩa (ví dụ `C:\`) và chạy tập tin `nginx.exe`.
*   **Xử lý lỗi:** Mọi thông tin về lỗi trong quá trình khởi chạy hoặc vận hành đều được ghi lại trong tập tin `error.log` nằm tại thư mục `logs`.

#### 2. Các lệnh quản lý cơ bản
Bạn có thể điều khiển Nginx thông qua cửa sổ dòng lệnh (CMD hoặc PowerShell) với các lệnh sau,:
*   `start nginx`: Khởi chạy Nginx.
*   `nginx -s stop`: Dừng Nginx ngay lập tức.
*   `nginx -s quit`: Dừng Nginx một cách an toàn (chờ các tác vụ hiện tại hoàn thành xong mới tắt).
*   `nginx -s reload`: Khởi chạy lại các worker process để **cập nhật cấu hình mới** mà không cần tắt máy chủ.

#### 3. Cấu hình hệ thống (nginx.conf)
Tất cả các thiết lập của Nginx được quản lý trong tập tin `nginx.conf` (thường nằm ở thư mục `conf`). Các thông số quan trọng bao gồm:
*   **Cổng (Port):** Mặc định Nginx lắng nghe các yêu cầu tại cổng **80**. Người dùng có thể tùy chỉnh sang các cổng khác như 9000 hay 65535 tùy theo nhu cầu,.
*   **Web root:** Là thư mục gốc chứa các tập tin của ứng dụng web (mặc định là thư mục `html`).
*   **Trang mặc định:** Khi người dùng truy cập vào địa chỉ web mà không chỉ định rõ tập tin, Nginx sẽ tự động gọi tập tin mặc định là `index.html` hoặc `index.htm`.

#### 4. Quy trình xử lý yêu cầu
Khi bạn truy cập `http://localhost`, trình duyệt sẽ gửi một yêu cầu (request) đến Nginx. Nếu Nginx đang sẵn sàng, nó sẽ tiếp nhận, phân tích yêu cầu, thực hiện xử lý (như đọc tập tin hoặc thực thi mã nguồn) và gửi phản hồi (response) về trình duyệt để hiển thị cho người dùng,.

***

Để dễ hình dung, hãy tưởng tượng **Nginx giống như một người quản lý nhà hàng**: 
*   **Master process** là người quản lý chính, đứng ra điều hành và nhận các chỉ thị mới (như thay đổi thực đơn - reload cấu hình). 
*   **Worker process** là các nhân viên phục vụ trực tiếp bưng bê món ăn (dữ liệu) cho khách hàng (trình duyệt). 
*   **Tập tin `nginx.conf`** chính là cuốn sổ tay quy định về giờ mở cửa (port) và thực đơn chính (web root) của nhà hàng đó.
