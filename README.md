# williamshillsoftware.com

Static site for Williams Hill Software (the app's store name is
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
| `cardiacstudy-player/media/ct.jpg` | `build/store-screenshots/5-ct.png` (tools/store_screenshots.sh), saved as JPEG |

`badges/` holds Apple's unaltered "Download on the Mac App Store" badges
(toolbox.marketingtools.apple.com, black for light mode, white for dark).
