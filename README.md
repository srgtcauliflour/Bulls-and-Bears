# Bulls&Bears

Cross-browser market decision-support extension using Massive market data and TypeSafe Jev.

## Current milestone
- Core/Chrome: **v0.2.1 refactor**
- Safari iOS: **v0.1 bootstrap**
- Shared WebExtension resources: `extension/`
- Safari packaging/build: GitHub Actions on macOS

## Architecture
Massive observed data → deterministic feature engine → normalized Jev state → independent typed judgments → Bulls&Bears UI.

Arithmetic, indicators, freshness and trade-plan calculations stay in code. Jev supplies narrow semantic judgments. Noul values are Jev decision probabilities, not empirically validated probabilities of market movement or profit.

## Chrome
Open `chrome://extensions`, enable Developer mode, Load unpacked, select `extension/`.

## Safari iOS
Run the **Safari iOS unsigned IPA** workflow. It packages the shared extension with Apple's Safari Web Extension packager, builds the iOS container without signing, and publishes an unsigned IPA artifact for signing/testing.

## Future Page Intelligence
The planned Analyse This Page layer will read a page only after user permission/action, extract candidate symbol/asset/timeframe with provenance, confirm ambiguity, retrieve authoritative market data from Massive, and send a compact normalized state to Jev. It will not dump arbitrary page contents into Jev.

## Disclaimer
Decision support only, not financial advice. Model outputs can be wrong and require historical validation/calibration.
