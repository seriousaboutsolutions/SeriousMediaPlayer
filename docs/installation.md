# Installation

```bash
# 1. Clone the repo
git clone https://github.com/seriousaboutsolutions/SeriousMediaPlayer.git
cd SeriousMediaPlayer

# 2. Create a virtual environment
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. (Optional) Install FFmpeg for conversion support
#    On macOS: brew install ffmpeg
#    On Ubuntu: sudo apt-get install ffmpeg
```

> **Note:** The player requires Python 3.9+ and a recent version of FFmpeg for video conversion.