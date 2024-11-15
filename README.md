This program is deployed and verified at: FWEYpBAf9WsemQiNbAewhyESfR38GBBHLrCaU3MpEKWv

Verify command:

```bash
solana-verify verify-from-repo https://github.com/Woody4618/crispy-waffle --program-id FWEYpBAf9WsemQiNbAewhyESfR38GBBHLrCaU3MpEKWv --mount-path  waffle
```

Notice how the program is in the `waffle` directory and the workspace has a member `waffle` that points to the program.
Also its important that the lib-name in the Cargo.toml is `waffle` and the program name is `waffle.so`
The verify command then uses the `--mount-path` flag to specify the directory where the program is located.

Find the program in the Solana Explorer here:
https://explorer.solana.com/address/FWEYpBAf9WsemQiNbAewhyESfR38GBBHLrCaU3MpEKWv?cluster=mainnet

Find the verify docs here:
https://solana.com/developers/guides/advanced/verified-builds

And the code here:
https://github.com/Ellipsis-Labs/solana-verifiable-build
