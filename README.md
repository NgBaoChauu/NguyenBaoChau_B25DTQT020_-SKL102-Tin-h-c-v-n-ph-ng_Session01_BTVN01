graph TD
    A[Nhập Dữ liệu - Input] --> B(Xử lý Dữ liệu - Processing);
    B --> C{Lưu trữ Dữ liệu - Storage};
    C --> B;
    B --> D[Xuất Kết quả - Output];
    A --> C;
    D --> A;

    style A fill:#F4A460,stroke:#333,stroke-width:2px,color:#000
    style B fill:#87CEFA,stroke:#333,stroke-width:2px,color:#000
    style C fill:#98FB98,stroke:#333,stroke-width:2px,color:#000
    style D fill:#FFD700,stroke:#333,stroke-width:2px,color:#000

    subgraph Hệ thống Bán hàng Online
        direction LR
        A;
        B;
        C;
        D;
    end
    
