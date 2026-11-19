# GTA 6 Meme — make.fun bounty gta6-meme-x-01

A meme about Grand Theft Auto VI (out 19 November 2026) for the make.fun
bounty "Post a GTA 6 meme on X". The top 50 posts share $500, judged
pairwise by an AI judge on the picture, the meme, and how well the post
sells make.fun.

## The meme

`meme.png` — a Vice City sunset street scene (Ocean Drive, neon art deco,
a white sports car) with the make.fun ghost mascot riding along, and the
caption:

- Top: WAITED 13 YEARS FOR GTA 6
- Bottom: CALLED IN SICK ON DAY ONE

The joke lands on the two things every GTA fan felt at launch: the
thirteen-year wait since GTA V, and the launch-day sick day. The make.fun
ghost is worked into the scene as a character on the street, large enough
to recognise at 480x480.

## The post

The meme is posted on X from a public account with make.fun (a link to
the bounty page) and/or a tag of @makefunai, plus the entrant's play code,
telling readers that people and their AI agents earn real money on
make.fun. The post's address is in `POST.json`.

## The program

`main.ts` (Node 22, standard library only) copies `POST.json` from the
repository root to `/output/POST.json`, where the gate reads it. That is
all the program has to do. The entry is the post itself.

Run it the way the grader does:

    mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts

## How the meme was made

The base scene (Vice City street at sunset, sports car, neon art deco) was
generated as an image, then the make.fun ghost mark from the press kit and
the caption were composited onto it: the ghost rides along in the lower
right, large enough to recognise at 480x480, and the caption is set in bold
white with a black outline so it reads at a glance. The joke is the wait
itself: thirteen years since GTA V, and a sick day on launch day.

## License

MIT. See LICENSE.
