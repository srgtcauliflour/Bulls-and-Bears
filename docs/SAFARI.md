# Safari iOS v0.1

The canonical WebExtension is `extension/`. CI invokes Apple's Safari Web Extension packager to generate the Xcode project instead of committing generated boilerplate.

The Safari workflow validates JS, packages an iOS-only Safari Web Extension, discovers the generated iOS scheme, builds with signing disabled, wraps the .app in Payload/, and uploads an unsigned IPA artifact.

v0.1 scope is manual Stock / Forex / Crypto analysis. Page reading is deliberately deferred until explicit permission UX and site adapters exist.
