# Händler erzeugen

## NPC-Händler (Citizen-Plugin)

1. gewünschte Skin suchen (z.B. [hier](https://de.namemc.com/minecraft-skins)), Namen des Spielers merken
1. an die gewünschte Stelle gehen (Umplazieren ist möglich)
1. `/npc create GewünschterName` (falls es ein bestehender NPC ist: diesen ansehen und `/npc select`)
1. `/npc skin GemerkterSpielername` (auf Survival geht auch `/npc skin -u <URL zur Skin>`)
   
   Dies ist nicht nötig, falls _GewünschterName_ und _GemerkterSpielername_ identisch sind.
1. `/trait shopkeeper`
1. alle Materialien, die der Händler verkaufen oder als Bezahlung annehmen soll 
   _in ausreichender Menge!_ ins Inventar nehmen (im Kreativmodus reicht eines, 
   da per mittlerer Maustaste vervielfältigbar).
1. den Händler mit Ducken+Rechtsklick anklicken, das öffnet das Shop-Konfigurieren-UI.
1. im erscheinenden Menü können jetzt die möglichen Transfers eingegeben werden.
   Es sind bis zu neun Transfers pro Seite möglich (einer pro Spalte),
   dann muss man mit den Seiten-Icons navigieren, um weitere anzulegen.
   * in der _ersten_ Zeile steht, was der Händler _verkauft_.
   * in der _dritten_ Zeile steht, was er dafür will. Im Shop-UI muss dies in den Linken Bezahl-Slot. 
   * in der _zweiten_ Zeile kann man noch einen weiteren Stack einfügen, dann verlangt der Händler dies zusätzlich. 
     Dies muss dann in den rechten Bezahlslot.
   
   Die erste und dritte Zeile müssen gefüllt sein, die zweite ist optional. 
1. mit den weiteren Optionen des Menüs kann man den Händler löschen oder umbenennen, wobei letzeres für den Titel im
   Shop-UI wichtig ist, aber gleichzeitig auch den NPC umbenennt. Man muss diesen ggf. danach mit `/npc rename GewünschterName`
   wieder zurückbenennen.
1. mit `/npc tphere` kann der Händler umpositioniert werden (an den Ort, an dem man sich gerade befindet).

## Mob-Händler

1. an die gewünschte Stelle gehen
1. `/shopkeeper MobTyp` oder `/shopkeeper Admin-shop MobTyp` zum erzeugen _auf dem Block, den man anschaut_. 
   _MobTyp_ muss dabei der interne Name des gewünschten Mobs sein. Lässt man _MobTyp_ weg wird ein Villager erzeugt. 
   Die In-Game-Konsole bietet Autocomplete für die Mobtypen. 
1. Ab jetzt ist alles wie beim NPC-Händler (ab Schritt 6). 
1. Das Shop-Konfigurieren-UI bietet je nach Mobtyp ggf. noch Buttons um das Aussehen zu verändern (z.B. Baby-Form bei denen,
   die eine solche haben,  geladene Creeper, oder die diversen Villager-Varianten).
1. ein Umpositionieren ist soweit ich das sehe nicht möglich (außer vielleicht mit MC-Standardbefehlen?). 

## Links
* [Citizens2-Befehle](https://wiki.citizensnpcs.co/Commands)
  Man kann sie z.B. rumwandern lassen.
* [Shopkeepers-Befehle](https://github.com/Shopkeepers/Shopkeepers-Wiki/wiki/Commands)
  Man kann z.B. spezielle Permissions erforderlich machen. 
