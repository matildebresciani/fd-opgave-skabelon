# Opgaveskabelon til Frontend Design tema på Frontend-valgfaget

Se opgavebeskrivelsen på Fronter.

## Medfølgende API

Der medfølger en simpel API, som du kan bruge til at hente data til din opgave. Det er ikke et krav til opgaven, men det kan gøre det nemmere og hurtigere at få tekst og billeder ind i dit projekt.

Dokumentationen til API'et finder du på: [https://frontend-design-theme.netlify.app/](https://frontend-design-theme.netlify.app/).

Her er et eksempel på, hvordan du kan hente data fra API'et:

```astro
const employeesData = await fetch(
  "https://frontend-design-theme.netlify.app/api/employees"
).then((response) => response.json());

console.log(employeesData);
```

## Refleksion

## Reflekter kort men fagligt over din løsning med henblik på udfordringerne og successerne ved opgaven.

Jeg synes jeg er kommet godt i mål med mange ting, men jeg ville ønske der have været mere tid (bare en dag mere kunne have været brugbart).
Nogle af udfordringerne var at det var en meget stor opgave der var uoverskuelig at gå i gang med, men når man først var inde i det og havde sat mange af tingene op var det nemmere at arbejde med. Det var også svært at få tilpasset de forskellige eksempler og tidligere opgaver vi har lavet på forløbet, til lige netop den her opgave.

## Fremhæv specifikke kodestumper, der illustrerer brugen af forskellige teknikker og principper (gerne fra undervisningen).

Jeg har prøvet at bruge spacing og font sizes fra utopia så godt som muligt på min elementer.

Jeg har gjort meget brug af nesting undervejs.

Derudover har jeg også lavet subgrid og brugt at navngive mine columns i layout.
fx:
grid-template-columns:
[full-start] 1fr [content-start] minmax(0, var(--content-half))
[middle] minmax(0, var(--content-half)) [content-end] 1fr [full-end];

## Forklar, hvordan du har organiseret din CSS; hvornår er det globalt, og hvornår er det komponent-specifikt.

Jeg har mest gjort brug af det globale til at lave custom properties også sætte font sizes, line heights, font weight og lign på min tekst.
Ellers er det meste blevet lavet i hver sit komponent, men med meget brug af custom properties.
