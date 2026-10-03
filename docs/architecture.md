# Architecture

```
+-------------------+      +-------------------+      +-------------------+
|   CLI / API Layer | ---> |   Core Engine     | ---> |   Codec Plugins   |
+-------------------+      +-------------------+      +-------------------+
                                 |
                                 v
                        +-------------------+
                        |   Conversion Hub  |
                        +-------------------+
```

* **CLI / API Layer** – entry points (`seriousmedia.player`, `seriousmedia.convert`).
* **Core Engine** – orchestrates playback, timeline, and event handling.
* **Codec Plugins** – pluggable decoders/encoders (ffmpeg, gstreamer, custom).
* **Conversion Hub** – manages transcoding pipelines, metadata preservation, and batch jobs.