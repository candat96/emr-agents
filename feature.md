# Danh sách tính năng EMR chuẩn quốc tế

> **Tổng cộng: ~400 tính năng** | **16 modules** | **Tiêu chuẩn: HL7 FHIR R4, ICD-10, LOINC, SNOMED CT**

---

## Tổng quan modules

| # | Module | Số lượng | Mô tả |
|---|--------|----------|-------|
| 1 | [Quản lý bệnh nhân](#1-quản-lý-bệnh-nhân) | 30 | Hồ sơ, bảo hiểm, tiền sử, dị ứng |
| 2 | [Lịch hẹn & Xếp lịch](#2-lịch-hẹn--xếp-lịch) | 30 | Đặt lịch, hàng đợi, nhắc hẹn, lịch bác sĩ |
| 3 | [Bệnh án điện tử (EMR)](#3-bệnh-án-điện-tử-emr) | 60 | SOAP note, chẩn đoán, điều trị, chuyên khoa |
| 4 | [Đơn thuốc & Dược](#4-đơn-thuốc--dược) | 40 | Kê đơn, tương tác thuốc, tồn kho dược |
| 5 | [Xét nghiệm](#5-xét-nghiệm) | 30 | Chỉ định, mẫu bệnh phẩm, kết quả, LIS |
| 6 | [Chẩn đoán hình ảnh](#6-chẩn-đoán-hình-ảnh) | 20 | DICOM, PACS, đọc kết quả, lưu trữ |
| 7 | [Thanh toán & Hoá đơn](#7-thanh-toán--hoá-đơn) | 25 | Viện phí, bảo hiểm, hoàn trả, báo cáo |
| 8 | [Tồn kho](#8-tồn-kho) | 20 | Thuốc, vật tư, nhập xuất, hạn dùng |
| 9 | [Báo cáo & Phân tích](#9-báo-cáo--phân-tích) | 20 | Dashboard, KPI, dự báo, BI |
| 10 | [Quản trị hệ thống](#10-quản-trị-hệ-thống) | 15 | User, role, cấu hình, audit log |
| 11 | [Khám từ xa](#11-khám-từ-xa) | 20 | Video call, tư vấn từ xa, IoT |
| 12 | [Cổng bệnh nhân & Mobile](#12-cổng-bệnh-nhân--mobile) | 25 | Portal, app, đặt lịch, xem kết quả |
| 13 | [Tích hợp & Liên thông](#13-tích-hợp--liên-thông) | 25 | HL7, FHIR, BHXH, SSO, webhook |
| 14 | [Điều dưỡng & Quản lý buồng](#14-điều-dưỡng--quản-lý-buồng) | 25 | Giường bệnh, MAR, bàn giao ca |
| 15 | [Phòng mổ & Phẫu thuật](#15-phòng-mổ--phẫu-thuật) | 20 | Lịch mổ, WHO checklist, gây mê, hồi sức |
| 16 | [Tuân thủ & Bảo mật](#16-tuân-thủ--bảo-mật) | 20 | RBAC, MFA, mã hoá, DPIA |

---

## 1. Quản lý bệnh nhân

> **30 tính năng** — Quản lý toàn bộ thông tin hành chính, bảo hiểm, tiền sử bệnh nhân

| # | Tính năng | Mô tả |
|---|-----------|-------|
| 1 | Tạo hồ sơ bệnh nhân | Đăng ký bệnh nhân mới với đầy đủ thông tin nhân khẩu |
| 2 | Cập nhật hồ sơ bệnh nhân | Chỉnh sửa thông tin hành chính, liên hệ |
| 3 | Tìm kiếm bệnh nhân | Tìm theo tên, mã bệnh nhân, CCCD, SĐT |
| 4 | Gộp hồ sơ trùng | Phát hiện và merge hồ sơ bệnh nhân bị trùng lặp |
| 5 | Quản lý nhân khẩu học | Quản lý thông tin dân tộc, nghề nghiệp, địa chỉ |
| 6 | Quản lý thông tin bảo hiểm | BHYT, bảo hiểm tư nhân, hạn thẻ |
| 7 | Quản lý liên hệ khẩn cấp | Thông tin người thân, người liên hệ khẩn cấp |
| 8 | Quản lý tiền sử bệnh | Tiền sử bệnh lý cá nhân |
| 9 | Quản lý tiền sử gia đình | Tiền sử bệnh lý gia đình (di truyền) |
| 10 | Quản lý dị ứng | Danh sách dị ứng thuốc, thực phẩm, hoá chất |
| 11 | Quản lý thuốc đang dùng | Danh sách thuốc bệnh nhân đang sử dụng |
| 12 | Ảnh bệnh nhân | Chụp và lưu ảnh chân dung bệnh nhân |
| 13 | Tải lên tài liệu | Tải lên giấy tờ, kết quả xét nghiệm cũ |
| 14 | Phiếu đồng ý điều trị | Quản lý consent form theo quy định |
| 15 | Đồng ý quyền riêng tư | Consent về bảo mật thông tin cá nhân |
| 16 | Gắn nhãn bệnh nhân | Tag phân loại: VIP, ưu tiên, cảnh báo |
| 17 | Ghi chú bệnh nhân | Note nội bộ của nhân viên y tế |
| 18 | Timeline bệnh nhân | Dòng thời gian lịch sử khám chữa bệnh |
| 19 | Nguồn giới thiệu | Theo dõi nguồn giới thiệu bệnh nhân đến |
| 20 | Phân nhóm bệnh nhân | Phân nhóm theo bệnh lý, độ tuổi, khu vực |
| 21 | Danh sách chặn | Chặn bệnh nhân vi phạm nội quy |
| 22 | Quan hệ bệnh nhân | Liên kết gia đình (vợ/chồng, con, bố mẹ) |
| 23 | Truy cập cổng bệnh nhân | Cấp quyền đăng nhập cổng bệnh nhân |
| 24 | Mã QR bệnh nhân | Tạo QR code định danh nhanh |
| 25 | Mã định danh duy nhất | Mã bệnh nhân duy nhất toàn hệ thống |
| 26 | Kiểm tra quyền lợi BHYT | Tra cứu trực tuyến tình trạng thẻ BHYT |
| 27 | Phát hiện hồ sơ trùng | Tự động cảnh báo hồ sơ có nghi ngờ trùng |
| 28 | Phân tích nhân khẩu học | Thống kê độ tuổi, giới tính, khu vực |
| 29 | Tuỳ chọn liên lạc | Email, SMS, Zalo — kênh liên lạc ưu tiên |
| 30 | Quản lý trạng thái | Đang điều trị, xuất viện, chuyển viện, tử vong |

---

## 2. Lịch hẹn & Xếp lịch

> **30 tính năng** — Quản lý lịch khám, hàng đợi, nhắc hẹn tự động

| # | Tính năng | Mô tả |
|---|-----------|-------|
| 1 | Quản lý lịch bác sĩ | Cài đặt giờ làm việc, nghỉ phép từng bác sĩ |
| 2 | Quản lý lịch phòng khám | Lịch hoạt động phòng khám theo ngày/tuần |
| 3 | Đặt lịch hẹn | Đặt lịch khám cho bệnh nhân |
| 4 | Huỷ lịch hẹn | Huỷ bỏ lịch hẹn đã đặt |
| 5 | Đổi lịch hẹn | Chuyển đổi ngày/giờ hẹn khám |
| 6 | Nhắc hẹn qua SMS | Gửi SMS nhắc lịch hẹn tự động |
| 7 | Nhắc hẹn qua email | Gửi email nhắc lịch hẹn tự động |
| 8 | Danh sách chờ | Quản lý bệnh nhân chờ khi hết slot |
| 9 | Đặt lịch online | Bệnh nhân tự đặt lịch qua website/app |
| 10 | Quản lý hàng đợi | Số thứ tự, màn hình gọi số |
| 11 | Tình trạng bác sĩ | Hiển thị bác sĩ đang rảnh/bận/nghỉ |
| 12 | Xếp lịch đa cơ sở | Đặt lịch tại nhiều cơ sở phòng khám |
| 13 | Lịch hẹn định kỳ | Hẹn tái khám định kỳ tự động |
| 14 | Xác nhận lịch hẹn | Bệnh nhân xác nhận qua SMS/app |
| 15 | Check-in bệnh nhân | Đăng ký có mặt tại quầy lễ tân |
| 16 | Check-out bệnh nhân | Kết thúc lượt khám, chuyển thanh toán |
| 17 | Phân tích lịch hẹn | Thống kê tỷ lệ huỷ, no-show, tái khám |
| 18 | Lịch hẹn dạng calendar | Hiển thị lịch hẹn theo ngày/tuần/tháng |
| 19 | Quản lý slot | Cài đặt số lượng slot mỗi khung giờ |
| 20 | Phát hiện xung đột | Cảnh báo trùng lịch bác sĩ/phòng |
| 21 | Ghi chú lịch hẹn | Note yêu cầu đặc biệt của bệnh nhân |
| 22 | Phân loại lịch hẹn | Khám mới, tái khám, cấp cứu, tư vấn |
| 23 | Thời lượng khám | Cài đặt thời gian khám từng loại |
| 24 | Theo dõi no-show | Ghi nhận bệnh nhân vắng mặt không báo |
| 25 | Hẹn khám từ xa | Đặt lịch khám telemedicine |
| 26 | Đặt nhiều bác sĩ | Hẹn khám với nhiều bác sĩ trong 1 lượt |
| 27 | Dashboard lịch hẹn | Tổng quan lịch hẹn trong ngày |
| 28 | Theo dõi trạng thái | Chờ khám, đang khám, đã khám, huỷ |
| 29 | Quản lý công suất | Giới hạn số bệnh nhân tối đa/ngày |
| 30 | Báo cáo lịch hẹn | Báo cáo chi tiết theo bác sĩ, phòng khám |

---

## 3. Bệnh án điện tử (EMR)

> **60 tính năng** — Module lớn nhất — ghi nhận, chẩn đoán, điều trị, theo dõi lâm sàng

| # | Tính năng | Mô tả |
|---|-----------|-------|
| 1 | Tạo lượt khám | Khởi tạo encounter mới cho bệnh nhân |
| 2 | SOAP Note | Ghi nhận theo chuẩn Subjective-Objective-Assessment-Plan |
| 3 | Template lâm sàng | Mẫu bệnh án theo chuyên khoa |
| 4 | Danh sách vấn đề | Problem list theo dõi các vấn đề sức khoẻ |
| 5 | Nhập chẩn đoán | Ghi chẩn đoán chính, phụ |
| 6 | Mã hoá ICD | Gán mã ICD-10 cho chẩn đoán |
| 7 | Soạn thảo ghi chú | Editor ghi chú lâm sàng (rich text) |
| 8 | Nhập sinh hiệu | Nhiệt độ, huyết áp, mạch, SpO2, cân nặng |
| 9 | Khám thể lực | Ghi nhận khám toàn thân, cơ quan |
| 10 | Hỏi bệnh hệ thống | Review of Systems theo cơ quan |
| 11 | Cảnh báo lâm sàng | Alert dị ứng, tương tác thuốc, kết quả bất thường |
| 12 | Kiểm tra dị ứng | Tự động kiểm tra dị ứng khi kê đơn |
| 13 | Kiểm tra tương tác thuốc | Cảnh báo tương tác thuốc-thuốc |
| 14 | Hỗ trợ phác đồ | Gợi ý phác đồ điều trị theo chẩn đoán |
| 15 | Kế hoạch điều trị | Lập kế hoạch điều trị tổng thể |
| 16 | Kế hoạch tái khám | Hẹn lịch tái khám, theo dõi |
| 17 | Hướng dẫn bệnh nhân | In/gửi hướng dẫn chăm sóc tại nhà |
| 18 | Giấy ra viện | Tạo tóm tắt ra viện |
| 19 | Giấy chuyển viện | Tạo giấy giới thiệu chuyển tuyến |
| 20 | Đính kèm lâm sàng | Đính kèm file, hình ảnh vào bệnh án |
| 21 | Chụp ảnh lâm sàng | Chụp và lưu ảnh tổn thương, thương tích |
| 22 | Hồ sơ y tế có cấu trúc | Dữ liệu có cấu trúc theo chuẩn FHIR |
| 23 | Giọng nói thành văn bản | Nhận dạng giọng nói để ghi bệnh án |
| 24 | Tóm tắt lượt khám | Tự động tạo tóm tắt encounter |
| 25 | Timeline lâm sàng | Dòng thời gian toàn bộ lịch sử điều trị |
| 26 | Xem lại tiền sử | Review toàn bộ tiền sử bệnh lý |
| 27 | Đối chiếu thuốc | So sánh thuốc trước/sau nhập viện |
| 28 | Hỗ trợ quyết định lâm sàng | CDS — gợi ý dựa trên evidence-based |
| 29 | Nhật ký kiểm soát | Audit trail mọi thao tác trên bệnh án |
| 30 | Liên trình chăm sóc | Care pathway theo bệnh lý |
| 31 | Phân loại cấp cứu | Triage assessment tại phòng cấp cứu |
| 32 | Đánh giá điều dưỡng | Phiếu đánh giá điều dưỡng |
| 33 | Đánh giá bác sĩ | Phiếu đánh giá của bác sĩ điều trị |
| 34 | Ghi nhận thủ thuật | Tài liệu hoá thủ thuật, tiểu phẫu |
| 35 | Mẫu tài liệu lâm sàng | Template giấy tờ lâm sàng |
| 36 | Smart Forms | Biểu mẫu thông minh tự động điền |
| 37 | Smart Macros | Phím tắt nhập nhanh cụm từ thường dùng |
| 38 | Gợi ý mã bệnh | Tự động gợi ý ICD-10 từ mô tả |
| 39 | Sổ đăng ký bệnh | Registry theo dõi bệnh truyền nhiễm, mạn tính |
| 40 | Cộng tác nhóm điều trị | Phối hợp liên chuyên khoa |
| 41 | Ký số tài liệu y tế | Chữ ký điện tử trên bệnh án |
| 42 | Quản lý phiên bản bệnh án | Version control dữ liệu lâm sàng |
| 43 | Theo dõi bệnh mạn tính | Quản lý dài hạn: đái tháo đường, tăng HA |
| 44 | Lịch sử tiêm chủng | Ghi nhận vaccine đã tiêm |
| 45 | Theo dõi thai kỳ | Sản khoa — theo dõi thai kỳ |
| 46 | Biểu đồ tăng trưởng nhi | Growth chart cho trẻ em |
| 47 | Hồ sơ ung bướu | Bệnh án chuyên khoa ung thư |
| 48 | Sơ đồ răng | Dental chart cho răng hàm mặt |
| 49 | Hình ảnh da liễu | Chụp và so sánh tổn thương da |
| 50 | Template chuyên khoa | Mẫu bệnh án riêng theo từng chuyên khoa |
| 51 | Chấm điểm nguy cơ | Scoring: NEWS, APACHE, qSOFA... |
| 52 | Gắn nhãn lượt khám | Tag encounter: cấp cứu, VIP, nghiên cứu |
| 53 | Tự động hoá quy trình | Workflow automation lâm sàng |
| 54 | Quản lý ca bệnh | Case management phức tạp |
| 55 | Ghi chú liên chuyên khoa | Note đa chuyên khoa trong 1 bệnh án |
| 56 | KPI lâm sàng | Theo dõi chỉ số chất lượng lâm sàng |
| 57 | Theo dõi tiến trình | Biểu đồ tiến trình điều trị bệnh nhân |
| 58 | Xuất tóm tắt lâm sàng | Export bệnh án ra PDF/FHIR |
| 59 | Theo dõi chuyển viện | Trạng thái giấy chuyển tuyến |
| 60 | Quản lý đợt điều trị | Care episode từ nhập viện đến ra viện |

---

## 4. Đơn thuốc & Dược

> **40 tính năng** — Kê đơn điện tử, kiểm soát tương tác, quản lý dược

| # | Tính năng | Mô tả |
|---|-----------|-------|
| 1 | Kê đơn điện tử | Tạo đơn thuốc điện tử (ePrescription) |
| 2 | Danh mục thuốc | Catalog thuốc theo tên gốc, tên thương mại |
| 3 | Tính liều dùng | Tự động tính liều theo cân nặng, tuổi |
| 4 | Kiểm tra tương tác thuốc | Cảnh báo tương tác thuốc-thuốc |
| 5 | Kiểm tra dị ứng thuốc | Cảnh báo dị ứng khi kê đơn |
| 6 | Mẫu đơn thuốc | Template đơn thuốc theo chẩn đoán |
| 7 | Kê đơn tiếp | Refill đơn thuốc cũ |
| 8 | Huỷ đơn thuốc | Huỷ bỏ đơn thuốc đã kê |
| 9 | Duyệt đơn thuốc | Phê duyệt đơn bởi dược sĩ |
| 10 | Lịch sử dùng thuốc | Toàn bộ lịch sử thuốc đã dùng |
| 11 | Theo dõi tuân thủ thuốc | Đo lường bệnh nhân uống thuốc đúng lịch |
| 12 | Xử lý đơn tại nhà thuốc | Quy trình nhận đơn, cấp phát |
| 13 | Tích hợp tồn kho thuốc | Kiểm tra tồn trước khi kê |
| 14 | Quét barcode thuốc | Xác nhận thuốc bằng mã vạch |
| 15 | Cấp phát thuốc | Ghi nhận phát thuốc cho bệnh nhân |
| 16 | Thay thế thuốc | Đổi thuốc tương đương khi hết hàng |
| 17 | Cảnh báo thuốc | Alert quá liều, chống chỉ định |
| 18 | Phác đồ dùng thuốc | Tích hợp guideline dùng thuốc quốc tế |
| 19 | Quản lý thuốc kiểm soát | Thuốc gây nghiện, hướng thần đặc biệt |
| 20 | In đơn thuốc | In đơn thuốc theo mẫu quy định |
| 21 | Chữ ký số đơn thuốc | Ký điện tử xác nhận đơn thuốc |
| 22 | Đối chiếu thuốc | Medication reconciliation nhập/xuất viện |
| 23 | Ghi nhận tư vấn thuốc | Nội dung tư vấn cho bệnh nhân |
| 24 | Phân tích đơn thuốc | Thống kê xu hướng kê đơn |
| 25 | Danh mục thuốc BV | Formulary thuốc được phép sử dụng |
| 26 | Xác nhận thuốc BHYT | Kiểm tra thuốc thuộc danh mục BHYT |
| 27 | Nhắc uống thuốc | Push notification nhắc giờ uống |
| 28 | Kiểm tra hạn dùng | Cảnh báo thuốc gần/hết hạn |
| 29 | Theo dõi lô thuốc | Truy xuất nguồn gốc theo batch |
| 30 | Cảnh báo tồn kho dược | Alert khi thuốc sắp hết |
| 31 | Trả thuốc | Quy trình bệnh nhân trả thuốc |
| 32 | Xử lý thuốc huỷ | Quản lý thuốc huỷ, hết hạn |
| 33 | KPI nhà thuốc | Hiệu suất hoạt động nhà thuốc |
| 34 | Kiểm soát đối chiếu thuốc | Audit quy trình medication reconciliation |
| 35 | Báo cáo dược | Báo cáo sử dụng thuốc định kỳ |
| 36 | Dashboard tương tác thuốc | Tổng quan cảnh báo tương tác |
| 37 | Quản lý kháng sinh | Antibiotic stewardship tracking |
| 38 | Phân tích chi phí thuốc | So sánh chi phí thuốc theo chẩn đoán |
| 39 | Giáo dục bệnh nhân về thuốc | Tài liệu hướng dẫn sử dụng thuốc |
| 40 | Lịch sử chỉ định thuốc | Toàn bộ order thuốc đã kê |

---

## 5. Xét nghiệm

> **30 tính năng** — Chỉ định, thu mẫu, kết quả, tích hợp LIS

| # | Tính năng | Mô tả |
|---|-----------|-------|
| 1 | Tạo chỉ định xét nghiệm | Bác sĩ chỉ định xét nghiệm |
| 2 | Danh mục xét nghiệm | Catalog xét nghiệm có sẵn |
| 3 | Theo dõi mẫu bệnh phẩm | Tracking specimen từ thu đến kết quả |
| 4 | Dán barcode mẫu | In mã vạch cho ống mẫu |
| 5 | Thu mẫu bệnh phẩm | Ghi nhận quy trình lấy mẫu |
| 6 | Quản lý quy trình lab | Workflow toàn bộ quy trình xét nghiệm |
| 7 | Nhập kết quả | Kỹ thuật viên nhập kết quả |
| 8 | Xác nhận kết quả | Validation kết quả bởi kỹ thuật viên cấp cao |
| 9 | Duyệt kết quả | Bác sĩ lab phê duyệt trả kết quả |
| 10 | Cảnh báo kết quả bất thường | Alert khi chỉ số ngoài khoảng tham chiếu |
| 11 | Đính kèm kết quả | Gắn file PDF, hình ảnh vào kết quả |
| 12 | Tích hợp thiết bị | Kết nối trực tiếp máy xét nghiệm |
| 13 | Tích hợp LIS | Liên thông với hệ thống Lab Information System |
| 14 | Quản lý khoảng tham chiếu | Cài đặt reference range theo tuổi, giới |
| 15 | Biểu đồ xu hướng | Trend chart theo dõi chỉ số theo thời gian |
| 16 | Cảnh báo giá trị nguy hiểm | Critical value alert báo bác sĩ ngay |
| 17 | Theo dõi thời gian xử lý | TAT — turnaround time mỗi xét nghiệm |
| 18 | Ưu tiên xét nghiệm | Cấp độ ưu tiên: thường, khẩn, cấp cứu |
| 19 | Xử lý theo lô | Chạy xét nghiệm theo batch |
| 20 | Theo dõi trạng thái chỉ định | Trạng thái: đã chỉ định, đang xử lý, có kết quả |
| 21 | Tích hợp thanh toán lab | Liên kết chi phí xét nghiệm với viện phí |
| 22 | Chia sẻ kết quả | Gửi kết quả cho bác sĩ điều trị/bệnh nhân |
| 23 | Tạo báo cáo xét nghiệm | In phiếu kết quả xét nghiệm |
| 24 | Kiểm soát chất lượng | QC nội kiểm, ngoại kiểm |
| 25 | Nhật ký kiểm soát lab | Audit trail thao tác trong lab |
| 26 | Xuất kết quả | Export kết quả ra PDF, CSV |
| 27 | Dashboard phân tích lab | Thống kê hoạt động lab |
| 28 | Báo cáo năng suất | Hiệu suất kỹ thuật viên, máy móc |
| 29 | Huỷ chỉ định | Huỷ bỏ chỉ định xét nghiệm |
| 30 | Sửa chỉ định | Chỉnh sửa chỉ định đã tạo |

---

## 6. Chẩn đoán hình ảnh

> **20 tính năng** — DICOM, PACS, đọc kết quả, lưu trữ hình ảnh y tế

| # | Tính năng | Mô tả |
|---|-----------|-------|
| 1 | Chỉ định CĐHA | Bác sĩ chỉ định chụp X-quang, CT, MRI... |
| 2 | Quản lý modality | Cài đặt máy chụp: X-ray, CT, MRI, US |
| 3 | Quy trình X-quang | Workflow từ chỉ định đến trả kết quả |
| 4 | Báo cáo X-quang | Bác sĩ CĐHA đọc và trả kết quả |
| 5 | Trình xem hình ảnh | Viewer xem ảnh DICOM trên web |
| 6 | Tích hợp DICOM | Nhận ảnh từ máy chụp qua giao thức DICOM |
| 7 | Tích hợp PACS | Kết nối hệ thống lưu trữ hình ảnh |
| 8 | Ghi chú trên hình ảnh | Annotation: đo, đánh dấu, ghi chú |
| 9 | So sánh hình ảnh | So sánh ảnh trước/sau điều trị |
| 10 | Đính kèm hình ảnh | Gắn ảnh vào bệnh án |
| 11 | Duyệt báo cáo CĐHA | Phê duyệt kết quả CĐHA |
| 12 | Cảnh báo nguy hiểm | Alert kết quả bất thường nguy hiểm |
| 13 | Trạng thái chỉ định | Theo dõi: đã chỉ định, đã chụp, có kết quả |
| 14 | Thanh toán CĐHA | Liên kết chi phí CĐHA với viện phí |
| 15 | Phân tích CĐHA | Thống kê số lượng, loại chụp |
| 16 | Lưu trữ hình ảnh | Archive ảnh dài hạn |
| 17 | Chia sẻ hình ảnh | Gửi ảnh cho bác sĩ khác/bệnh nhân |
| 18 | Kiểm soát chất lượng | QC hình ảnh và báo cáo |
| 19 | Nhật ký kiểm soát | Audit log thao tác CĐHA |
| 20 | Xuất kết quả | Export báo cáo ra PDF |

---

## 7. Thanh toán & Hoá đơn

> **25 tính năng** — Quản lý viện phí, bảo hiểm, hoàn trả, báo cáo tài chính

| # | Tính năng | Mô tả |
|---|-----------|-------|
| 1 | Danh mục dịch vụ | Catalog dịch vụ khám, thủ thuật, xét nghiệm |
| 2 | Quản lý bảng giá | Cài đặt giá theo đối tượng, loại dịch vụ |
| 3 | Tạo phiếu thu | Lập phiếu thu viện phí |
| 4 | Điều chỉnh viện phí | Sửa lại chi phí khi có sai sót |
| 5 | Giảm giá/miễn giảm | Áp dụng giảm giá, miễn phí theo chính sách |
| 6 | Xuất hoá đơn | Tạo hoá đơn điện tử/giấy |
| 7 | Ghi nhận thanh toán | Thu tiền mặt, chuyển khoản, thẻ |
| 8 | Phương thức thanh toán | Tiền mặt, thẻ, QR Pay, ví điện tử |
| 9 | Thanh toán bảo hiểm | Xử lý phần BHYT chi trả |
| 10 | Tính đồng chi trả | Tự động tính phần bệnh nhân đóng |
| 11 | Tạo hồ sơ bảo hiểm | Tạo claim gửi cơ quan bảo hiểm |
| 12 | Theo dõi claim | Trạng thái claim: gửi, duyệt, từ chối |
| 13 | Hoàn trả | Hoàn tiền khi huỷ dịch vụ |
| 14 | Huỷ phiếu thu | Huỷ bỏ phiếu thu sai |
| 15 | Dashboard doanh thu | Tổng quan doanh thu theo ngày/tháng |
| 16 | Kiểm toán viện phí | Audit phiếu thu, hoá đơn |
| 17 | Báo cáo doanh thu ngày | Kết ca, đối soát cuối ngày |
| 18 | Doanh thu theo khoa | Phân tích doanh thu từng khoa/phòng |
| 19 | Chia sẻ doanh thu bác sĩ | Tính hoa hồng, thu nhập bác sĩ |
| 20 | Phân tích tài chính | Thống kê xu hướng doanh thu |
| 21 | Tính thuế | Thuế GTGT, thuế thu nhập |
| 22 | Xuất dữ liệu | Export báo cáo ra Excel, PDF |
| 23 | Báo cáo tài chính | Báo cáo tài chính tổng hợp |
| 24 | Tích hợp cổng thanh toán | Kết nối VNPay, Momo, ngân hàng |
| 25 | Đối soát | Reconciliation sổ sách hàng ngày |

---

## 8. Tồn kho

> **20 tính năng** — Quản lý thuốc, vật tư, nhập xuất, hạn dùng

| # | Tính năng | Mô tả |
|---|-----------|-------|
| 1 | Tồn kho thuốc | Quản lý số lượng thuốc hiện có |
| 2 | Tồn kho vật tư y tế | Quản lý vật tư tiêu hao, thiết bị |
| 3 | Quản lý kho | Cài đặt nhiều kho: kho chính, kho lẻ, kho khoa |
| 4 | Nhập xuất kho | Ghi nhận phiếu nhập, phiếu xuất |
| 5 | Theo dõi lô | Quản lý batch/lot number |
| 6 | Theo dõi hạn dùng | Cảnh báo thuốc/vật tư gần hết hạn |
| 7 | Cảnh báo tồn kho | Alert khi dưới mức tồn tối thiểu |
| 8 | Chuyển kho | Điều chuyển giữa các kho |
| 9 | Điều chỉnh tồn kho | Xử lý chênh lệch kiểm kê |
| 10 | Đặt hàng | Tạo đơn đặt hàng nhà cung cấp |
| 11 | Quản lý nhà cung cấp | Danh sách NCC, hợp đồng, giá |
| 12 | Định giá tồn kho | Tính giá trị tồn kho (FIFO, bình quân) |
| 13 | Báo cáo tồn kho | Báo cáo nhập xuất tồn |
| 14 | Barcode tồn kho | Mã vạch cho thuốc, vật tư |
| 15 | Kiểm kê | Kiểm kê định kỳ, đột xuất |
| 16 | Phân tích tồn kho | Thống kê tiêu thụ, tồn đọng |
| 17 | Tích hợp nhà thuốc | Đồng bộ tồn kho với nhà thuốc |
| 18 | Gợi ý đặt hàng | Tự động đề xuất đặt hàng khi tồn thấp |
| 19 | Báo cáo sử dụng | Thống kê lượng tiêu thụ theo thời gian |
| 20 | Dashboard tồn kho | Tổng quan tồn kho realtime |

---

## 9. Báo cáo & Phân tích

> **20 tính năng** — Dashboard, KPI, dự báo, kết nối BI

| # | Tính năng | Mô tả |
|---|-----------|-------|
| 1 | Dashboard vận hành | Tổng quan hoạt động bệnh viện theo ngày |
| 2 | KPI lâm sàng | Chỉ số chất lượng khám chữa bệnh |
| 3 | KPI tài chính | Chỉ số doanh thu, công nợ, lợi nhuận |
| 4 | Phân tích bệnh nhân | Thống kê bệnh nhân theo nhóm |
| 5 | Hiệu suất bác sĩ | Số lượt khám, doanh thu, đánh giá |
| 6 | Thống kê bệnh tật | Phân bổ bệnh theo ICD-10 |
| 7 | Phân tích đơn thuốc | Xu hướng kê đơn, chi phí thuốc |
| 8 | Phân tích lịch hẹn | Tỷ lệ đặt lịch, huỷ, no-show |
| 9 | Phân tích doanh thu | Xu hướng doanh thu theo thời gian |
| 10 | Phân tích tồn kho | Tiêu thụ, tồn đọng, quá hạn |
| 11 | Phân tích xét nghiệm | Thống kê loại XN, tỷ lệ bất thường |
| 12 | Phân tích CĐHA | Thống kê loại chụp, thời gian đọc |
| 13 | Phân tích cohort | So sánh nhóm bệnh nhân |
| 14 | Phân tích lưu giữ BN | Tỷ lệ bệnh nhân quay lại |
| 15 | Phân tích hài lòng | Khảo sát mức độ hài lòng |
| 16 | Phân tích dự báo | Predictive: dự báo lượt khám, doanh thu |
| 17 | Tích hợp BI | Kết nối Power BI, Metabase, Superset |
| 18 | Xuất dữ liệu | Export CSV, Excel, PDF |
| 19 | Tạo báo cáo tuỳ chỉnh | Drag & drop report builder |
| 20 | Gửi báo cáo tự động | Gửi báo cáo định kỳ qua email |

---

## 10. Quản trị hệ thống

> **15 tính năng** — Quản lý người dùng, phân quyền, cấu hình

| # | Tính năng | Mô tả |
|---|-----------|-------|
| 1 | Quản lý người dùng | Tạo, sửa, khoá tài khoản nhân viên |
| 2 | Quản lý vai trò | Định nghĩa role: bác sĩ, điều dưỡng, admin... |
| 3 | Quản lý quyền | Phân quyền chi tiết theo chức năng |
| 4 | Nhật ký hệ thống | Audit log mọi thao tác |
| 5 | Quản lý tổ chức | Cấu hình bệnh viện, phòng khám |
| 6 | Quản lý phòng khám | Thông tin cơ sở, địa chỉ, liên hệ |
| 7 | Quản lý khoa phòng | Cấu trúc khoa, phòng, đơn vị |
| 8 | Quản lý cấu hình | Tham số hệ thống, tuỳ chọn |
| 9 | Quản lý mẫu biểu | Template đơn thuốc, giấy tờ, báo cáo |
| 10 | Quản lý danh mục gốc | Master data: ICD, thuốc, dịch vụ |
| 11 | Cấu hình thông báo | Cài đặt kênh và nội dung thông báo |
| 12 | Cấu hình tích hợp | Quản lý kết nối API bên ngoài |
| 13 | Sao lưu dữ liệu | Backup định kỳ, phục hồi |
| 14 | Giám sát hệ thống | Health check, uptime, performance |
| 15 | Quản lý giấy phép | Bản quyền, hạn sử dụng, module |

---

## 11. Khám từ xa

> **20 tính năng** — Khám từ xa, video call, theo dõi IoT

| # | Tính năng | Mô tả |
|---|-----------|-------|
| 1 | Tư vấn video | Khám bệnh qua video call |
| 2 | Tư vấn audio | Khám bệnh qua điện thoại/audio |
| 3 | Đặt lịch telemedicine | Xếp lịch khám từ xa |
| 4 | Phòng chờ từ xa | Waiting room ảo trước khi vào phòng khám |
| 5 | Chia sẻ màn hình | Bác sĩ chia sẻ hình ảnh, kết quả cho BN |
| 6 | Đồng ý khám từ xa | Consent form khám telemedicine |
| 7 | Kê đơn từ xa | Kê đơn điện tử sau khám online |
| 8 | Theo dõi sinh hiệu từ xa | Nhận dữ liệu từ thiết bị tại nhà |
| 9 | Tích hợp thiết bị đeo | Kết nối smartwatch, máy đo huyết áp |
| 10 | Ghi hình buổi khám | Lưu lại video buổi tư vấn |
| 11 | Ghi chú telemedicine | Note bác sĩ trong buổi khám từ xa |
| 12 | Tái khám từ xa | Hẹn lịch tái khám telemedicine |
| 13 | Thanh toán telemedicine | Thu phí khám từ xa |
| 14 | Phân tích telemedicine | Thống kê lượt khám online |
| 15 | Hội chẩn nhiều bác sĩ | Hội chẩn từ xa nhiều chuyên gia |
| 16 | Hàng đợi telemedicine | Quản lý thứ tự bệnh nhân chờ |
| 17 | Thông báo telemedicine | Push thông báo đến giờ khám |
| 18 | Check-in telemedicine | Bệnh nhân báo có mặt online |
| 19 | Kiểm tra kỹ thuật | Test camera, mic trước khi khám |
| 20 | Khảo sát hài lòng | Đánh giá chất lượng sau khám từ xa |

---

## 12. Cổng bệnh nhân & Mobile

> **25 tính năng** — Patient portal, ứng dụng di động cho bệnh nhân

| # | Tính năng | Mô tả |
|---|-----------|-------|
| 1 | Đăng nhập/đăng ký | Bệnh nhân tạo tài khoản và đăng nhập |
| 2 | Xem hồ sơ sức khoẻ | Bệnh nhân xem bệnh án của mình |
| 3 | Xem kết quả xét nghiệm | Tra cứu kết quả lab online |
| 4 | Xem kết quả CĐHA | Xem ảnh chụp và kết quả CĐHA |
| 5 | Đặt lịch hẹn online | Tự đặt lịch khám qua app |
| 6 | Lịch sử khám bệnh | Xem toàn bộ lịch sử khám |
| 7 | Xem đơn thuốc | Xem đơn thuốc đã kê |
| 8 | Nhắc uống thuốc | Thông báo nhắc giờ uống thuốc |
| 9 | Thanh toán online | Thanh toán viện phí qua app |
| 10 | Lịch sử thanh toán | Xem hoá đơn, biên lai |
| 11 | Nhắn tin bác sĩ | Chat với bác sĩ điều trị |
| 12 | Upload tài liệu | Gửi file, ảnh cho bác sĩ |
| 13 | Tóm tắt sức khoẻ | Tổng quan sức khoẻ cá nhân |
| 14 | Truy cập thành viên gia đình | Quản lý hồ sơ người thân |
| 15 | Góp ý/khảo sát | Đánh giá chất lượng dịch vụ |
| 16 | Cài đặt thông báo | Tuỳ chọn nhận thông báo |
| 17 | Kiến thức sức khoẻ | Bài viết giáo dục sức khoẻ |
| 18 | Sổ tiêm chủng | Xem lịch sử tiêm vaccine |
| 19 | Trạng thái chuyển viện | Theo dõi tình trạng giấy chuyển tuyến |
| 20 | Đồng bộ thiết bị đeo | Kết nối smartwatch, fitness tracker |
| 21 | Liên hệ khẩn cấp | Cập nhật thông tin liên hệ khẩn cấp |
| 22 | Quản lý đồng ý | Xem và ký consent form online |
| 23 | Xuất dữ liệu (FHIR) | Tải hồ sơ sức khoẻ theo chuẩn FHIR |
| 24 | Push notification | Thông báo lịch hẹn, kết quả, nhắc thuốc |
| 25 | Chatbot hỗ trợ | Trợ lý ảo trả lời câu hỏi thường gặp |

---

## 13. Tích hợp & Liên thông

> **25 tính năng** — HL7, FHIR, BHXH, SSO, webhook

| # | Tính năng | Mô tả |
|---|-----------|-------|
| 1 | HL7 v2 messaging | Gửi/nhận thông điệp HL7 v2.x |
| 2 | HL7 FHIR R4 API | RESTful API theo chuẩn FHIR R4 |
| 3 | Tích hợp LIS | Kết nối hệ thống xét nghiệm |
| 4 | Tích hợp PACS/RIS | Kết nối hệ thống CĐHA |
| 5 | DICOM gateway | Cổng tiếp nhận ảnh DICOM |
| 6 | Cổng BHXH (XML 4210) | Gửi dữ liệu giám định BHXH |
| 7 | Cổng báo cáo CDC | Báo cáo bệnh truyền nhiễm lên CDC |
| 8 | Tích hợp hệ thống dược | Kết nối DMS, nhà thuốc ngoài |
| 9 | Tích hợp cổng bảo hiểm | Tra cứu, gửi claim bảo hiểm |
| 10 | Tích hợp cổng thanh toán | VNPay, Momo, ngân hàng |
| 11 | Tích hợp SMS gateway | Gửi SMS tự động |
| 12 | Tích hợp email | Gửi email thông báo, báo cáo |
| 13 | Single Sign-On (SSO) | Đăng nhập một lần (Keycloak, Azure AD) |
| 14 | Tích hợp nhà cung cấp định danh | LDAP, SAML, OpenID Connect |
| 15 | Master Patient Index | Định danh bệnh nhân toàn hệ thống |
| 16 | Health Information Exchange | Trao đổi dữ liệu giữa cơ sở y tế |
| 17 | Tích hợp thiết bị IoT | Kết nối thiết bị đeo, cảm biến |
| 18 | API cho ứng dụng thứ ba | Open API cho partner tích hợp |
| 19 | Công cụ nhập/chuyển đổi dữ liệu | Import từ hệ thống cũ |
| 20 | Xuất dữ liệu | Export CSV, Excel, PDF |
| 21 | Hệ thống webhook | Event-driven thông báo realtime |
| 22 | Rate limiting & monitoring | Kiểm soát lưu lượng API |
| 23 | Xử lý lỗi & tự động thử lại | Retry mechanism cho tích hợp |
| 24 | Nhật ký tích hợp | Audit log mọi giao dịch liên thông |
| 25 | FHIR Bulk Data Export | Xuất dữ liệu lớn theo chuẩn FHIR Bulk |

---

## 14. Điều dưỡng & Quản lý buồng

> **25 tính năng** — Giường bệnh, điều dưỡng, bàn giao ca, MAR

| # | Tính năng | Mô tả |
|---|-----------|-------|
| 1 | Quản lý giường bệnh | Cài đặt giường theo khoa, phòng, buồng |
| 2 | Dashboard giường trống | Hiển thị real-time giường còn trống |
| 3 | Phân giường | Xếp giường cho bệnh nhân nhập viện |
| 4 | Chuyển giường | Chuyển bệnh nhân giữa các giường/phòng |
| 5 | Thống kê buồng bệnh | Census — số bệnh nhân đang nằm viện |
| 6 | Phiếu đánh giá điều dưỡng | Form đánh giá của điều dưỡng |
| 7 | Kế hoạch chăm sóc | Nursing care plan cho từng bệnh nhân |
| 8 | Phiếu theo dõi thuốc (MAR) | Medication Administration Record |
| 9 | Biểu đồ sinh hiệu | Charting: nhiệt độ, mạch, HA, SpO2 |
| 10 | Theo dõi vào/ra | Intake/output: dịch truyền, nước tiểu |
| 11 | Đánh giá nguy cơ té ngã | Fall risk assessment scoring |
| 12 | Đánh giá đau | Pain assessment scale |
| 13 | Ghi nhận chăm sóc vết thương | Wound care documentation |
| 14 | Phiếu bàn giao bệnh nhân | Handoff report khi chuyển ca |
| 15 | Bàn giao ca trực | Shift handover — điều dưỡng giao ca |
| 16 | Quản lý công việc điều dưỡng | Task list cho từng ca trực |
| 17 | Lịch đi buồng | Patient rounding schedule |
| 18 | Cảnh báo cách ly | Alert bệnh nhân cần cách ly |
| 19 | In vòng tay bệnh nhân | In wristband định danh |
| 20 | Dashboard khối lượng công việc | Workload của từng điều dưỡng |
| 21 | Kế hoạch xuất viện | Discharge planning và hướng dẫn |
| 22 | Giáo dục bệnh nhân | Tài liệu hướng dẫn chăm sóc |
| 23 | KPI điều dưỡng | Chỉ số hiệu suất điều dưỡng |
| 24 | Ghi chú điều dưỡng | Nurse note theo dõi hàng ngày |
| 25 | Phân tích buồng bệnh | Thống kê công suất, thời gian nằm |

---

## 15. Phòng mổ & Phẫu thuật

> **20 tính năng** — Lịch mổ, WHO checklist, gây mê, hồi sức

| # | Tính năng | Mô tả |
|---|-----------|-------|
| 1 | Xếp lịch phẫu thuật | Đặt lịch mổ cho bệnh nhân |
| 2 | Lịch phòng mổ | Calendar phòng mổ theo ngày |
| 3 | Quản lý phòng mổ | Tình trạng phòng mổ: trống, đang sử dụng |
| 4 | Đánh giá tiền phẫu | Khám và đánh giá trước mổ |
| 5 | Checklist phẫu thuật (WHO) | WHO Surgical Safety Checklist |
| 6 | Phiếu gây mê | Ghi nhận quy trình gây mê/hồi sức |
| 7 | Ghi nhận trong mổ | Intra-operative note |
| 8 | Ghi nhận sau mổ | Post-operative note |
| 9 | Theo dõi dụng cụ phẫu thuật | Kiểm đếm dụng cụ trước/sau mổ |
| 10 | Phiếu đồng ý phẫu thuật | Consent form phẫu thuật |
| 11 | Phân công ê-kíp mổ | Phân công phẫu thuật viên, gây mê, điều dưỡng |
| 12 | Thời gian phẫu thuật | Theo dõi thời gian từng giai đoạn mổ |
| 13 | Biến chứng phẫu thuật | Ghi nhận và theo dõi biến chứng |
| 14 | Thanh toán phẫu thuật | Chi phí phẫu thuật, vật tư, gây mê |
| 15 | Báo cáo phẫu thuật | Báo cáo kết quả phẫu thuật |
| 16 | Phân tích sử dụng phòng mổ | OR utilization analytics |
| 17 | Theo dõi huỷ mổ | Ghi nhận lý do huỷ/hoãn phẫu thuật |
| 18 | Quản lý vật tư phẫu thuật | Vật tư tiêu hao trong mổ |
| 19 | Quản lý phòng hồi sức | Recovery room sau phẫu thuật |
| 20 | Nhật ký phẫu thuật | Audit log mọi thao tác |

---

## 16. Tuân thủ & Bảo mật

> **20 tính năng** — RBAC, MFA, mã hoá, DPIA, kiểm soát truy cập

| # | Tính năng | Mô tả |
|---|-----------|-------|
| 1 | Kiểm soát truy cập (RBAC) | Phân quyền theo vai trò |
| 2 | Xác thực đa yếu tố (MFA) | OTP, authenticator app, SMS |
| 3 | Mã hoá dữ liệu lưu trữ | AES-256 encryption at rest |
| 4 | Mã hoá dữ liệu truyền tải | TLS 1.3 encryption in transit |
| 5 | Nhật ký bất biến | Immutable audit trail |
| 6 | Quản lý đồng ý | Consent management theo quy định |
| 7 | Chính sách lưu trữ dữ liệu | Data retention policy cấu hình |
| 8 | Ẩn danh hoá dữ liệu | De-identification cho nghiên cứu |
| 9 | Giả danh hoá dữ liệu | Pseudonymization cho phân tích |
| 10 | Quy trình thông báo vi phạm | Breach notification workflow |
| 11 | Đánh giá tác động DPIA | Data Protection Impact Assessment |
| 12 | Dashboard tuân thủ | Tổng quan trạng thái tuân thủ |
| 13 | Tạo báo cáo tuân thủ | Báo cáo gửi cơ quan quản lý |
| 14 | Xử lý yêu cầu truy cập dữ liệu | Data access request handling |
| 15 | Quy trình xoá dữ liệu | Right to erasure workflow |
| 16 | Lưu trữ dữ liệu nội địa | Data localization enforcement |
| 17 | Quản lý phiên & timeout | Session management bảo mật |
| 18 | IP whitelist/blacklist | Hạn chế truy cập theo IP |
| 19 | Nhật ký sự cố bảo mật | Security incident logging |
| 20 | Theo dõi pentest | Penetration test report tracking |

---

> **Tổng cộng: 400 tính năng** trên 16 modules, bao phủ toàn bộ quy trình vận hành bệnh viện và phòng khám theo tiêu chuẩn quốc tế.
