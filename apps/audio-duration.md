---
title: audio_duration
icon: screenshots/audio-duration/icon.png
screenshots:
  - screenshots/audio-duration/1.png
category: Developer Tools
summary: Get the length of an audio file like an MP3 in Flutter, in milliseconds, with one call and without playing it. For Android
tags: [Flutter, Audio duration, MP3, Android, Dart, Audio length, pub.dev, Mobile development]
website: https://github.com/p32929/flutter_audio_duration
source: https://github.com/p32929/flutter_audio_duration

platforms:
  Library: https://pub.dev/packages/audio_duration
---

audio_duration is a small Flutter package that tells you how long an audio file is, in milliseconds. Usually you have to load the file into a player and wait for it just to read its length. With audio_duration it is one call, with no playback and no listeners.

I made it for myself while building a meditation app. I cut a full meditation into pieces, like different affirmations and visualizations you can turn on or off. I wanted to know how long each piece and the whole session would be before playing it, and the default way to get that in Flutter was cumbersome.

1. **One call:** `AudioDuration.getAudioDuration(path)`.
2. **No playing needed:** it reads the length straight from the file.
3. **MP3 and more:** any format Android can read.

Great for music, podcast and recorder apps that show track lengths. It works on Android only for now.

## Install

```bash
flutter pub add audio_duration
```

```dart
var ms = await AudioDuration.getAudioDuration('/path/to/file.mp3');
```

Building a meditation, music or audio app and want a hand with it? Contact me through my portfolio: https://p32929.github.io
