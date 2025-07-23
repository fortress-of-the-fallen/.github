
# Cấu trúc Thư mục Dự án

```plaintext
Source/
├── GameClient/
│   └── Bootstrap/
│       └── AddDependenciesInjection.cs       # Đăng ký toàn bộ DI, SignalBus, Handler
│
├── Adapter/
│   ├── Signals/
│   │   └── <ServiceName>/
│   │       ├── ReqModel.cs                   # Gửi signal: _signalBus.Fire(Mapper.Map<ReqDto>(ReqModel))
│   │       └── ResModel.cs                   # Nhận kết quả và map: Mapper.Map<ResModel>(resDto)
│   │
│   ├── Mapper/                               # Chứa logic mapping giữa Model <-> Dto
│   └── SignalsRegister.cs                    # Đăng ký các Signal vào Zenject
│
└── Application/
    ├── Service/
    │   └── <ServiceName>/
    │       ├── ReqModel/                     # Dto được xử lý bên trong Service
    │       ├── ResModel/
    │       └── <ServiceName>.cs              # Interface + Implementation xử lý logic nghiệp vụ
    │
    ├── External/
    │   ├── API/                              # Tích hợp API bên ngoài
    │   ├── Storage/                          # Lưu trữ dữ liệu tạm/thường
    │   └── Logger/                           # Ghi log và trace hệ thống
    │
    ├── Domain/
    │   ├── Entities/                         # Các entity cốt lõi của domain
    │   ├── Constants/                        # Hằng số dùng chung
    │   ├── Messages/                         # Message hiển thị, exception, v.v.
    │   └── Enums/                            # Enum dùng trong toàn ứng dụng
    │
    └── UnitTest/                             # Unit test cho các phần của Application
```
