# Android Methods Count

Ruby script to count dex methods in jar, aar, apk or arbitrary artifact.

## Usage

- `./android-methods-count <path-to-jar>`
- `./android-methods-count <path-to-aar>`
- `./android-methods-count <path-to-apk>`
- `./android-methods-count <artifact>`, eg. `./android-methods-count 'com.google.android.gms:play-services-location:16.0.0'`

## P.S.

Tested on macOS, but should work at any *NIX. Have not clue about Windows, but probably will not work.

Following tools should be installed:

- `ruby`, at least `2.3.7` or newer;
- `unzip` - to unpack `.apk` and `.aar`;
- `dx` - to convert `.jar` to `.dex` (this tool is bundled with Android SDK, so if you are developing for Android, you should have it);
- `cat`, `head`, `tail`, `hexdump` - sorry, I'm too lazy to convert it to native Ruby :)
