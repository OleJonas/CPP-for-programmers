## Oppgave 2
Dette er ikke trygt siden man bare setter av en adresse til pekeren. Å bruke strcpy til å kopiere "Dette er en tekst" over til pekeren vil gå utenfor minneområdet som er satt av til den. Det kan føre til at vi ødelegger dataene som eventuelt lå her siden vi ikke hadde reservert denne plassen til en char-tabell (det er jo tross alt det en tekststreng er).

## Oppgave 3
I denne kodebiten er det bare satt av plass til 5 tegn inkludert nullstrengen. Det å ta ukontrollert input fra brukeren med cin og legge det inn i tekst kan føre til at man går utover det maksimale minneområdet satt av til tabellen text. Da kan man ødelegge data som ligger utenfor minneområdet som er ment å bli brukt. Samtidig kan man risikere å havne i en løkke som går helt til siste minneadresse programmet har fått tilgang til og endre dataene på disse til 'e'.