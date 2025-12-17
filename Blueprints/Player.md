# Blueprint: Držení a animace objektů (Held Object Animations)

Tento Blueprint v **ALS_CharacterBP** řídí dynamické přepínání animací držaných objektů (zbraně, pochodně, bedny atd.) pomocí overlay stavů v animátoru.
---

## 🎮 Player Movement Blueprint

![Player Movement](IMG/Pohyb/prvni_pohyb.png)
![Player Movement](IMG/Pohyb/druhy_pohyb.png)
![Player Movement](IMG/Pohyb/treti_pohyb.png)

### Popis funkce
Zajišťuje:
- Přepínání overlay animací podle typu držaného objektu (rifle, pistole, pochodně, binokulár, bedna...).
- Aktualizaci spine rotace a připojení meshů k rukám.
- Kompatibilitu s mužskými/ženskými/injured postoji.

### Jak funguje
- **Event Update Held Object** spouští **On Update Held Object Animations** (implementable event).
- **Switch on EALOverlayState** vybere stav podle aktuálního objektu (Masculine/Feminine/Injured, Rifle, Pistol 1/2 Handed, Torch, Binoculars, Box, Barrel).
- **Get Anim Instance → Cast to ALS_AnimBP** → **Get Anim Curve Value "Enable_SpineRotation"** → **Set** na Skeletal Mesh (umožňuje rotaci páteře).
- Další uzly řídí **Attach to Hand**, **Target Arm Mesh**, **Blend Poses** pro plynulý přechod.
---

## 🎞 Animace postavy

![Player Animation](IMG/animace/anim1.png)
![Player Animation](IMG/animace/anim2.png)
![Player Animation](IMG/animace/anim3.png)
![Player Animation](IMG/animace/anim4.png)
![Player Animation](IMG/animace/anim5.png)
![Player Animation](IMG/animace/anim6.png)
![Player Animation](IMG/animace/anim7.png)
![Player Animation](IMG/animace/anim8.png)
### Popis funkce
Blueprint propojuje:
- rychlost pohybu hráče
- stav skoku
- animace postavy

### Jak funguje
- Rychlost postavy se přenáší do Animation Blueprintu.
- Podle hodnot se přepínají animace chůze, běhu a skoku.

---

## 🎥 Third Person Camera

![Third person Camera](IMG/Kamera/Kamera_aim.png)
![Third person Camera](IMG/Kamera/Kamera_popis.png)

### Popis funkce
Tento blueprint zajišťuje:
- sledování hráče z pohledu třetí osoby,
- plynulé otáčení kolem postavy podle vstupu myši nebo gamepadu,
- možnost přibližování a oddalování kamery.

### Jak funguje
- Kamera je připojena k **Spring Arm komponentě**, která udržuje určitou vzdálenost od hráče.
- Rotace kamery se ovládá podle vstupů z **Input Axis** (myš / analogový joystick).
- Spring Arm zabraňuje průniku kamery do objektů pomocí **collision testu**.
- Při pohybu hráče se kamera hladce interpoluje, aby sledování bylo plynulé a nepůsobilo trhaně.

