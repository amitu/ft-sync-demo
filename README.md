# ft-sync-demo
This repo contains Docs related to ft-sync.


## Steps to sync local document to fifthtry
- Create a collection on FifthTry

- Create a `ft-sync.p1` config file
```
-- ft-sync:
mode: local-to-remote
backend: ftd
root: docs
repo: https://github.com/abrarNitk/ft-sync-demo 
collection: amitu/ftsync-demo

-- ignored:
**/*.py

```
- Set ENV variable FT_AUTH_CODE=**** and FT_HOST=https://www.fifthtry.com
- Status Command `./ft-sync --config=ft-sync.p1 status`
- Sync Command `./ft-sync --config=ft-sync.p1 sync`