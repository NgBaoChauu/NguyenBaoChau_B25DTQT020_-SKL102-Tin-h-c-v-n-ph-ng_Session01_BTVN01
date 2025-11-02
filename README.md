```mermaid
graph TD
    A([Bắt Đầu]) --> B;
    B{{Sinh viên nhập điểm kiểm tra/bài tập}};
    B --> C[Phần mềm tiếp nhận và kiểm tra tính hợp lệ của điểm];
    C --> D{Điểm có hợp lệ không?};
    D -- Có --> E[Hệ thống Tính Điểm Trung bình Môn/Tổng kết];
    D -- Không --> F{{Thông báo lỗi: Yêu cầu nhập lại}};
    F --> B;
    E --> G[Lưu trữ Điểm số đã tính vào Cơ sở Dữ liệu];
    G --> H{Cần in Báo cáo?};
    H -- Có --> I[Hệ thống Tạo Phiếu báo điểm/Bảng điểm];
    H -- Không --> J[Hiển thị Bảng điểm trên giao diện người dùng];
    I --> K{{In Phiếu báo điểm/Bảng điểm}};
    K --> L([Kết Thúc]);
    J --> L;

    % Định nghĩa màu sắc và hình dạng cho dễ đọc (Tùy chọn)
    style A fill:#D8BFD8,stroke:#800080
    style L fill:#D8BFD8,stroke:#800080
    style B fill:#F5F5DC,stroke:#B8860B % Bình hành - Input
    style F fill:#F5F5DC,stroke:#B8860B % Bình hành - Output
    style K fill:#F5F5DC,stroke:#B8860B % Bình hành - Output
    style C fill:#ADD8E6,stroke:#0000FF % Chữ nhật - Process
    style E fill:#ADD8E6,stroke:#0000FF % Chữ nhật - Process
    style G fill:#ADD8E6,stroke:#0000FF % Chữ nhật - Process
    style I fill:#ADD8E6,stroke:#0000FF % Chữ nhật - Process
    style J fill:#ADD8E6,stroke:#0000FF % Chữ nhật - Process
    style D fill:#FFA07A,stroke:#FF4500 % Thoi - Decision
    style H fill:#FFA07A,stroke:#FF4500 % Thoi - Decision
