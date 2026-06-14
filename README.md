# Harjoitusavustaja

Selainpohjainen työkalu harjoitusten suunnitteluun ja visualisointiin. Avaa `index.html` suoraan selaimessa — ei asennuksia.

## Objektit

| Tyyppi | Muoto | Väri |
|---|---|---|
| Pallo | ympyrä | musta/valkoinen |
| Oma pelaaja | ympyrä | sininen, musta reunaviiva |
| Vastustaja | ympyrä | punainen, musta reunaviiva |
| Tötsä | kolmio | oranssi |
| Teksti | lappu | tumma tausta |

## Käyttö

1. Valitse objekti työkalupalkista
2. Klikkaa kenttää lisätäksesi — työkalu pysyy valittuna, voit lisätä useita peräkkäin
3. Raahaa objekteja hiirellä
4. Kaksoisklikkaa muokataksesi nimeä tai tekstiä
5. Hiiren oikea tai **Del** poistaa objektin

## Animaatio

1. Asettele objektit alkutilanteeseen
2. Klikkaa **+ jälkeen** — tallentaa nykyisen hetken
3. Siirrä objekteja uusiin asemiin
4. Toista — keltaiset nuolet näyttävät liikkeen seuraavaan hetkeen
5. **▶** toistaa animaation pehmein siirtymin

Hetkiä voi lisätä myös **+ ennen** -painikkeella, jolloin uusi hetki tulee nykyisen eteen (toimii myös alussa).

## Tallennus ja jako

- **Arkisto** — tallenna harjoitus nimellä selaimen muistiin; lataa tai poista listalta
- **Lataa .json / Avaa .json** — vie tai tuo harjoitus tiedostona (siirto koneelta toiselle, varmuuskopio)
- **Vie video** — tallentaa animaation `.webm`-videoksi; toimii WhatsAppissa Android-laitteilla

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
