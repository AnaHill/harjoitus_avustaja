# Harjoitusavustaja

Selainpohjainen työkalu harjoitusten suunnitteluun ja visualisointiin. Avaa `index.html` suoraan selaimessa — ei asennuksia.

## Objektit

| Tyyppi | Muoto | Väri |
|---|---|---|
| Pallo | pieni ympyrä | musta, valkoinen reuna |
| Oma pelaaja | ympyrä + numero | sininen, musta reuna |
| Vastustaja | ympyrä + numero | punainen, musta reuna |
| Tötsä | pieni kolmio | oranssi |
| Teksti | moniriviset tekstilaput | tumma tausta |

Pelaajien numerointi löytää aina pienimmän vapaan numeron — poistaminen ei hyppää numerointia.

## Käyttö

- Valitse objektityyppi työkalupalkista — työkalu pysyy valittuna, voit lisätä useita peräkkäin
- Klikkaa kenttää lisätäksesi objektin
- **Raahaa** siirtääksesi
- **Kaksoisklikkaa** muokataksesi nimeä, numeroa tai tekstiä
- **Hiiren oikea** tai **Del** poistaa objektin

Tekstilappu näkyy **vain siinä hetkessä johon se lisätään**. Poisto koskee vain nykyistä hetkeä.

## Animaatio

1. Asettele objektit alkutilanteeseen
2. **+ jälkeen** — lisää uusi hetki nykyisen jälkeen (kopio nykyisestä)
3. Siirrä objekteja uusiin asemiin
4. Keltaiset nuolet näyttävät liikkeen seuraavaan hetkeen
5. **▶** toistaa animaation pehmein siirtymin

**+ ennen** lisää hetken nykyisen eteen — toimii myös aivan alussa.  
Hetkiä voi poistaa 🗑-napilla animaatiopalkista.

## Tallennus ja jako

### Arkisto (Arkisto-nappi)
- **Tallenna nimellä** → tallennetaan selaimen muistiin (localStorage), pysyy tallessa vaikka sivu ladataan uudelleen
- **Lataa .json** → vie harjoitus tiedostona varmuuskopioksi tai siirtoa varten
- **Avaa .json** → lataa aiemmin viety harjoitus
- **📁 Kansio** → selaa paikallista kansiota ja lataa sieltä .json-tiedostoja (Chrome/Edge)

Arkisto on laitekohtainen — puhelimen ja tietokoneen arkistot ovat erilliset. JSON-tiedoston voi siirtää laitteiden välillä manuaalisesti.

### Videon vienti (Vie video -nappi)
Tallentaa animaation videotiedostoksi:
- **Mobiili (Android/iOS):** avaa natiivi jakolistan — valitse WhatsApp suoraan
- **Tietokone:** lataa MP4- tai WebM-tiedoston

Formaatti valitaan automaattisesti: MP4 iOS:llä, WebM muilla.

## Käyttö puhelimella

`file://`-protokolla rajoittaa joitain ominaisuuksia (erityisesti videon jako). Suositukset:

**Nopea testi (sama WiFi):**
```
npx serve .
```
Avaa puhelimella `http://192.168.x.x:8000` (oman koneen IP).

**Pysyvä ratkaisu:** julkaise Netlify Dropissa (netlify.com/drop) raahaamalla `index.html` — saat `https://`-osoitteen joka toimii kaikilla laitteilla.

## Näppäinoikotiet

| Näppäin | Toiminto |
|---|---|
| `V` | Valitse ja siirrä |
| `P` | Pallo |
| `O` | Oma pelaaja |
| `R` | Vastustaja |
| `T` | Tötsä |
| `K` | Teksti |
| `← →` | Hetket |
| `Välilyönti` | Toista / pysäytä |
| `Del` | Poista valittu |
| `Esc` | Takaisin valintatyökaluun |

Ohjeet löytyvät myös sovelluksen **?**-napista.
