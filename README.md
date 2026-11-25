# MEX Mobile

**Your Jellyfin library, made for the way you watch on Android.**

[Română](README.ro.md) · [Download the beta](https://github.com/minuteoneminute/mex-mobile-releases/releases) · [Report an issue](https://github.com/minuteoneminute/mex-mobile-releases/issues)

MEX Mobile is an independent Android client for your own [Jellyfin](https://jellyfin.org/) server. Browse your films and shows, continue watching, and prepare downloads for a trip—all in an interface designed for phones.

**Status: beta.** Features are still being tested and may behave differently depending on your server, media files, Android device and network. Feedback is welcome.

## The story

MEX Mobile started with a practical need: make a personal Jellyfin library easier to use on a phone, especially when watching away from home or without a stable connection. It builds on the work of the [Jellyflix](https://github.com/jellyflix-app/jellyflix) project and adds MEX's own mobile interface and workflows for browsing, playback and downloads.

It is an **unofficial, independent client**. It is not affiliated with or endorsed by Jellyfin or Jellyflix. The app does not provide films, shows, a server or an account—you connect it to a Jellyfin server you already have access to.

## Highlights

### Find something to watch

- Browse movie and series libraries, search titles, and filter or sort the library. Search can also use actor, director or genre when the server supplies the relevant metadata.
- See watched indicators, unwatched episode counts and download badges on supported library items.
- Continue watching, see next episodes, explore recommendations and keep a watchlist. Recommendations depend on what the server returns.
- Group recently added episodes by series on the phone home screen.
- Hide selected libraries locally for a profile and show them again later. This is a display preference, not an access-control feature; it does not delete the library from the server. Existing downloads remain on the device.
- Pull down to refresh Home, Library and Downloads.

### Downloads and offline viewing

- Download supported films and episodes for offline playback, choosing **Original**, **Balanced** or **Economy**. Converted options depend on server transcoding support. File-size estimates are approximate and may be unavailable.
- Use a download queue with pause, resume, ordering, retry and an error history. Temporary interruptions can be retried automatically where supported.
- Set a storage limit, restrict transfers to unmetered networks, and optionally require charging or set a start window. Android can delay background work, and changes to transfer constraints may apply only to new downloads.
- Group episodes by series, search downloads, review storage usage, and check files before a trip. The check verifies file presence and size; it cannot guarantee full playback.
- Continue an offline title from its locally saved position. Offline viewing progress is queued for synchronization with the server when possible.
- Opt in to automatic downloads of the next one or two unwatched episodes for selected series, and protect downloads from optional automatic cleanup.

### Playback and everyday tools

- Choose available audio and subtitle tracks, set preferred languages and adjust playback quality.
- Stop playback and return to the title, lock player controls, or set a sleep timer. Continue to a subsequent episode when available.
- Use playback presets, a resume widget, connection diagnostics and optional notifications for new episodes, queue completion or server recovery.
- Choose which libraries to show for a profile, manage multiple server profiles, and use Quick Connect where supported.
- Copy a limited settings export or a diagnostic summary after reviewing it. The summary excludes account credentials, server addresses and media titles.

Some features require a connection to the server; notification timing and background work are subject to Android's restrictions. Downloaded files and app preferences live on the device unless otherwise stated. Test important downloads in airplane mode before relying on them offline.

## How does it compare with the official Jellyfin app?

Both apps connect to a Jellyfin server and let you browse and watch your own media. The [official Jellyfin Android client](https://github.com/jellyfin/jellyfin-android) integrates Jellyfin's web interface; MEX Mobile uses its own Flutter interface, based on Jellyflix, with a particular focus on the download queue, offline workflows and mobile presentation described above.

This is a difference in approach, not an exhaustive feature comparison. Features can overlap or change across versions. For example, offline and transcoded downloads are also part of the upstream [Jellyflix project](https://github.com/jellyflix-app/jellyflix). The official client has its own strengths, including Chromecast support in its proprietary distribution; choose the client that fits your setup.

## Install and connect

1. On an Android device running **Android 7.0 or newer**, open [Releases](https://github.com/minuteoneminute/mex-mobile-releases/releases) and download the newest **beta APK**.
2. Open the APK and, if Android asks, allow installation from the app you used to download it. Install MEX Mobile.
3. Enter your own Jellyfin server address and sign in with an account that can access it. There is no server address prefilled for new installations.
4. For access away from home, your server must be reachable through your own network setup. Server access and transcoding are managed by your Jellyfin installation.

To update, install a newer signed MEX Mobile APK over the existing app and confirm Android's prompt. Keep a backup of anything important and check the release notes for changes. Beta releases are listed on the Releases page and may not appear under GitHub's stable “Latest” label.

## Feedback and privacy

Please use [GitHub Issues](https://github.com/minuteoneminute/mex-mobile-releases/issues) for bug reports and suggestions. Include the app version, Android version, what you did and what happened. **Do not post passwords, access tokens, private server addresses or other sensitive information.**

## Credits and source

MEX Mobile is based on [Jellyflix](https://github.com/jellyflix-app/jellyflix), which is licensed under [GPL-3.0](https://github.com/jellyflix-app/jellyflix/blob/main/LICENSE). Thank you to the Jellyflix, Jellyfin and other open-source contributors whose work makes this project possible.

This repository currently hosts the public APK releases and documentation. The MEX Mobile source is maintained separately; the upstream Jellyflix repository does not contain the MEX-specific changes.
