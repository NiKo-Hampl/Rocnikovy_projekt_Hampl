# 🧍 Blueprinty hráče (Player)

Tato část dokumentace popisuje blueprinty,
které se starají o **pohyb, animace a kameru hráče**.

---

## 🎮 Player Movement Blueprint

![Player Movement](movement.png)

### Popis funkce
Tento blueprint zajišťuje:
- pohyb hráče dopředu, dozadu a do stran,
- skákání postavy,
- základní ovládání pomocí klávesnice.

### Jak funguje
- Vstupy z klávesnice jsou zpracovány pomocí Input Actions.
- Pohyb je řešen pomocí Character Movement komponenty.
- Skok je aktivován při stisknutí příslušné klávesy.

---

## 🎞 Animace postavy

![Player Animation](animation.png)

### Popis funkce
Blueprint propojuje:
- rychlost pohybu hráče
- stav skoku
- animace postavy

### Jak funguje
- Rychlost postavy se přenáší do Animation Blueprintu.
- Podle hodnot se přepínají animace chůze, běhu a skoku.
