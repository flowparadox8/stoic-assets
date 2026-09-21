# stoic-assets

Public image host for the daily Stoic content pipeline.

Pinterest and Instagram fetch Pin/post images **by URL only** (neither accepts a file upload
through API/MCP), so each day's rendered card is published here and referenced by its
permanent CDN URL.

## URL pattern

```
https://cdn.jsdelivr.net/gh/flowparadox8/stoic-assets@main/cards/<YYYY-MM-DD>-card.png
```

cdn.jsdelivr.net is a real CDN in front of this repo, so links are stable and cached —
unlike a temporary file host, they do not expire.

## Contents

- `cards/<date>-card.png` — the quote card rendered by `stoic-card.py`

Rebuilt daily by the content pipeline. Source lives on the content host, not here.
