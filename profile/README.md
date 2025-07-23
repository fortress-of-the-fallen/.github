.
└── Source/
    ├── GameClient/
    │   └── Bootstrap/
    │       └── AddDependenciesInjection.cs   # Add all denpendency
    ├── Adapter/
    │   ├── Signals/ 
    │   │   └── <ServiceName>/
    │   │       ├── ReqModel.cs # _signalBus.Fire(Mapper.map<ReqDto>(ReqModel))
    │   │       └── ResModel.cs # Mapper.map<ResModel>(reqDto)
    │   ├── Mapper/
    │   └── SignalsRegister.cs
    └── Application/
        ├── Service/
        │   └── <ServiceName>/
        │       ├── ReqModel
        │       ├── ResModel
        │       └── <ServiceName>.cs # Include 1 interface 1 class impl interface
        ├── External/
        │   ├── API
        │   ├── Storage
        │   └── Logger
        ├── Repository/
        ├── Domain/
        │   ├── Entities
        │   ├── Constants
        │   ├── Messages
        │   └── Enums
        └── UnitTest/
