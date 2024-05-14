# Steps to reproduce

1. Copy `.env.example` to `.env` and add a WC project ID
2. Install deps (`yarn add`) and run (`yarn dev`) and open the app at `http://localhost:5173`
3. Click the connect button, copy the URI, paste it in a non-mainnet Safe (or Party) for connection
4. Open the developer console to see the logs. You'll see the correct connected address logged but an incorrect `chainId` (it's always 1 since that's the first entry in `optionalChains`)

