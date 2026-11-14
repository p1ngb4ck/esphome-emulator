# `pr/emulator`

One part of the topic repo p1ngb4ck/esphome-emulator. The whole topic, with its description, is the branch `main`.

Change of this branch: `emulator`: the game emulator app - one non-blocking PPA pass per frame into the video output's rows, the scale stepped down by the measured pass time (kept per system), systems gated by the screen size at build time (`min_scale`), keys through LVGL's key bindings, save files / states through the storage worker, players, link

Based on these branches, whose changes it holds and builds on:

- `pr/display-video-output-rows` of p1ngb4ck/esphome-esp-video: display: `open_rows`, `rows_begin` / `rows_end` for a writer of its own, `rotation()`, `display()`
- `pr/storage` of p1ngb4ck/esphome-storage-interface: the `storage` component: registry, path / filesystem / network / raw storages, the asynchronous worker (jobs, streams), `storage.*` actions, PSRAM transfer buffer, change feed, ISO 9660 mount
