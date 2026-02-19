# Melvin-Web_CSS

## Dag 1: 18 - 2 - 2026 Introductie
Ik moest gaan werken aan het Make-up gedeelte van CSS. Hier vallen onder andere shapes onder. Ik wilde hier dus mee gaan oefenen om vormen mee te maken. Dit kan ik namelijk later ook gebruiken voor mijn eigen website die ik gedurende de minor bij ga houden. Op die andere website wilde ik namelijk veel verschillende controllers doen, in tegenstelling tot de enkele controlle die ik had voor mijn persoonlijke website in de kick-off weken. Sommige van deze controllers hebben niet alleen de standaard vierkant en ronde vormen. Daarom wilde ik daar mee gaan oefenen tijdens deze opdracht. Ik had voor mezelf voorgenomen dat ik ik ging proberen om een gamecube controller te maken. Ik denk niet dat het er super goed uit gaat komen te zien, of uberhaupt af komt. Maar dan heb ik er wel mee geoefend.<br><br>

Ik was eerst gewoon een beetje documentatie aan het lezen en dingen aan het proberen. Maar kwam er niet echt uit, daarna ben ik eerst de dingen gaan namaken uit de voorbeeldwebsites die op DLO stonden. Door hier een beetje mee te spelen kreeg ik een beetje idee van hoe het werkte en kon ik er zelf mee gaan spelen. Ik was eerst begonnen met de controller. Ik probeerde hem eerst op te delen in stukken, beginnend met het midden gedeelte want die leek me het makkelijkst. Dit lukte redelijk, ik heb veel inspiratie van de vlag code gebruikt om deze te maken.

<img src="Assets/README_imgs/controller-shape-first.png>

Daarna ging ik eerst bezig met sommige andere onderdelen en knoppen om meer te spelen met de verschillende vormen. Zo had ik een octagon gemaakt voor een joystick en heb ik een plusje gemaakt voor de dpad. Deze gingen vrij snel af. Daarna ging ik werken aan de X en Y knoppen. Deze hebben een beetje de vorm van een boon. Het was even gedoe voordat deze goed werkte maar uiteindelijk zien ze er nu wel redelijk uit.

<img src="Assets/README_imgs/bean-shape-paint.png">

Omdat ik nu wat meer ervaring heb met clip-path: path en clip-path: shape, wilde ik proberen om misschien de controller in 1x te maken, in plaats van losse onderdelen. Ik besloot hier met clip-path: shape te werken zodat ik hem later eventueel nog groter of kleiner makkelijker kon maken. Ik had hem eerst even in Figma geschets zodat ik makkelijker de percentages af kon lezen. Daarna heb ik hem in code gezet en hier en daar nog een beetje de waardes veranderd zodat hij er beter uit ziet. Ik ben tevreeden met het resultaat.

```
#controller-shape {
    background: var(--controller-color);
    width: 520px;
    height: 300px;
    /* clip-path: path("M0 60 Q250 0 500 60 L500 240 Q250 200 0 240 Z"); */
    clip-path: shape(
            /* Startpunt */
            from 5% 25%,

            /* Start to top midden */
            curve to 50% 0% with 15% 0,

            /* Top midden naar rechtsboven */
            curve to 95% 25% with 85% 0,

            /* Rechtsboven naar rechtsonder */
            curve to 98% 95% with 100% 60%,

            /* Rechtsonder naar rechter handheld */
            curve to 85% 95% with 91.5% 100%,

            /* Rechter handheld naar midden center */
            curve to 50% 45% with 75% 40%,

            /* Midden center naar linker handheld */
            curve to 15% 95% with 25% 40%,

            /* linker handheld naar linksonder */
            curve to 2% 95% with 8.5% 100%,

            /* Linksonder naar Start */
            curve to 5% 25% with 0% 60%,

            close
        )
}

```

<img src="Assets/README_imgs/Controller-shape-Figma.png">
<img src="Assets/README_imgs/shapes">

### Interessante websites
https://bennettfeely.com/clippy/
https://css-tricks.com/css-blob-recipes/
https://css-shape.com/
https://css-generators.com/blob/
https://developer.chrome.com/blog/css-shape?hl=nl
https://frontendmasters.com/blog/understanding-css-corner-shape-and-the-power-of-the-superellipse/

### Inspiratie / hulp
https://cdn.prod.website-files.com/5b44edefca321a1e2d0c2aa6/5e5f3b54311da41f4689a476_Dimensions-Guide-Digital-Video-Game-Controllers-GameCube-Controller-Dimensions.svg
https://upload.wikimedia.org/wikipedia/commons/a/a5/GameCube_controller.png

### Checkout met Groepje + Sanne
Tijdens de checkout hebben we even kort uitgelegd waar we aan hebben gewerkt en hoe de presentatie van morgen eruit komt te zien. Hierin waren we nog even wat dieper in gegaan op hsl en rgba. Hier had Sanne nog even een duidelijk voorbeeld van gegeven van wat het verschil is als je bijvoorbeeld een gradient gebruikt. Dit was goed om te zien. Morgen kunnen we nog even testen hoeveel we te vertellen hebben zodat we niet te kort of te lang aan het praten zijn. Zelf heb ik vandaag in ieder geval veel geleerd over clip-path: path en clip-path: shape. Samen met verschillende corner-shapes.

## Dag 2: 19 - 2 - 2026
