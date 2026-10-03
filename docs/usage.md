# Usage

## Quick start (CLI)

```bash
# Play a video
python -m seriousmedia.player path/to/video.mp4

# Convert a video to lossless MKV
python -m seriousmedia.convert \
    --input path/to/video.mp4 \
    --output path/to/video.mkv \
    --lossless
```

## As a library

```python
from seriousmedia.player import Player
from seriousmedia.converter import Converter

player = Player()
player.load("evidence.mp4")
player.play()

converter = Converter()
converter.convert("evidence.mp4", "evidence.mkv", lossless=True)
```