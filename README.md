
### 実行例

```
$ cargo run --bin helloworld-server
$ grpcurl -plaintext -import-path ./proto -proto helloworld.proto -d '{"name": "Tonic"}' '[::]:50051' helloworld.Greeter/SayHello
```

### 説明

https://github.com/284km/helloworld-tonic_20240906/blob/main/Cargo.toml

tonic:
https://github.com/hyperium/tonic
A native gRPC client & server implementation with async/await support

prost:
brotobuf を rust で使用するための library
.proto ファイルを解析して、対応する rust の型定義や構造体を生成する。
いつも go でやっているのと同じ！

tokio
rust の非同期 runtime


