# Set up your GitHub profile README

This package is intended for the special public profile repository named **`VinayCodes17`** under the GitHub account **`VinayCodes17`**.

## 1. Copy the files

Upload the contents of this folder to the root of `https://github.com/VinayCodes17/VinayCodes17`:

```text
VinayCodes17/
├── README.md
├── PROFILE-SETUP.md
├── assets/
│   ├── hero-banner.jpg
│   └── system-map.svg
└── .github/
    └── workflows/
        ├── snake.yml
        └── profile-3d.yml
```

The repository should be public for the profile README to appear on your GitHub profile.

## 2. Enable workflow write permissions

In the profile repository, open **Settings → Actions → General → Workflow permissions** and enable **Read and write permissions**. The workflows also declare `contents: write` explicitly.

## 3. Generate the contribution snake

1. Open the **Actions** tab.
2. Select **Generate contribution snake**.
3. Choose **Run workflow**.
4. After it completes, it publishes `github-snake.svg` and `github-snake-dark.svg` to the `output` branch.

The README references the dark SVG at:

```text
https://raw.githubusercontent.com/VinayCodes17/VinayCodes17/output/github-snake-dark.svg
```

To display the snake in the README, add this where you want it:

```html
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/VinayCodes17/VinayCodes17/output/github-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/VinayCodes17/VinayCodes17/output/github-snake.svg" />
    <img src="https://raw.githubusercontent.com/VinayCodes17/VinayCodes17/output/github-snake.svg" alt="GitHub contribution snake" />
  </picture>
</p>
```

## 4. Generate the 3D contribution calendar

1. Open the **Actions** tab.
2. Select **Generate 3D contribution calendar**.
3. Choose **Run workflow**.
4. When the workflow finishes, it commits generated SVGs into `profile-3d-contrib/`.

The README uses `profile-3d-contrib/profile-night-view.svg`. The action also produces other styles, including animated and green variants.

## 5. Personalize the project and contact details

Before publishing, review `README.md`:

- Confirm the education and achievement wording is accurate.
- Add direct repository links to OceanEmbed and any other projects you want to feature.
- Add your LinkedIn URL and a public contact email if you want them displayed.
- Remove any technology that no longer reflects what you're actively using.
- Keep the “Currently Exploring” list separate from your core stack until you have hands-on experience.

## Notes

- The hero image and architecture illustration are local assets, so they do not depend on an external image-hosting service.
- Typing SVG, skill icons, shields and analytics cards use third-party services. If one is unavailable, replace or remove that image.
- GitHub README files do not run arbitrary JavaScript or embedded 3D WebGL scenes. These workflows generate static SVG assets that GitHub can display.
- The stats cards are community-hosted services, not official GitHub analytics endpoints. Their availability and rate limits can change.
