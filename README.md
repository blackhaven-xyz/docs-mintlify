# Blackhaven Documentation

Official documentation for Blackhaven—the reserve-backed liquidity engine powering sustainable rewards and reserve growth across the MegaETH ecosystem.

![Blackhaven](https://img.shields.io/badge/Blackhaven-MegaETH-D4FFAF?style=for-the-badge)

## 🌐 Live Documentation

**[View Documentation →](https://docs.blackhaven.fi)**

## 📁 Project Structure

```
├── overview.mdx              # Landing page
├── mint.json                 # Site configuration & navigation
├── bunny.js                  # Interactive mascot
├── bunny-config.json         # Mascot dialog configuration
├── styles/
│   └── global.css            # Custom styling & theme
├── rbt/                      # RBT Token documentation
│   ├── overview.mdx
│   └── notes.mdx
├── products/                 # Product documentation
│   ├── haven-protected-notes.mdx
│   ├── fixed-term-bonds.mdx
│   └── blackhaven-dex.mdx
├── reserves/                 # Reserve documentation
│   ├── overview.mdx
│   └── bam.mdx
└── resources/                # Additional resources
    ├── risks.mdx
    └── glossary.mdx
```

## 🚀 Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/fattybagz/BlackHavenDocs.git
cd BlackHavenDocs
```

2. Install the Mintlify CLI:
```bash
npm i -g mintlify
```

3. Start the development server:
```bash
mintlify dev
```

4. Open [http://localhost:3000](http://localhost:3000) in your browser.

## 🎨 Customization

### Theme Colors

The documentation uses a custom dark theme with Blackhaven brand colors:

| Color | Hex | Usage |
|-------|-----|-------|
| Haven Night | `#0A0C14` | Background |
| Ozone Green | `#D4FFAF` | Primary accent |
| Sidebar | `#07080D` | Navigation background |

Colors are defined in `styles/global.css` under the `:root` CSS variables.

### Navigation

Edit `mint.json` to modify:
- Page order and grouping
- Navigation structure
- Footer social links
- Site metadata

## 🐰 Bunny Mascot

The interactive bunny mascot provides an engaging user experience with random facts, sleep cycles, and reactions.

### How It Works

The bunny has three states:
- **Awake** - Idle with subtle head bob animation, random blinking
- **Sleeping** - Breathing animation with ZzZ effects and dream bubbles
- **Angry** - Turns red when disturbed while sleeping

### Toggle Button

A carrot toggle button (🥕) in the bottom-right corner allows users to show/hide the bunny:

- **Click to toggle** - Bunny hops in/out with animation
- **Persists preference** - Saved to localStorage
- **🥕 bright** = Bunny visible
- **🥕 dimmed** = Bunny hidden

When hiding, all elements (dialog, ZZZs, dream bubbles) are immediately cleared before the bunny hops out.

### Configuring Dialog Phrases

Edit `bunny-config.json` to customize the bunny's dialog:

```json
{
  "phrases": [
    "RBT backing grows as reserves grow",
    "HPNs are principal-protected",
    "52-week Note = 52% yield",
    "Built for MegaETH 🚀",
    "Bonds give you discounted RBT",
    "Reserves = protocol-owned liquidity",
    "BAM captures value from price swings",
    "Early exit = forfeited yield"
  ]    
}
```

**To add new phrases:**
1. Open `bunny-config.json`
2. Add your phrase to the `"phrases"` array
3. Save the file
4. Refresh the page

**Tips for good phrases:**
- Keep them short (under 50 characters works best)
- Make them educational about Blackhaven
- Add emojis for personality 🎯
- Use simple, clear language

### Bunny Behavior Settings

The bunny behavior is controlled in `bunny.js`. Key timing parameters:

| Setting | Default | Description |
|---------|---------|-------------|
| Sleep cycle | 15-30s | Time before bunny falls asleep |
| Wake duration | 20-40s | How long bunny stays awake |
| Phrase display | 6s | How long speech bubble shows |
| Blink interval | 2-6s | Random blinking frequency |
| Dream bubble | 50% chance | Appears every 4s while sleeping |

## 📝 Content Guidelines

### Callout Components

Use Mintlify's built-in callouts for emphasis:

```mdx
<Tip>Helpful tips and best practices</Tip>
<Note>Important information</Note>
<Warning>Cautions and alerts</Warning>
<Info>General information</Info>
```

### Styled Containers

Use the `formula-box` class for framed content:

```mdx
<div className="formula-box">

**Your content here**

- Bullet points
- More content

</div>
```

### Math Formulas

LaTeX math is supported and styled in brand green:

```mdx
$$
D_{\text{final}} = D_{\text{base}} + \text{Bonus}
$$
```

## 🔧 Development

### File Naming

- Use lowercase with hyphens: `fixed-term-bonds.mdx`
- Place files in appropriate folders
- Update `mint.json` when adding new pages

### Frontmatter

Each page requires frontmatter:

```yaml
---
title: "Page Title"
icon: "icon-name"
---
```

Browse available icons at [Font Awesome](https://fontawesome.com/icons).

## 📦 Deployment

The documentation is deployed via Mintlify's hosting. Push changes to `main` branch to trigger automatic deployment.

```bash
git add .
git commit -m "Update documentation"
git push origin main
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📄 License

This documentation is proprietary to Blackhaven.

---

**Built with 💚 for the MegaETH ecosystem**
