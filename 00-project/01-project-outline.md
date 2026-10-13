---
name: Mándity Gábor
neptun: F0I4OY
id: 2026-LG-03
github: https://github.com/username/low-cost-headless-cms
github_project: https://github.com/users/username/projects/1
---
# Alacsony költségű headless CMS és statikus weboldalgenerátor

A kisebb szervezeteknek gyakran egyszerű weboldalra, blogintegrációra és adminisztrációs felületre van szükségük, egy hagyományos monolitikus CMS üzemeltetési költsége és összetettsége nélkül. A projekt célja egy alacsony költségű headless tartalomkezelő rendszer, amely oldalak, strukturált adatok és fájlok tárolását végzi, majd egyedi sablonokból statikus publikus weboldalt generál. A rendszer magában foglal egy alacsony erőforrás-igényű backendet, egy statikusan kiszolgálható adminisztrációs felületet, valamint egy GitHub Actions alapú automatizált statikus buildelési folyamatot, amely külső blogok (pl. Substack) tartalmát is beépíti.

## Célok

- **Elsődleges cél:** Működő, verziókezelt, alacsony költségű headless CMS és statikus weboldalgenerátor kifejlesztése.
- **Célfelhasználók / érintettek:** Kisebb szervezetek, szerkesztők és webfejlesztők, akik minimális fenntartási költséggel szeretnének statikus weboldalakat kezelni.
- **Mérhető sikerkritériumok:** Az adminisztrátor bejelentkezhet, létrehozhat és szerkeszthet oldalakat, feltölthet fájlokat; a rendszer sikeresen generál egy statikus publikus weboldalat a külső blogbejegyzésekkel együtt; a kimenet kiszolgálható alkalmazásszerver nélkül.
- **Korlátok:** TypeScript használata a teljes alkalmazásban; Vue vagy SvelteKit az egyedi sablonokhoz és a publikus oldalhoz; alacsony költségű vagy saját üzemeltetésű backend (pl. PocketBase); titkos kulcsok és emelt jogosultságú adatok nem kerülhetnek a klienskódba vagy a repóba.

## Hatókör

### Benne van a hatókörben

- Felhasználói regisztráció, hitelesítés és jogosultságkezelés az adminisztrációs felülethez.
- Site-ok, oldalak, strukturált tartalmi rekordok és feltöltött fájlok kezelése.
- Headless tartalom-API a tartalomkezelés és megjelenítés szétválasztására.
- Legalább egy Vue-val vagy SvelteKittel megvalósított egyedi publikus weboldalsablon.
- Külső blog (pl. Substack vagy Medium) RSS/Atom feedjének integrálása build időben.
- Statikus oldalgenerálás és GitHub Actions alapú automatikus publikálás.

### Nincs benne a hatókörben

- Valós idejű többjátékos vagy kollaboratív szerkesztés.
- A külső blogbejegyzések szerkesztése vagy tárolása a CMS-en belül.
- Folyamatosan futó alkalmazásszerver a publikus oldal kiszolgálásához.

## Jegyzetek

A fejlesztés során kiemelt figyelmet kell fordítani a backend és a frontend szigorú elválasztására, valamint arra, hogy a build folyamat során az érzékeny adatok (API kulcsok) ne szivárogjanak ki a generált statikus kimenetbe.