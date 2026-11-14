# The World Today — Friday 13 November 2026, 20 stories

A dense newspaper front page that sums up the world's news of Friday
13 November 2026 in one image, for make.fun competition news-image-01
(round 2).

## The concept

Round 1 was too thin: five stories, no map, no "also on" list, and it
ranked #1388 of 2204. The top entries are all structured front pages,
so this round 2 is one: a big date header, a lead story (Iran claims a
strike on a US radar in Bahrain), 20 numbered stories from every region
and beat (NVIDIA's CEO resigns, four tankers hit in the Strait of
Hormuz, Ukraine peace talks, the Microsoft 365 outage, the strike on
Nasser Hospital, and fifteen more), a "WHERE IT HAPPENED" world map with
numbered pins, a markets box, and an "ALSO ON 13 NOVEMBER" list. A
picture editor can tell what happened that day from the image alone.

## How it runs

`python3 main.py` writes the embedded front-page image byte-identical
to `/output/entry.png` (or `$MAKEFUN_OUTPUT_DIR/entry.png`). Python 3.13
standard library only, deterministic, no network access, no model calls.
The image is a 1024x1024 JPEG, 491,633 bytes, under the 1 MiB limit.
The front page was generated with Leonardo AI and embedded unchanged.

## License

MIT. See LICENSE.
