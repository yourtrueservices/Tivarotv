# Tivaro-TV

Tivaro-TV is a remote-first Android TV and Fire TV player for customers using credentials supplied by their legal IPTV provider.

## Download

[Download Tivaro-TV 0.2.5](releases/Tivaro-TV-0.2.5.apk)

Version 0.2.5 restores exact one-step focus and scroll return across browsing, details, playback, Favorites, and Live TV; smooths D-pad rails; simplifies history-removal dialogs; persists subtitle choices; adds a final-150-second next-episode prompt and automatic episode advance; and improves Continue Watching details and server focus. Live TV playback sources, login, providers, and admin manifests remain unchanged. Future updates are downloaded automatically when Tivaro-TV opens; Fire OS then asks the user to confirm installation.

The application does not include IPTV credentials or channel lists. A valid provider profile is required before its interface unlocks.

## Managed catalog registry

`addon-registry.json` is generated and cryptographically signed by the Tivaro-TV Admin utility. Customer installations reject modified remote registries and keep the last verified copy when GitHub or an add-on is temporarily unavailable.

The initial registry contains metadata/catalog and subtitle services only. It does not bundle torrent scrapers, piracy providers, IPTV subscriptions, or private access tokens.

Movie and show playback is resolved only through enabled admin-managed add-ons that return authorized direct stream URLs. IPTV provider connections are used only for account validation and live channels.
