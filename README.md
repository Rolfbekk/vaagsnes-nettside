# Gutta Velsigner – nettside

Nettside for **Gutta Velsigner**, et frivillig initiativ fra Unge Voksne i Sørlandskirken.
Praktisk hjelp, ekte omsorg – helt gratis.

Dette er en **prototype**. Hele siden ligger i én fil, `index.html` (HTML, CSS og JavaScript),
uten byggesteg eller avhengigheter som må installeres.

## Se siden

Dobbeltklikk på `index.html`, så åpnes den i nettleseren.

Vil du heller kjøre en lokal server (f.eks. for å teste på mobil på samme nett):

```sh
python3 -m http.server 8000
# åpne http://localhost:8000
```

## Komme i gang

```sh
git clone https://github.com/Rolfbekk/vaagsnes-nettside.git
cd vaagsnes-nettside
```

## Slik jobber vi sammen

1. **Hent siste versjon** før du starter: `git checkout main && git pull`
2. **Lag en egen gren** for endringen din: `git checkout -b kort-beskrivelse`
3. Gjør endringen, sjekk at siden ser riktig ut i nettleseren, og commit.
4. **Push grenen** (`git push -u origin kort-beskrivelse`) og åpne en **pull request** på GitHub.
5. La en av de andre se over før den merges inn i `main`.

Siden alt ligger i én fil, er det lurt å si fra til de andre hva du jobber med,
så vi unngår at to personer endrer samme del samtidig.

## Greit å vite om koden

- **Eksempeldata:** Forespørsler, historier og frivillige i `db`-objektet er oppdiktet. Ingen ekte personopplysninger skal inn i koden.
- **Skjemaene sender ingenting ennå.** Innsendt data lagres bare i nettleseren til siden lastes på nytt.
- **«For ledere» (admin)** har passordet `demo`. Det er bare en demo og gir ingen ekte sikkerhet.
- **Plassholdere:** Kontaktperson, e-post, telefon og møtetid står i `church`-objektet øverst i `<script>` som `[…]` og må fylles inn.
- **Fonter:** Caveat Brush og Bebas Neue er lagt inn direkte i filen (de to veldig lange linjene øverst i `<style>`). Ikke rediger dem for hånd. DM Sans hentes fra Google Fonts.
