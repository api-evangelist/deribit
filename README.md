# Deribit

Deribit is a leading Bitcoin and Ethereum options and futures exchange offering a comprehensive REST and WebSocket API for derivatives trading, market data, portfolio management, and block trades. The platform supports futures, perpetuals, options, and spot trading across BTC, ETH, and SOL with both individual and institutional access via JSON-RPC, HTTP, and FIX protocol interfaces.

## APIs

- **REST API** - JSON-RPC over HTTP for trading operations, market data, account management, and wallet operations
- **WebSocket API** - JSON-RPC over WebSocket for real-time bidirectional communication and streaming subscriptions
- **FIX API** - Financial Information eXchange protocol for institutional low-latency trading

## Base URLs

| Environment | HTTP | WebSocket |
|---|---|---|
| Production | https://www.deribit.com/api/v2 | wss://www.deribit.com/ws/api/v2 |
| Test | https://test.deribit.com/api/v2 | wss://test.deribit.com/ws/api/v2 |

## Key Capabilities

- Futures trading (weekly and quarterly) for BTC, ETH, SOL
- Perpetual swaps across major assets
- Options trading (largest BTC/ETH options exchange)
- Block trading and Block RFQ (Request for Quote)
- Real-time market data subscriptions
- Portfolio management and account analytics
- Multi-asset wallet operations (deposits, withdrawals, transfers)
- Subaccount management
- Market Maker Protection (MMP)
- Mass quoting functionality
- Cancel on Disconnect (CoD)

## Authentication

OAuth 2.0 style authentication using Client ID and Client Secret or asymmetric signature keys. Public endpoints (market data) require no authentication. Private endpoints require an access token obtained via `public/auth`.

## Rate Limits

- 32 simultaneous connections per IP address
- 200 WebSocket messages per second (burst to 300)
- Credit-based system for authenticated users that scales with trading tier
- 8 API keys per subaccount, 16 active sessions per API key

## Resources

- Documentation: https://docs.deribit.com/
- Dev Hub: https://insights.deribit.com/dev-hub/
- Status: https://status.deribit.com/
- Support: https://support.deribit.com/hc/en-us
- Blog: https://insights.deribit.com/
