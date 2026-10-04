# Grafiikat Pelimoottorissa

## Johdatus

Taitava graafikko voi luoda visuaalisesti puhuttelevia kuvia, malleja ja animaatioita, mutta mitä täytyy huomioida sisällyttäessä niitä peliin? Entä mitä osia peligrafiikasta voidaan toteuttaa pelimoottorin ja koodin puolella?

[comment]: <> (tälle osiolle vois keksiä hyvän otsikon)

## Osat

### Peligrafiikkojen luonnissa huomioitavaa

**Perinteisen ja pelitaiteen ero**

- Pelitaidetta luodessa joutuu ottamaan paljon teknisiä seikkoja huomioon, oli kyseessä 2D- tai 3D-taide
- Taideteosta harvoin tehdään yhdelle "kankaalle", jokainen osa täytyy erotella ja mahdollisesti tallentaa eri kerrokset erikseen, riippuen käyttötarkoituksesta
- Yksittäisenkin esineen tai hahmon osia saattaa joutua luomaan ja tallentamaan erikseen

**Tiedoston ominaisuudet**
- Valmis kuvatiedosto tulee tallentaa käytettävässä muodossa, esim. PNG
- 2D-animaatioista tehdään usein spritesheet/kuvatiedosto, ei videotiedostoa
    - Poikkeuksena peliin tarkoituksella sisällytetyt videot, esim. "cutscenet" eli välianimaatiot, jotka voi myös renderöidä pelin sisällä valmiin videon sijaan
- Resoluutio valitaan käytön mukaan:
    - Pikselitaidetta tehdessä täytyy olla tarkkana pikseleiden sekä lopullisen grafiikan koon suhteen
    - Pelissä pienet tai kaukaiset asiat usein ovat yksinkertaisempia, kuin muu grafiikka, sillä niiden  
    - Asioita skaalatessa resoluution muutos voi olla helposti huomattavissa, etenkin pienillä resoluutioilla


### Pelimoottorin & koodin puoli
**Pelimoottorin hyödyntäminen**
- Peligraafikon ei tarvitse, eikä voi, tehdä kaikkea (kuten dynaamisia muutoksia). Tiettyjä asioita voidaan tehdä pelin sisäisesti:
    - Modulaariset animaatiot ja liike
    - Animaatioiden ajoitusten muokkaaminen
    - Sävyn/läpinäkyvyyden muutokset
    - Koon muutokset
    - Rotaatio
    - Partikkelit, valaistus ja muut lisäefektit
    - Ja niin edelleen...

## Yhteenveto

Peligraafikon tulee siis osata tietenkin luoda taidetta, mutta myös sellaisessa muodossa, että sitä voidaan käyttää pelissä. Tämän vuoksi jokaisen peligraafikon on hyvä omata perustason ymmärrys pelien teknisestä puolesta itse taiteen luomisen lisäksi. Hänen täytyy huomioida, miten ja millaisessa kontekstissa mitäkin grafiikkaa tarvitaan.
