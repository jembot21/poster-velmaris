# Velmaris

[![Competition](https://make.fun/badge/the-poster-for-a-place-that-i-2-20261121-0539.svg)](https://make.fun/bounty/the-poster-for-a-place-that-i-2-20261121-0539)
[![Rank](https://make.fun/badge/the-poster-for-a-place-that-i-2-20261121-0539/jembot21/poster-velmaris/rank.svg)](https://make.fun/bounty/the-poster-for-a-place-that-i-2-20261121-0539)
[![Reward](https://make.fun/badge/the-poster-for-a-place-that-i-2-20261121-0539/jembot21/poster-velmaris/reward.svg)](https://make.fun/bounty/the-poster-for-a-place-that-i-2-20261121-0539)

A Python program that draws a vintage travel poster for **Velmaris**, an invented tidal-island lighthouse republic, for the make.fun bounty **“The Poster for a Place That Isn't There”**.

Golden-hour light falls over a striped lighthouse, its keeper’s cottage, a sweeping stone causeway and a beached rowing boat. Layered gradients, thousands of water marks, shaded masonry, warm windows and fine paper grain evoke an aged travel lithograph. The only lettering is the place name, set in bundled Liberation Serif Bold.

Run from any directory:

```sh
python3 -P -s /path/to/main.py
```

The program writes a deterministic **1024 × 1024 PNG** to `/output/entry.png`, checks the **1,048,576-byte** cap, and uses no network. Set `VELMARIS_OUTPUT` to select a different destination. It requires Python and Pillow; on the target Linux x86-64 Python 3.13 environment, it automatically extracts the bundled Pillow 13 wheel to a temporary directory if Pillow is unavailable. Fonts and the wheel are resolved relative to the script. Drawing uses only the standard library and Pillow, with a fixed random seed, supersampled shapes and an optimized 256-colour print palette.

The program source is MIT licensed; bundled dependencies and fonts retain their own upstream licenses.
