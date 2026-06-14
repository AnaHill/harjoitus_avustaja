# Harjoitusavustaja
Avustaja suunnittelemaan ja visualisoimaan harjoituksia

## Toteutus
Selainpohjainen työkalu harjoituksen esittämisen. Toimii suoraan selaimessa ilman asennuksia — avaa `index.html`.

## Tarpeet
- tehdä yksinkertaisia animaatioita, missä voi liikuttaa ainakin seuraavia yksinkertaisia objekteja
  - peliväline: ympyrä eli pallo
  - omat pelaajat; neliö tai ympyrä
  - vastustajat, eri värillä kuin omat pelaajat
  - tötsät tms vaikka kolmioina
- voisin laittaa selitystekstiä tiettyihin kohtiin

## Ideoita jatkokehitykseen
- pohjalle voisi laittaa yksinkertaisen osan kenttää, eri kentän kohdista eri lajeista 
- Käyttäjä voi valita sopivan hahmotelma
- esimerkiksi jalkapallo
  - koko kenttä
  - puolet kentästä
  - hieman maalivahdin aluetta suurempi kokonaisuus, maalintekoharjoituksia varten
- koripallossa sitten esimerkiksi hyökkäysalue
- ringetessä tai jääkiekossa kaukalo viivoineen
- jne

### Tallennusparannusta
Tallennus voisi olla parempi. Esimerkiksi animaation jako whatsappiin vaikutti hankalalta. Osaatko suositella tapoja? Ehdota, älä toteuta.

Clauden ehdotus

Pysyvä käyttö / jaa muille -->	Netlify Drop

Netlify Drop on todennäköisesti kätevin pitkällä tähtäimellä — yksittäinen HTML-tiedosto menee suoraan ilman rekisteröitymistä ja saat https://-osoitteen joka toimii WhatsApp-jaon kanssa kaikkialla.

Netlify Drop — pysyvä, ei vaadi serveriä
1. Mene netlify.com/drop
2. Raahaa index.html sivulle
3. Saat julkisen https://-osoitteen (esim. https://random-name.netlify.app)
4. Toimii kaikilla laitteilla, ei vaadi konetta päällä

Tämä on paras vaihtoehto jos haluat jakaa sovelluksen myös muille valmentajille

Tietokone (Netlify-osoite)
  → teet harjoitteen
  → tallennat JSON-tiedostoksi varmuuskopioksi
  → vie video → WhatsApp

Puhelin (sama Netlify-osoite)
  → oma erillinen localStorage
  → voit avata tietokoneelta siirretyn JSON:n

Jos haluat vain tehdä harjoitteen ja jakaa videon WhatsAppiin → Netlify Drop on täydellinen, yksinkertainen, toimii.

Jos haluat arkiston kaikilla laitteilla → helpoin ratkaisu olisi tallentaa JSON-tiedostot Google Driveen tai vastaavaan ja avata ne "Kansio"-toiminnolla aina tarvittaessa. Ei vaadi mitään lisäkehitystä.

Itse arvioisin että Netlify + JSON Google Driveen on riittävä ja yksinkertainen ratkaisu — varsinainen palvelin ei tuo niin paljon lisäarvoa että sen rakentaminen kannattaisi.
