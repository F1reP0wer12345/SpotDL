# SpotDL Binaries
My Kodi addon plugin.audio.spotdl doesn't work with the prebuilt spotdl binaries, because they require python to be installed.
After compiling spotdl with poetry with no changes made, it runs even when python isn't installed.
I also included ffmpeg, because you need it in a certain directory in order for my addon to work.
My addon will ask to download these files. If you don't trust them, compile them for your self. Here are the instructions:

```bash
git clone https://github.com/spotDL/spotify-downloader && cd spotify-downloader
pip install poetry
poetry install
poetry run python3 scripts/build.py
```
 
