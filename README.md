# Qambariddin avlodlari — oila shajarasi

Oddiy statik sayt: bitta `index.html` fayl, server va baza kerak emas.

## Maʼlumotlarni oʻzgartirish

`index.html` ichida `window.SHAJARA = {` qatorini toping. Har bir odam bitta qator:

```js
{ id: "nargiza", ism: "Nargiza", jins: "a", ota_ona: "madxiddin", maxsus: true },
```

- `id` — lotin harflarida noyob nom (boʻshliqsiz)
- `ism`, `familiya` — ismi va familiyasi
- `jins` — `"e"` (erkak) yoki `"a"` (ayol)
- `ota_ona` — shajaradagi otasi yoki onasining `id` si (eng birinchi ajdodda `null`)
- `tugilgan`, `vafot` — yil (`1956`) yoki sana (`"1956-03-14"`); vafot yili nomaʼlum boʻlsa `"?"`
- `turmush`, `joy`, `kasb`, `izoh`, `rasm` — ixtiyoriy
- `maxsus: true` — shu odam va uning nasabi oltin rangda ajratib koʻrsatiladi

Oʻzgarishni `main` ga yuborganingizdan keyin GitHub Pages saytni 1–2 daqiqada yangilaydi.

## Kompyuterda koʻrish

```bash
python3 -m http.server 8765
```

Soʻng brauzerda http://localhost:8765 ni oching.
