# gpui-pre-wgpu (sqm patch)

`gpui-pre-wgpu` 0.3.7 from crates.io (a republish of Zed's `gpui_wgpu`, Apache-2.0) with one change: the atlas sampler magnifies with `Nearest`, so enlarged pixel art stays crisp. Minification stays `Linear`.

Used by [sqm](https://github.com/lgrossi/sqm) via `[patch.crates-io]`. To upgrade: replace the tree with the new published version, re-apply the one-line change in `src/wgpu_renderer.rs`, bump the tag. Delete this repo once upstream GPUI offers a sampling option.
