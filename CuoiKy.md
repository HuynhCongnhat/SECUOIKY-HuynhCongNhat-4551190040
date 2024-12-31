# Bài tập đánh giá kết thúc học phần

## I. Phân tích bài toán

### Các chức năng chính của hệ thống:
- **Nhập dữ liệu giao dịch**: Cho phép người dùng nhập các file dữ liệu giao dịch từ các nguồn khác nhau (như file CSV, Excel, PDF).
- **Phân tích dữ liệu giao dịch**:
  - Tổng hợp các giao dịch theo các tiêu chí khác nhau.
  - Tính toán các chỉ số thống kê.
- **Báo cáo và hiển thị kết quả**:
  - Tạo các báo cáo thống kê theo yêu cầu của người dùng.
  - Hiển thị kết quả phân tích dưới dạng biểu đồ, bảng biểu.
- **Lưu trữ kết quả**:
  - Lưu trữ các báo cáo và kết quả phân tích vào thiết bị lưu trữ của người dùng.
  - Cho phép người dùng tải xuống hoặc in các báo cáo.
- **Quản lý người dùng và quyền truy cập**:
  - Đăng ký, đăng nhập, quản lý thông tin người dùng.
  - Phân quyền truy cập cho các chức năng khác nhau của hệ thống.

### Các tác nhân liên quan đến hệ thống:
- **Khách hàng (Người dùng)**: Người sử dụng hệ thống để nhập dữ liệu, phân tích giao dịch và xem báo cáo.
- **Quản trị viên hệ thống**: Người quản lý hệ thống, thiết lập các cấu hình ban đầu và xử lý các vấn đề kỹ thuật.
- **Ngân hàng**: Nguồn cung cấp dữ liệu giao dịch thông qua các file sao kê.

## II. Xây dựng ca biểu đồ
![PlantText](https://www.planttext.com/plantuml/png/V9JDQjj04CVlUef1fnQS5-YX1Dg38S4aO7fVhOHciJehoxkbFfOSGicbflHOg6j28JGqXrog9UIm9k-nJz1NABEot6AtkMdtF_kRR_rozuSp8nfZNrU9a4OtS8H2ub1G2M86wH7wfKH0_uNAT6DnQWMD6_LA5HHjJcreLmIc2Uu2tYX_HRtbg1IqHOrA_vLwKlB7pS71StWoGb53Rg5IXOLI2GsvalWKda4wmj1Urv07zmCg5TnvRn3SXSHqbpJML0BgUeSo3kuJ2y6jQf1-AH-7A48mMX18L33JO92naw9Z-Uie-oLrA8d1lOTPS0im6Do2JVtLFbLeo8G6ANQ1eLrgoFnICqy_2XbosGqgoBXKEHEfZ8U86ghWpjY0cv7nmS9w4Tp70MJSfd9pkSSzjXPCOs5I69XQ4M773pTyoPMVXFQUXT2k_f6NWhUMyr7K9zZdjM8fPZE8Qf_Z7kGbVqtcx9kWccyAP1G1bLOho2sL4Rh-i3wBjRaRTF4GLFuE3FhRxOE7c-0-AyZzJnws7KydA0YcTivrREmSfAWZ-0HvGATs7joxNkBHIvFaxv6F3BxWAB7e0es0pI9mD1ZSUT_6TF_v65LXe18rI641UTeoGP2BhebZLB7SLPny6TfB2-Y_RwpMYz1-iscIRDShCbzOAZcN_wnH9uVsyf5LEYmevpz1yXi00F__0m00)

## III. Đặc tả

# Đặc tả ca sử dụng: Thống kê các giao dịch ngân hàng

## Tên ca sử dụng
**Thống kê các giao dịch ngân hàng**

## Tác nhân tham gia
- Khách hàng (Người dùng)

## Mô tả tóm tắt
Ca sử dụng này cho phép người dùng thống kê các giao dịch ngân hàng dựa trên dữ liệu sao kê được nhập vào hệ thống. Người dùng có thể xem các chỉ số thống kê như tổng số tiền giao dịch, số lượng giao dịch và các biểu đồ minh họa.

## Tiền điều kiện (preconditions)
- Người dùng đã đăng nhập vào hệ thống.
- Dữ liệu sao kê giao dịch đã được nhập vào hệ thống.

## Luồng sự kiện chính (main flow)
1. Người dùng chọn chức năng "Thống kê giao dịch" từ giao diện chính.
2. Hệ thống hiển thị các tùy chọn thống kê cho người dùng (theo thời gian, loại giao dịch, tài khoản liên quan, v.v.).
3. Người dùng chọn tiêu chí thống kê và nhấn nút "Thực hiện".
4. Hệ thống tiến hành phân tích dữ liệu giao dịch dựa trên các tiêu chí đã chọn.
5. Hệ thống hiển thị kết quả thống kê dưới dạng bảng biểu và biểu đồ cho người dùng.
6. Người dùng có thể lựa chọn lưu kết quả thống kê hoặc in báo cáo.

## Luồng sự kiện phụ nếu có (alternative flow)
**A1.** Người dùng chọn sai tiêu chí thống kê.
   - Hệ thống hiển thị thông báo lỗi và yêu cầu người dùng chọn lại tiêu chí.

**A2.** Người dùng muốn thay đổi tiêu chí thống kê sau khi nhận kết quả.
   - Người dùng chọn lại tiêu chí thống kê và nhấn nút "Thực hiện".
   - Hệ thống cập nhật và hiển thị kết quả thống kê mới.

## Hậu điều kiện (post conditions)
- Kết quả thống kê được hiển thị cho người dùng.
- Người dùng có thể lưu trữ hoặc in kết quả thống kê nếu muốn.

## Các ngoại lệ
**E1.** Không có dữ liệu giao dịch phù hợp với tiêu chí thống kê.
   - Hệ thống hiển thị thông báo không tìm thấy kết quả và yêu cầu người dùng chọn lại tiêu chí.

**E2.** Hệ thống gặp lỗi khi phân tích dữ liệu.
   - Hệ thống hiển thị thông báo lỗi và yêu cầu người dùng thử lại sau.
## IV. Phi chức năng

### Yêu cầu phi chức năng: Bảo mật thông tin

#### Mô tả
Hệ thống phải đảm bảo rằng tất cả các thông tin giao dịch và dữ liệu cá nhân của người dùng được bảo mật tuyệt đối. Điều này bao gồm việc sử dụng các biện pháp mã hóa, bảo mật khi truyền dữ liệu và kiểm soát truy cập để ngăn chặn truy cập trái phép.

#### Tiêu chí cụ thể
1. **Mã hóa dữ liệu**: Tất cả dữ liệu giao dịch và thông tin cá nhân phải được mã hóa bằng các thuật toán mã hóa mạnh (ví dụ: AES-256) khi lưu trữ và truyền tải.
2. **Kiểm soát truy cập**: Chỉ những người dùng đã được xác thực và có quyền truy cập hợp lệ mới có thể truy cập vào các phần khác nhau của hệ thống. Phải có cơ chế phân quyền rõ ràng.
3. **Xác thực hai yếu tố (2FA)**: Hệ thống phải hỗ trợ xác thực hai yếu tố để tăng cường bảo mật khi người dùng đăng nhập.
4. **Ghi log và giám sát**: Tất cả các hoạt động truy cập và giao dịch phải được ghi log và giám sát để phát hiện và ngăn chặn kịp thời các hành vi truy cập trái phép.
5. **Cập nhật và vá lỗi bảo mật**: Hệ thống phải thường xuyên được cập nhật và vá lỗi bảo mật để đối phó với các mối đe dọa mới nhất.
