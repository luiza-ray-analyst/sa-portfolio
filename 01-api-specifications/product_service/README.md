# ProductService API

gRPC/Protobuf контракт для CRUD-операций с товарами.

## Требования
- Авторизация через AuthData
- Идемпотентность создания через idempotency_key
- Единый формат ответа: status + meta_info

## Генерация кода
```bash
protoc --go_out=./pb --go-grpc_out=./pb product_service.proto