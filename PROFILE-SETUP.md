# Profile setup

## Files to upload

Copy this folder's contents to the root of the public profile repository `VinayCodes17/VinayCodes17`:

```text
VinayCodes17/
├── README.md
└── .github/
    └── workflows/
        └── contribution-fx.yml
```

## Enable the animation workflow

1. Open **Settings → Actions → General** in the profile repository.
2. Under **Workflow permissions**, allow **Read and write permissions**.
3. Open **Actions → Animate contribution graph → Run workflow**.
4. After it succeeds, the workflow publishes two generated SVG files to the `output` branch.
5. The README will load those files automatically.

The action refreshes the artwork daily. To change the visual effect, edit the `theme`, `palette`, or `speed` query values in `contribution-fx.yml`.

## GitCity: interactive 3D city

GitCity does **not** need a GitHub Action, token, or generated local image. The README uses its live SVG preview as a clickable link. Clicking it opens the full GitCity experience for `VinayCodes17`, where the contribution history can be explored in 3D and the city simulation can be driven.

GitHub profile READMEs do not support embedding the live Three.js experience with an iframe. The clickable preview is the practical README-compatible approach.

## Removed from the previous version

- `profile-3d.yml`: replaced by GitCity, which has an interactive 3D city and a driveable simulation.
- `snake.yml`: replaced by the animated contribution-fx widget to avoid stacking multiple versions of the same contribution graphic.
- Generated hero artwork and static architecture artwork: removed; this version uses live widgets and no AI-generated images.

## Before publishing

Check that the GitHub account is `VinayCodes17`. Review the skills shown in the icon strip and remove any tools you no longer use. Add a LinkedIn or portfolio link only when you have the exact public URL.
