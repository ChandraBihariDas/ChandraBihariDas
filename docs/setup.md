# ⚙️ Setup Guide

## Prerequisites

- A GitHub account
- A repository named **exactly** your GitHub username (e.g., `ChandraBihariDas/ChandraBihariDas`)
- Git installed locally

## Step 1: Create the Profile Repository

If you haven't already:
```bash
# Create the repository on GitHub with your exact username
# Then clone it
git clone https://github.com/YOUR_USERNAME/YOUR_USERNAME.git
cd YOUR_USERNAME
```

## Step 2: Copy the Files

Copy the entire structure into your repository:
```
├── README.md
├── assets/
│   ├── logo.svg
│   ├── banner.svg
│   ├── background.svg
│   ├── divider.svg
│   ├── footer.svg
│   ├── profile-card.svg
│   ├── projects.svg
│   ├── tech-icons.svg
│   └── timeline.svg
├── docs/
└── .github/workflows/
```

## Step 3: Customize Your Information

Edit the following in `README.md`:
- Name and role
- Social links (LinkedIn, email, etc.)
- Project details and URLs
- Hackathon achievements
- Tech stack badges

See [customization.md](./customization.md) for detailed instructions.

## Step 4: Enable GitHub Actions

1. Go to your repository → **Settings** → **Actions** → **General**
2. Set "Workflow permissions" to **Read and write permissions**
3. Go to the **Actions** tab
4. Manually trigger each workflow once via "Run workflow"

## Step 5: Wait for Assets to Generate

Some workflows generate output files:
- **Snake animation**: Generates to the `output` branch (~1 minute)
- **Metrics**: Generates SVG to the repository (~2 minutes)
- **Profile summary**: Generates cards (~2 minutes)

## Step 6: Push and Verify

```bash
git add .
git commit -m "feat: premium GitHub profile setup"
git push origin main
```

Visit your GitHub profile at `https://github.com/YOUR_USERNAME` to verify everything renders correctly.

## Troubleshooting

| Issue | Solution |
|:---|:---|
| SVGs not rendering | Ensure SVGs are committed, not gitignored |
| Snake not showing | Run the snake workflow manually, wait for `output` branch |
| Stats showing wrong data | Stats services cache — wait 24 hours |
| Badges not loading | Check shields.io status at `status.shields.io` |
| Actions failing | Check workflow permissions in repository settings |
