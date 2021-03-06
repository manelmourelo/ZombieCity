## About the game

[ZombieCity](https://bitbucket.org/manel_mourelo/ia-game/wiki/Home) is a project consistent of creating a AI based Game made with [Unity3D](https://unity3d.com/es).

You play the roll of a zombie commander and you must build different buildings to organize your troops and end with the military forces that are the last defensive forces of the humans.

This game has been done in the [Artificial Intelligence](https://www.upc.edu/estudispdf/guia_docent.php?codi=804245&lang=ing) subject in the 3rd year of the [Game Design and Development](https://www.citm.upc.edu/ing/estudis/graus-videojocs/) grade of [CITM](https://www.citm.upc.edu/ing/) ([UPC](https://www.upc.edu/en?set_language=en)).

## Team Members

### Sergio Gómez Roldán: 
* Artist, programmer and designer
* [GitHub](https://github.com/Sersius) 
* [BitBucket](https://bitbucket.org/Sersius3/)

### Manel Mourelo Montero: 
* Manager, programmer and designer
* [GitHub](https://github.com/manelmourelo) 
* [BitBucket](https://bitbucket.org/manel_mourelo/)

## Evolution

We started the game programming simple Steering Behaviours that combined allowed us to have all the entities moving through the map. Once we had all the entities moving, we passed its behaviours to Behaviour Trees (using [NodeCanvas](http://nodecanvas.paradoxnotion.com/)), so we could manage them in an easier way. Once it was all implemented, we began to add sounds particles and menus to the game, so it could be easier to understand what was happening.

### Normal Zombie and Ranged Zombie BT
!["Ranged+NormalBT"](BT/Ranged%2BNormal.PNG)

With this tree this zombies will search a random barricade, when their approach to another barricade they will attack it, and then all the soldiers around an area.

### Suicide Zombie BT
!["SuicideBT"](BT/Suicide.PNG)

This zombie will go to the closest barricade he can found and explode making AOE damage.

### Tank Zombie BT
!["TankBT"](BT/Tank.PNG)

The tank will do the same as the normal and ranged but only with barricades, so they will never attack a soldier.

### Soldier BT
!["Soldier"](BT/Soldier.PNG)

The soldier will go to their position to guard and in the night they will shoot all the zombies that come.

### Builder BT
!["BuilderBT"](BT/Builder.PNG)

The builder function is to go to the barricades that are not destroyed and repair them.

## Links
* [Repository](https://bitbucket.org/manel_mourelo/ia-game/src/master/)
* [Game Wiki](https://bitbucket.org/manel_mourelo/ia-game/wiki/Home)
* [Download latest version](https://github.com/manelmourelo/ZombieCity/releases)

## Gameplay

Here you can see a short video gameplay of the game.
<iframe width="560" height="315" src="https://www.youtube.com/embed/MAiDKeBfwgA" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Controls

### CAMERA CONTROLS

* Move mouse: Camera will move
* Mouse wheel: Move Camera forward and backward

### CONTROLS

* To build just use the build button and chose what you want to build with the menu. Once it’s selected click the buildable areas to build.

* To upgrade a building just click on the building and use the menu.

* If you use the right button of the mouse you’ll drop a brain that if is eaten by a zombie it will heal him and double his attack damage.

## License

### ZombieCity is under the MIT License

#### Copyright (c) 2018 Sergio Gómez Roldán and Manel Mourelo Montero

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
