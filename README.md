# greco-ad-boards

Public host for **finished ad creatives** (the images that run as Meta ads for DEFENDER, ALBANOTTE and MoopTop).

Why it is public: Meta's media upload is not enabled for the ad accounts, so `ads_create_creative` needs an
`image_url` it can fetch over the open internet. These images are ads: they are seen by anyone the ad reaches.

**What belongs here:** ad board images and video thumbnails, nothing else.

**What must never be pushed here:** anything from the desk repo — briefs, ledgers, lines, reader output, order or
customer data, screenshots of the admin, credentials, unreleased product photography, notes. Those live in the
private repo `greco-desk`. If it would embarrass anyone to find it on a billboard, it does not go in this repo.

Boards are published by `tools/lines/publish_board.py` in the desk repo, which copies the file in, commits and
pushes, and prints the raw URL to hand to Meta:
`https://raw.githubusercontent.com/antoniogreco5/greco-ad-boards/main/boards/<file>`
