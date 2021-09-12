# basics

## Ereignisverarbeitung
```
 while(true)
 {
	read_input_devices();
	animate_scene();
	draw_scene();
	sleep_until_next_event(); / no change in animated scene if nothing happens either in the scene or because of the user input
 }
 ```
 
## Bildpuffer
In Bildpuffern wird pro Fragment/Pixel die eine Eigenschaft gespeichert, abhängig vom Puffer.
 * Tiefenpuffer enthält z Koordinate des Punkts vor der Projektion auf die Bildebene und dient der Extraktion des vordersten Fragments (projezierten Punkts auf der Bildebene), also Entscheidung welches Pixel soll an der entsprechenden Stelle auf dem Bildschirm angezeigt werden, falls es mehrere Pixel mit gleichem x- und y-Wert gibt.
 * Farbpuffer, enhält Farben für jeden Pixel, RGBA-Farpuffer enthält zusätzlich die Deckkraft der Farbe
 * stencil buffer - verschieden einsetzbar (z.B. für Projektion von 3D Elementen auf Spiegeloberfläche oder für CSG Operationen)
 * accum(ulation) buffer - für Bildüberlagerung bei z.B. motion blur order Antialiasing

## Datenfluss in Graphiksystemen
1. CPU
	* zerlegt Szene in Objekte
	* zerlegt Objekte in ebene Dreiecke, mit Eckpunkten und produziert so vertex data (Vektordaten)
	* sende Dreiecke implizit (implizit: ohne weitere Information auf etwas logisch schließbar) in Knotenreihenfolge (Knotenbenennungslogik notwendig?)
2. GPU
	* transformiere Knotenpositionen (durch Matrizenmultiplikation)
	* transformiere 3D-Knotenpositionen in Bildkoordinaten (perspektivische Projektion mit Matrizen/Matrizenmultiplikation)
	* zerlege Polygone in der Bildebene in Fragmente (Fragmente=Pixel?), also Rasterisierung

## OpenGL (1.x) fixed function pipeline
## OpenGL 2.0 pipeline (used in WebGL)
* Programming language is variant of C and C++
	* excluding: pointers, references, implicit type casts, #include
	* including: function calls by value, extensions for matrices, C++ constructors, access to large parts of OpenGl state (i.e. lights,materials, transforms)
## basics Graphik-APIs
* Graphik-APIs ermöglichen direkte Programmierung der GPU.
* Vorgehensweise:
	* **Konfiguration** der GPU (Hintergrundfarbe, also neutral value for "framebuffer memory"; verwendete Bildpuffer)
	* **Definition Ansicht** (Blickpunkt, Kameraparameter)
	* **Defintion Material** (Oberflächenfarbe, Texturen, Shader für "pro Pixel Auswertung" eines Beleuchtungsmodells)
	* **Definition der Geometriebeschreibung in der Szene** (Angabe der Art der Primitive (Punkt, Linie, Dreieck) im Raum; Spezifikation der Oberflächennormale ,Farbe ,Texturposition und Raumposition pro Knoten der Primitive)
	
>Danach projeziert GPU Punkte, Linien und Dreiecke im 3D auf die Bildebene, erstellt Pixel und trägt Farbe, Textur des 3D Elements in Pixel der rasterisierten Projektion.
### Konfiguration
* **zustandsbasierte Programmierung** GPU in OpenGL über Kontext angesteuert
Kontext verwaltet GPU Konfiguration, in der u.a. Shader, aktuelle Liniendicke, aktuelle Lininefarbe gespeichert sind
* verschiedene **Kontexte/Zustände existieren parallel**, aber nur einer kann akitv, also an ihm kann gearbeitet und von ihm kann gezeichnet werden (Kontext wird mit Fenster erzeugt (wobei OpenGL Version wählbar ist)), also muss zwischen Kontexten/Zustaänden gewechselt werden -> "MakeCurrent"; sammle OpenGL Funktionsaufrufe in einer function, vor deren oder zu Neginn deren Ausführung er Kontext garantiert zum gewünschten gewechselt wird und am Ende dieser der vorherige Zustand wiederhergestellt wird.

## Geometrie
* nur Dreiecke und Vierecke als Zeichenprimitve unterstützt, weshalb glatte Flächen durch ebene Polygone, auch Facetten genannt, approximiert werden
* um Fläche glatt wirken zu lassen Beleuchtung pro Knoten (also Facettenecke) genutzt
	* Flat Shading
	* Gouraud Shading - Normalen der anliegenden Facetten an Knoten gemittelt -> Beleuchtungsrechnung an Knoten durchgeführt -> Farbe interpoliert
	*

### Annotations
> freeglut zur Fenstererzeugung und Gerätedatenauslesung genutz um OpenGL nutzbar zu machen

