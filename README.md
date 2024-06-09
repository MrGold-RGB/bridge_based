# bridge_based

Create BINANCE/TON bridge management service on node.

Methods list:

1. create_ton_wrapped_token: Creates wrapped token from BNB to TON: { token contract address }
Creates wrapped coin contract on TON with methods: send, mintToAddress, burn

2. bridge_token_to_ton: Bridge token from BNB to TON: {amount, token contract address, TON address}
Receives token on BNB chain and stores it in contract, then mint same amount of wrapped token on TON and send it to TON address.

3. return_token_to_bnb: Return token from TON to BNB: {amount, token contract address, BNB address}
Receives token on TON chain and burns it, then send same amount of token to BNB address.


