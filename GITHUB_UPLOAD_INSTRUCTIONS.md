# Upload to GitHub

```bash
git init
git add .
git commit -m "Publish reverse engineer history and reconstructed runtime tester V7"
git branch -M main
git remote add origin https://github.com/naruepan2/SAP-Reverse-Engineer-Agent-and-Skill-for-VS-Code.git
git push -u origin main
```

If `origin` already exists:

```bash
git remote set-url origin https://github.com/naruepan2/SAP-Reverse-Engineer-Agent-and-Skill-for-VS-Code.git
git add .
git commit -m "Add complete history and runtime tester V7 reconstruction"
git push -u origin main
```
