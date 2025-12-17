# 📦 Trigger Boxy – Herní logika

Tato část dokumentace popisuje **Trigger Boxy**, které jsou použity
pro detekci pádu hráče a dokončení hry.

---

## ❌ Trigger Box – Game Over (pád hráče)

![Trigger Box ve hře](../IMG/TriggerBoxy/TriggerBox.png)

### Popis
Tento Trigger Box je umístěn pod herní mapou a slouží k detekci pádu hráče.

Pokud hráč spadne mimo herní plochu:
- hra se zastaví,
- zobrazí se **Game Over widget**.

---

## 🧠 Blueprint Trigger Boxu – Game Over

![Blueprint Trigger Boxu](../IMG/TriggerBoxy/blueprint_triggerBoxu.png)

### Jak blueprint funguje
- Trigger Box detekuje vstup hráče pomocí `OnActorBeginOverlap`.
- Po aktivaci:
  - hra se pozastaví,
  - zobrazí se UI widget **Game Over**,
  - hráč má možnost restartovat hru nebo ji ukončit.

---

## ✅ Trigger Box – Dokončení hry (You Won)

![Trigger Box You Won](../IMG/TriggerBoxy/TriggerBox2.png)

### Popis
Tento Trigger Box se nachází u cílového objektu.
Po vstupu hráče:
- hra je úspěšně dokončena,
- zobrazí se **You Won widget**.

---

## 📌 Shrnutí
Trigger Boxy zajišťují:
- detekci pádu hráče,
- správné ukončení hry,
- zobrazení odpovídajících UI widgetů.

