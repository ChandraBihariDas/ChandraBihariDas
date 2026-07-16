# 🎨 Design System

## Color Palette

### Primary Colors
| Name | Hex | Usage |
|:---|:---|:---|
| Cyan Neon | `#00C9FF` | Primary accent, links, highlights |
| Violet Neon | `#7B2FFF` | Secondary accent, AI/ML elements |
| Magenta Neon | `#FF006E` | Tertiary accent, urgent items |
| JavaScript Yellow | `#F7DF1E` | JavaScript emphasis (dominant) |

### Semantic Colors
| Name | Hex | Usage |
|:---|:---|:---|
| Success | `#00FF88` | Live status, available, active |
| Warning | `#FFB800` | In development, caution |
| Error | `#FF4444` | Reserved for errors |

### Neutral Colors
| Name | Hex | Usage |
|:---|:---|:---|
| Background | `#0A0A0F` | Base dark background |
| Surface | `#111118` | Card backgrounds |
| Border | `rgba(255,255,255,0.08)` | Subtle borders |
| Text Primary | `#E4E4E7` | Main text |
| Text Secondary | `#71717A` | Muted text, labels |

## Typography

### Font Stack
```
Primary: 'SF Pro Display', 'Inter', 'Segoe UI', system-ui, sans-serif
Mono:    'SF Mono', 'Fira Code', 'Cascadia Code', monospace
```

### Scale
| Level | Size | Weight | Usage |
|:---|:---|:---|:---|
| Display | 56px | 700 | Banner name |
| Heading 1 | 22px | 700 | Section titles |
| Heading 2 | 18px | 600 | Subsections |
| Body | 14px | 400 | Descriptions |
| Caption | 11-12px | 400 | Labels, metadata |
| Micro | 9-10px | 600 | Badges, tags |

## Effects

### Glassmorphism
```
Background: rgba(255, 255, 255, 0.03-0.05)
Border: rgba(255, 255, 255, 0.06-0.08)
Highlight: linear-gradient(top, rgba(255,255,255,0.04), transparent)
```

### Neon Glow
```svg
<filter id="glow">
  <feGaussianBlur stdDeviation="4-8"/>
  <feColorMatrix values="... neon color channel ..."/>
  <feMerge>
    <feMergeNode/> <!-- glow layer -->
    <feMergeNode in="SourceGraphic"/> <!-- sharp layer -->
  </feMerge>
</filter>
```

### Gradient Line
```
Left:   #00C9FF (0% opacity) → #00C9FF (full)
Center: #7B2FFF (full)
Right:  #FF006E (full) → #FF006E (0% opacity)
```

## Spacing

| Token | Value |
|:---|:---|
| Border Radius (cards) | 16px |
| Border Radius (chips) | 12px |
| Border Radius (pills) | 9999px |
| Card Padding | 16-20px |
| Section Gap | divider.svg |

## Component Patterns

### Status Badge
```
🟢 Live       → #00FF88 background
🟡 In Dev     → #FFB800 background
🔵 Learning   → #00C9FF background
🟣 Project    → #7B2FFF background
```

### Tech Chip
```
Standard:   Dark bg + subtle border + colored text
Emphasized: Solid fill (JavaScript Yellow) + dark text + glow
```

### Priority Label
```
#1: Largest card + neon gradient border + featured glow
#2: Standard card + subtle border
#3: Standard card + subtle border
```
