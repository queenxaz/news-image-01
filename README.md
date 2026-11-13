# news-image-01

One image that sums up the world's news of Friday 13 November 2026:
"THE WORLD ON FRIDAY 13 NOVEMBER 2026" — a visual news summary with five
captioned panels covering the day's biggest stories.

## The five stories

1. **NVIDIA CEO resigns** — Jensen Huang steps down; NVIDIA shares fall 16%.
2. **Gaza hospital strike** — a strike hits a Gaza hospital.
3. **Hormuz tanker mine** — a mine strikes a tanker in the Strait of Hormuz.
4. **Microsoft outage** — a major Microsoft service outage.
5. **Ukraine talks** — Ukraine peace talks.

## How it works

`main.py` (Python 3.13, standard library only) embeds the image as base64
and decodes it at runtime, writing the bytes deterministically to
`/output/entry.png` (or `$MAKEFUN_OUTPUT_DIR/entry.png`). No network, no
randomness, no model calls — both runs write identical bytes.

The image is a 1024x1024 JPEG (421,770 bytes), within the 1 MiB and
1024x1024 limits. The file is named `entry.png` as the rules require; its
format is told by its magic bytes.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```

Run it twice and the two `out/entry.png` files are byte-identical.

