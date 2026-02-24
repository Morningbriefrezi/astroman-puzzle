# GitHub-ზე ატვირთვის ზუსტი ინსტრუქცია (ASTROMAN თამაშები)

ეს ფაილები უკვე მზად არის:
- `index.html`
- `easy-level.html`
- `medium-level.html`
- `hard-level.html`

## 1) GitHub-ზე ახალი რეპოზიტორიის შექმნა
1. შედი GitHub-ში.
2. დააჭირე **New repository**.
3. მაგალითად დაარქვი: `astroman-space-games`.
4. აირჩიე **Public**.
5. **არ** მონიშნო “Add README / .gitignore / license” (რადგან უკვე გვაქვს ლოკალური git).
6. დააჭირე **Create repository**.

## 2) ლოკალური პროექტის მიბმა GitHub-ზე
ტერმინალში (პროექტის დირექტორიაში) გაუშვი:

```bash
cd /workspace/astroman-puzzle
git remote add origin https://github.com/<USERNAME>/<REPO>.git
git push -u origin work
```

თუ remote უკვე არსებობს, გამოიყენე:

```bash
git remote set-url origin https://github.com/<USERNAME>/<REPO>.git
git push -u origin work
```

## 3) პირდაპირი ლინკები ფაილებზე GitHub-ში
ატვირთვის შემდეგ ფაილების ლინკები იქნება:
- `https://github.com/<USERNAME>/<REPO>/blob/work/index.html`
- `https://github.com/<USERNAME>/<REPO>/blob/work/easy-level.html`
- `https://github.com/<USERNAME>/<REPO>/blob/work/medium-level.html`
- `https://github.com/<USERNAME>/<REPO>/blob/work/hard-level.html`

## 4) playable ლინკი (GitHub Pages)
რეპოზიტორიაში:
1. შედი **Settings → Pages**
2. Source: **Deploy from a branch**
3. Branch: **work** და Folder: **/(root)**
4. Save

2-5 წუთში მიიღებ:
- `https://<USERNAME>.github.io/<REPO>/`

და თამაშების პირდაპირი ლინკები:
- `https://<USERNAME>.github.io/<REPO>/easy-level.html`
- `https://<USERNAME>.github.io/<REPO>/medium-level.html`
- `https://<USERNAME>.github.io/<REPO>/hard-level.html`

## 5) სწრაფი შემოწმება ლოკალურად
```bash
cd /workspace/astroman-puzzle
python3 -m http.server 8000
```

გახსენი:
- `http://localhost:8000/`
- `http://localhost:8000/easy-level.html`
- `http://localhost:8000/medium-level.html`
- `http://localhost:8000/hard-level.html`
