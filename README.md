# Ročníkový projekt – 3D hra ve stylu Only Up

## Ročníkový projekt

### Název projektu
**3D parkourová hra ve stylu Only Up (Third-Person Game)**

---

## 1. Cíl ročníkového projektu
Cílem tohoto ročníkového projektu je vytvořit **3D hru inspirovanou principem hry Only Up**, která bude realizována z pohledu třetí osoby (third-person). Hráčovým úkolem je překonávat různé překážky, postupně se dostat až do cíle a hru úspěšně dokončit.

Projekt je zaměřen na:
- pochopení základních principů vývoje her,
- práci s pohybem postavy a animacemi,
- použití kolizí a triggerů,
- tvorbu jednoduchého uživatelského rozhraní (UI widgety),
- logiku vítězství a prohry ve hře.

Projekt souvisí s mým studovaným oborem a zároveň odpovídá mým osobním zájmům v oblasti her a jejich vývoje.

---

## 2. Popis projektu / Zadání
Vytvořit vlastní hru, ve které:
- hráč ovládá postavu z pohledu třetí osoby,
- cílem je dostat se přes překážky až do finálního bodu,
- pád znamená konec pokusu,
- po výhře nebo prohře se zobrazí herní menu s možnostmi další akce.

Projekt je zpracováván **individuálně**.

---

## 3. Současný stav projektu
Projekt je v rozpracované fázi a obsahuje následující funkční části:

### 3.1 Pohyb a ovládání postavy
- Implementovaný movement postavy (chůze, běh, skok).
- Kamera z pohledu třetí osoby (third-person).
- Základní animace postavy propojené s pohybem.

### 3.2 Herní prostředí a překážky
- Vytvořeno několik parkourových překážek.
- Přidány kolize k objektům, aby bylo možné po nich chodit nebo na ně skákat.
- Postupné testování obtížnosti a rozložení překážek.

### 3.3 Logika pádu (Game Over)
- Použit **Trigger Box**, který detekuje pád hráče.
- Po pádu se zobrazí **widget Game Over**, který obsahuje:
  - tlačítko **Restart** (znovu spuštění hry),
  - tlačítko **Quit** (ukončení hry).

### 3.4 Dokončení hry (You Won)
- Na konci mapy se nachází cílový objekt.
- Cílem je **rotující kámen**, který:
  - má vlastní animaci rotace,
  - slouží jako vizuální cíl hry.
- Po dosažení cíle se zobrazí **widget You Won**, který obsahuje:
  - tlačítko **Restart**,
  - tlačítko **Quit**.

---

## 4. Použité technologie a nástroje
- Herní engine: *Unreal Engine*
- Programování herní logiky (Blueprinty / skripty)
- GitHub – verzování projektu a dokumentace
- Markdown – tvorba projektové dokumentace

---

## 5. Moje práce na projektu
Na projektu jsem pracoval samostatně. Moje práce zahrnovala zejména:
- návrh herního principu inspirovaného hrou Only Up,
- tvorbu a rozmístění překážek,
- implementaci pohybu a animací postavy,
- práci s kolizemi a trigger boxy,
- vytvoření a napojení UI widgetů (Game Over, You Won),
- řešení logiky restartu a ukončení hry,
- základní optimalizaci a testování hratelnosti.

Během realizace jsem řešil například:
- správné nastavení kolizí,
- detekci pádu hráče,
- propojení herní logiky s uživatelským rozhraním,
- plynulost pohybu a animací.

---

## 6. Možná budoucí vylepšení
Do budoucna by bylo možné projekt rozšířit například o:
- více úrovní,
- checkpointy (uložení postupu),
- časomíru nebo bodovací systém,
- obtížnější překážky,
- lepší grafiku a efekty,
- dalsí zvuky a podkresovou hudbu.

---

## 7. Tým
Projekt je vypracován **individuálně**.

---

## 8. Zdroje a citace
(1) CITACE.COM, S.R.O. Citace.com. Online. © 2025. Dostupné z: [https://www.citace.com/](https://www.citace.com/). [cit. 2025-12-17].

(2) GITHUB, INC. GitHub. Online. © 2025. Dostupné z: [https://github.com/](https://github.com/). [cit. 2025-12-17].

(3) OPENAI, ChatGPT. Online. © 2025. Dostupné z: https://chatgpt.com/. [cit. 2025-12-17].

(4) Grok. Online. Grok.com. Dostupné z: https://grok.com/. [cit. 2025-12-19].

(5) Fab. Online. fab.com. Dostupné z: https://www.fab.com/. [cit. 2025-12-19].

(6) Video návod. Online. Dostupné z: https://www.youtube.com/watch?v=IPQldaLLx_Y&t=377s. [cit. 2025-12-19].

(7) Video tutorial. Online. Dostupné z: https://www.youtube.com/watch?v=e_SPuvO_l1w&t=127s. [cit. 2025-12-19].

(8) Video návod 2. Online. Dostupné z: https://www.youtube.com/watch?v=LrExuqVQDb4. [cit. 2025-12-19].

---

## 9. Literatura
[1] Markdown Guide. Online. © 2025. Dostupné z: [https://www.markdownguide.org/](https://www.markdownguide.org/). [cit. 2025-12-17].


---

## 10. Poděkování
Děkuji autorům online tutoriálů, dokumentací a komunitě, jejichž materiály mi pomohly při tvorbě tohoto projektu.
