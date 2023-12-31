# flwr Swift pod

This is a pod for your flower application. You could use it in your flutter application as well

## Installation

You can download the Flower project and integrate the package manually.

## Usage

A comprehensive example is available in: [```examples/ios/```](https://github.com/adap/flower/tree/main/examples/ios). To give information about the usage structurally: 

```
import flwr

...
let mlFlwrClient = MLFlwrClient(layerWrappers: layerWrappers, dataLoader: dataLoader, compiledModelUrl: compiledModelUrl)
let flwrGRPC = FlwrGRPC(serverHost: hostname, serverPort: port)
startFlwrGRPC(client: mlFlwrClient) {
    // completion handler
    print("Federated learning completed")
}
...
```

## Dependencies

1. grpc-swift https://github.com/grpc/grpc-swift
2. NumPy-iOS https://github.com/kewlbear/NumPy-iOS
3. PythonKit https://github.com/pvieito/PythonKit

## License

MIT
