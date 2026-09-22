# Tivaro-TV

Tivaro-TV is a remote-first Android TV and Fire TV player for customers using credentials supplied by their legal IPTV provider.

## Download

[Download Tivaro-TV 0.2.7](releases/Tivaro-TV-0.2.7.apk)

Version 0.2.7 makes movie and show detail controls immediately navigable before trailers begin, returns Back to the exact originating Movies or Shows position, corrects featured-title line spacing, and replaces the poster-ribbon startup background with a clean black Tivaro logo-and-name reveal with a left-to-right shine. Live TV, playback, updater, manifests, admin, and login remain unchanged. Future updates are downloaded automatically when Tivaro-TV opens; Fire OS requires one-time permission for Tivaro-TV to install updates and then asks the user to confirm each installation.

The application does not include IPTV credentials or channel lists. A valid provider profile is required before its interface unlocks.

## Managed catalog registry

`addon-registry.json` is generated and cryptographically signed by the Tivaro-TV Admin utility. Customer installations reject modified remote registries and keep the last verified copy when GitHub or an add-on is temporarily unavailable.

The initial registry contains metadata/catalog and subtitle services only. It does not bundle torrent scrapers, piracy providers, IPTV subscriptions, or private access tokens.

Movie and show playback is resolved only through enabled admin-managed add-ons that return authorized direct stream URLs. IPTV provider connections are used only for account validation and live channels.
