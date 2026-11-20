# williamshillsoftware.com

Static site for Williams Hill Software LLC (the app's store name is
"CardiacStudy: DICOM Viewer"; installed, it is "CardiacStudy Player"), served by GitHub Pages (custom domain
in `CNAME`; `.nojekyll` serves the files as-is).

| Page | URL | Used for |
| --- | --- | --- |
| `index.html` | https://williamshillsoftware.com/ | Developer home |
| `cardiacstudy-player/index.html` | https://williamshillsoftware.com/cardiacstudy-player/ | App Store **Support URL** and **Marketing URL** |
| `cardiacstudy-player/privacy.html` | https://williamshillsoftware.com/cardiacstudy-player/privacy.html | App Store **Privacy Policy URL** |

These files are copies from the MacAngioViewSwift repo; re-copy them when the
originals change:

| Site file | Source |
| --- | --- |
| `cardiacstudy-player/DICOM_CONFORMANCE.pdf` | `docs/DICOM_CONFORMANCE.pdf` |
| `cardiacstudy-player/CardiacStudyPlayer-Cardiology-Training-Guide.pdf` | `docs/CardiacStudyPlayer-Cardiology-Training-Guide.pdf` |
| `cardiacstudy-player/icon.png` | `tools/app_icon_1024.png`, scaled to 256 px |
| `cardiacstudy-player/media/*.jpg` (screenshots) | `build/store-screenshots/*.png` (tools/store_screenshots.sh), saved as JPEG (`sips -s format jpeg -s formatOptions 82`) |
| `cardiacstudy-player/media/preview-*.mp4` | `build/store-previews/*.mov` (the App Store previews), `avconvert --preset Preset960x540` |
| `cardiacstudy-player/media/poster-*.jpg` | the preview's frame at 3 s |
| `cardiacstudy-player/windows/*.pdf` | WinAngioViewSwift `docs/windows/*.pdf` |

`badges/` holds the stores' unaltered badges: Apple's "Download on the Mac App
Store" (toolbox.marketingtools.apple.com, black for light mode, white for
dark) and Microsoft's "Get it from Microsoft" (get.microsoft.com/images,
`en-us dark.svg` for light mode, `en-us light.svg` for dark).

The Versions section on the product page is written by hand: update it with
each release. The Mac version number also updates itself from Apple's lookup
API.

## Documents: always the latest

The training guides and conformance statements here are always the newest
versions, even when the copy bundled in a store build is older. Each time one
is re-rendered (in MacAngioViewSwift `docs/` or WinAngioViewSwift
`docs/windows/`), copy it here, keep its file name, and update its row in the
product page's Documentation table: the date or version in the link text,
and the same in the link's `?v=` (the guide's date, the conformance
statement's document version). The query string shows the version in the URL
and makes browsers fetch the new copy instead of a cached one.
