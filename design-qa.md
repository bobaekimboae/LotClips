# Design QA

## Compared scope

- Source: LotClips logged-in upload form at 390 × 844, including the empty and three-photo states.
- Implementation: deployed LotClips upload form at 390 × 844, including the empty and three-photo states.
- Checked: dark layout, sidebar/bottom navigation, listing URL row, photo drop zone, uploaded photo rows, vehicle fields, feature chips, preview action, and three-photo ordering state.

The upload form was adjusted after live review to use the source's flat numbered photo rows and the captured source icons. The three uploaded photos displayed their filenames and sizes, and the feature controls remained selectable.

## Blocker

The source's **Preview Video** action was intentionally not activated. Its account showed one free-trial video remaining, and the user authorized inspection and photo upload without creating a source video or spending that credit. Therefore the original preview/result screen and any behavior after that action could not be captured or compared. The local clone's preview screen is a functional, independent video renderer and is not verified as a visual match for the unseen original result screen.

## Verification evidence

- Deployed build: GitHub Actions run completed successfully.
- Three test photos uploaded to the clone; filenames, preview thumbnails, and sizes displayed.
- Generated a 720 × 1280 MP4 of about 8.4 seconds, opened it in the preview, and downloaded a 1.1 MB `.mp4` file.
- The original LotClips page still contains the three approved test photos in its upload form. No source project or video was generated, and no trial credit was spent.

final result: blocked
