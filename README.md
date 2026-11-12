# Kho-r-c- — Vzcmusico Music Library

Public MP3 music library connected to **World Simulator OSM**.

## Official links
- Vzcmusico Music Hub: https://vzcmusico.vercel.app/
- World Simulator OSM: https://world-simulator-osm.vzcapps.vercel.app
- Vzc© Copyright Center: https://vzc-copyright-center.vercel.app/
- Vzcmusico rights notice: [VZCMUSICO-COPYRIGHT.md](VZCMUSICO-COPYRIGHT.md)
- Machine-readable track catalogue: [tracks.json](tracks.json)
- Raw manifest: https://raw.githubusercontent.com/zhaxuan92-star/Kho-r-c-/main/tracks.json

## How the connection works
World Simulator OSM reads `tracks.json` and can also discover MP3 files from the repository root. The in-game music player refreshes its library periodically and supports manual refresh. GitHub Actions scans the repository on a schedule and after MP3 uploads to regenerate the manifest.

## Uploading music
1. Add an MP3 file to this repository (root or a subfolder).
2. The scheduled/action workflow indexes MP3 files into `tracks.json`.
3. The game refreshes the manifest and makes available tracks appear in its background music player.

Only upload audio that you created or for which you have the necessary rights and permissions. A successful upload or automatic indexing does not establish permission to redistribute or synchronise the recording into a game.

## Copyright and track status
- The Vzcmusico name, library organisation, and original documentation are publisher-declared brand/library materials, only to the extent owned or controlled by the publisher.
- Individual recordings, compositions, remixes, performances, samples, and artwork remain with their respective rights holders.
- In the generated manifest, `approved: true` means included in the playback catalogue; it does **not** mean copyright clearance has been verified.
- See [VZCMUSICO-COPYRIGHT.md](VZCMUSICO-COPYRIGHT.md) before public, commercial, streamed, or monetised use.

## Licence
No blanket licence is granted for the audio files by this README. Any software or documentation licence applies only to the material expressly covered by that licence. Third-party audio remains subject to its own rights and terms.
