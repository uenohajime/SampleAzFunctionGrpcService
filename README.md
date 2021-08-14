# Sample Azure Function with gRPC Service

## ディレクトリ構造

```
SampleAzFunctionGrpcService.sln
  |-- SampleAzFunctionGrpcService # gRPC サーバ・プロジェクト
  |-- GrpcClientConsoleApp # gRPC クライアント・プロジェクト（コンソールアプリ）
  |-- GrpcClientAzFunctionApp # gRPC クライアント・プロジェクト（Azure Function アプリ）
```

## Azure Function で gRPC サーバへアクセスする手順

1. Visual Sutdio を 2 つ立ち上げ、 SampleAzFunctionGrpcService.sln ファイルをそれぞれの Visual Studio で開く
2. 一方の Visual Studio で SampleAzFunctionGrpcService をデバッグの開始
3. もう一方の Visual Studio で GrpcClientAzFunctionApp をデバッグの開始
4. Web ブラウザで Azure Function の HTTP トリガーが定義されている URL ( http://localhost:7071/api/Function1 ) へアクセスすると、「Hello GreeterClient」と表示される

## 参考サイト

* [チュートリアル: ASP.NET Core で gRPC のクライアントとサーバーを作成する](https://docs.microsoft.com/ja-jp/aspnet/core/tutorials/grpc/grpc-start?view=aspnetcore-5.0&tabs=visual-studio)
