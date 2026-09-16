# Tivaro-TV

Tivaro-TV is a remote-first Android TV and Fire TV player for customers using credentials supplied by their legal IPTV provider.

## Download

[Download Tivaro-TV 0.1.7](releases/Tivaro-TV-0.1.7.apk)

Version 0.1.7 improves Fire TV remote navigation and restores the exact Live TV category/channel position after playback. It adds hold-to-confirm Favorites and history actions, two-second Live TV overlay hiding, predictable far-left vertical catalog navigation, and more reliable movie/show stream discovery when configured add-ons share an internal ID. Future updates are downloaded automatically when Tivaro-TV opens; Fire OS then asks the user to confirm installation.

The application does not include IPTV credentials or channel lists. A valid provider profile is required before its interface unlocks.

## Managed catalog registry

`addon-registry.json` is generated and cryptographically signed by the Tivaro-TV Admin utility. Customer installations reject modified remote registries and keep the last verified copy when GitHub or an add-on is temporarily unavailable.

The initial registry contains metadata/catalog and subtitle services only. It does not bundle torrent scrapers, piracy providers, IPTV subscriptions, or private access tokens.

Movie and show playback is resolved only through enabled admin-managed add-ons that return authorized direct stream URLs. IPTV provider connections are used only for account validation and live channels.
