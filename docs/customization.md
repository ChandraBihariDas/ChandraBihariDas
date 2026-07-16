# 🎨 Customization Guide

## Changing Your Information

### Name & Role
In `README.md`, find and replace:
- `Utkarsh Tripathi` → Your name
- `JavaScript Full Stack Developer` → Your role
- `AI Engineer` → Your secondary role
- `ChandraBihariDas` → Your GitHub username

### Social Links
Update the badge URLs in the Connect section:
```markdown
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](YOUR_LINKEDIN_URL)
```

### Projects
Edit the Featured Projects section with your own project details. Update:
- Project names and descriptions
- Repository URLs
- Live demo URLs
- Tech stack pills
- Status badges

### Hackathons
Update the achievements table with your verified accomplishments only.

## Changing Colors

The design system uses these primary colors. To change the theme, update these values across all SVG files and README badges:

| Token | Current | Your Value |
|:---|:---|:---|
| Primary Neon | `#00C9FF` | |
| Secondary Neon | `#7B2FFF` | |
| Accent | `#FF006E` | |
| TypeScript | `#3178C6` | |
| Success | `#00FF88` | |
| Warning | `#FFB800` | |
| Background | `#0A0A0F` | |
| Text | `#E4E4E7` | |
| Muted | `#71717A` | |

### Badge Colors
For shields.io badges, update the `color` and `labelColor` parameters:
```markdown
![Badge](https://img.shields.io/badge/Label-Text-COLOR?style=for-the-badge&labelColor=LABEL_COLOR)
```

### Stats Theme
For GitHub stats cards, update the color parameters:
```markdown
![Stats](https://github-readme-stats.vercel.app/api?username=YOUR_USERNAME&bg_color=0A0A0F&title_color=00C9FF&icon_color=7B2FFF&text_color=E4E4E7)
```

## Changing SVG Assets

See [assets-guide.md](./assets-guide.md) for instructions on modifying each SVG file.

## Adding New Sections

To add a new section, follow this pattern:
```markdown
<!-- DIVIDER -->
<img src="./assets/divider.svg" width="100%"/>

## 🆕 Your New Section

Content here...
```

Always use the divider SVG between sections for visual consistency.
