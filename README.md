# Advanced-Avalanche_Module-2

## changes made in the consts.go file

```

const (
	// TODO: choose a human-readable part for your hyperchain
	HRP = "RABBIT"
	// TODO: choose a name for your hyperchain
	Name = "PRATAP"
	// TODO: choose a token symbol
	Symbol = "PRO"
)
```

## changes made in the registry.go file

```
// TODO: register action: actions.CreateAsset
consts.ActionRegistry.Register(&actions.CreateAsset{}, actions.UnmarshalCreateAsset, false),
// TODO: register action: actions.MintAsset
consts.ActionRegistry.Register(&actions.MintAsset{}, actions.UnmarshalMintAsset, false),
```

## Step by Step project implementation:

1. Clone the initial repository
2. Inside your project folder, run go mod tidy to normalize all the dependencies
3. Configure your project constants
    Go to consts/consts.go and add the missing parts.
3. Register the Create_Asset and Mint_Assest actions in registry/registry.go
4. Run your VM locally
5. Make sure Go is on your path, defined on your terminal, if not you can do so by running export PATH=$PATH:$(go env GOPATH)/bin
6. Run MODE="run-single" ./scripts/run.sh
7. Run ./scripts/build.sh
8. Load the demo private key included on the project ./build/token-cli key import demo.pk and ./build/token-cli chain import-anr
9. Interact with your own HyperChain.
10. To close your Local Avalanche Network run killall avalanche-network-runner.

## Author
Pratap Singh
