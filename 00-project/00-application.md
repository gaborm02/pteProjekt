---
name: Mándity Gábor
neptun: F0I4OY
id: 2026-LG-03
---
# Alacsony költségű headless CMS és statikus weboldalgenerátor

## A brief értelmezése

A projekt célja egy olyan alacsony költségű verziókezelt headless CMS és statikus weboldalgenerátor kifejlesztése, amely felesleges szerverterhelés és drága infrastruktúra nélkül teszi lehetővé weboldalak, strukturált adatok és fájlok kezelését. A rendszer egy statikusan kiszolgálható adminisztrációs felületből, egy minimális erőforrásigényű backendből, egy jól definiált headless API-ból, valamint egy statikus oldalgenerátorból áll. A megoldásnak integrálnia kell külső blogszolgáltatók tartalmát is build időben, miközben a publikus oldal teljesen statikus kimenetként, alkalmazásszerver nélkül futtatható.

## Miért én lennék alkalmas erre a projektre?

Mérnökinformatikus hallgatóként kifejezetten érdekelnek a modern webes architektúrák és a rendszertervezési kihívások. A feladat által megkövetelt struktúra — a backend, a Headless API és a statikus generálás éles elválasztása — jó lehetőséget nyújt számomra arra, hogy a szoftverfejlesztési és adatbázis-kezelési alaptudásomat egy gyakorlati, valós problémát megoldó projektben alkalmazzam. Célom egy jól strukturált, tisztán dokumentált és fenntartható rendszer megvalósítása.

## Releváns tapasztalat és előzmények

Tanulmányaim során stabil alapokat szereztem objektumorientált programozásból, szoftverarchitektúrákból és adatbázis-kezelésből (C, C#, Java, SQL), valamint a webfejlesztés alapjaiból (HTML, CSS, JavaScript). Bár a projektben előírt TypeScript, SvelteKit és Vue keretrendszereket, illetve a PocketBase/Firebase jellegű backendeket most fogom mélyebben elsajátítani, a meglévő JavaScript és C#/Java ismereteimre építve magabiztosan tudok átállni a típusos webes fejlesztésre. A relációs adatbázisok és a JavaScript alaptudásom megkönnyíti az API-k, az adatmodellek és a backend-logika átlátását, a Gittel szerzett tapasztalataim pedig segítenek a verziókezelésben és a GitHub Actions workflow-k felépítésében.

## Tervezett megközelítés

A fejlesztést a legkisebb költségű backend és adattárolási architektúra kiválasztásával és összehasonlításával kezdem. Ezt követően megtervezem a tartalommodellt (oldalak, blokkok, fájlok) és a headless API-t. Elkészítem a statikusan kiszolgálható adminisztrációs felületet a tartalom szerkesztéséhez és a jogosultságkezeléshez. A publikációs folyamatot úgy alakítom ki, hogy a tartalom módosításakor egy automatizált CI/CD munkafolyamat (GitHub Actions) hívja meg a statikus weboldalgenerátort, amely lekéri a CMS adatait és a külső blog feedjét, majd legenerálja a tiszta HTML/CSS/JS kimenetet a statikus hosting felületre.

## Kezdeti terv

1. Az adattárolási, hitelesítési és hosting lehetőségek összehasonlítása és architektúrális döntések dokumentálása.
2. A tartalommodell, a szigorú TypeScript típusok és a headless API határainak megtervezése.
3. A statikusan generált adminisztrációs felület és a jogosultságkezelés alapjainak elindítása.
4. A publikus oldalsablon és a statikus weboldal generátor logikájának megvalósítása.
5. A külső blogbejegyzések integrálása a build folyamatba.
6. A GitHub Actions alapú automatikus publikációs és statikus telepítési (GitHub Pages) folyamat beállítása és tesztelése.

## További információ

A teljes fejlesztési folyamatot Git repóban vezetem, TypeScript használatával, figyelve arra, hogy érzékeny adatok (API kulcsok, tokenek) ne kerüljenek a verziókezelőbe. A feladatokat átlátható módon, issue-kra bontva követem. A frontendhez Vue vagy SvelteKit keretrendszert, az automatizált kiadáshoz GitHub Actionst használok.
