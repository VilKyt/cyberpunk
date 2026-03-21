# HOW TO PUT THIS ON GITHUB

Quick steps to get this folder into a private GitHub repo called `cyberpunk`.

---

## Option A — GitHub Website (easiest)

1. Go to https://github.com/new
2. Repository name: `cyberpunk`
3. Set to **Private**
4. Do NOT initialise with a README (you already have one)
5. Click **Create repository**
6. On the next screen, click **uploading an existing file**
7. Drag the entire `cyberpunk` folder contents in
8. Commit

Done. Files will be browsable on GitHub with the markdown rendered nicely.

---

## Option B — Git CLI (if you have git installed)

```bash
cd path/to/cyberpunk
git init
git add .
git commit -m "initial campaign files"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/cyberpunk.git
git push -u origin main
```

Replace `YOUR_USERNAME` with your GitHub username.

---

## Adding New Files Later

When we finish a new scene or NPC in chat, I'll give you the file content and tell you where it lives in the folder structure. You can either:
- Paste it in via the GitHub web editor (click **Add file → Create new file**)
- Or drop it into your local folder and `git push`

---

## Folder Structure Reference

```
cyberpunk/
├── README.md                        # Campaign overview
├── act-1/
│   ├── README.md                    # Act 1 overview + thread tracker
│   └── scene-1-the-tomb.md          # ✅ Complete
│   └── scene-2-rooks-camp.md        # 🔲 In progress
│   └── scene-3-night-city-fringe.md # 🔲 Planned
├── act-2/                           # 🔲 Planned
├── act-3/                           # 🔲 Planned
├── npcs/
│   ├── rook.md                      # ✅ Complete
│   ├── the-director.md              # ✅ Complete
│   └── [key-npc-name].md            # 🔲 Pending (name TBD)
├── world/
│   └── factions-and-lore.md         # ✅ Complete
└── assets/
    └── cyberpunk-wildemount.html    # ✅ The neon map
```
