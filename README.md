# Prinsipper

## Kontinuerlig leveranse

## Gjennomgripende navnkonvensjoner

## Kode-sentrisk


## Infrastruktur som kode
Absolutt all infrastruktur skal være definert som kode. Dette omfatter selvsagt databaser og annen infrastruktur for
applikasjoner, men det omfatter også alt som har med det å utvikle og vedlikeholde applikasjonene. Eksempler på sistnevnte
er AD-grupper for utviklingsteamet, GitHub teams og repo, m.m..

## Multi-sky
Plattformen bør å kunne kjøre på flere skyer, og være uavhengig av en spesifikk sky. Dette gjør at vi kan velge den 
beste skyen for en gitt oppgave, og at vi kan flytte applikasjonen til en annen sky uten å måtte endre kode.

I utgangspunktet er det naturlig å sentrere utvikling rundt en skyplattform, men man bør ha prinsippene rundt multi-
sky i bakhodet, hvilket medfører:
* Kode skal i størst mulig grad være uavhengig av en spesifikk skyplattform
* Komponenter for "cross cutting concerns" (for eksempel "key vault" for håndtering av applikasjonshemmeligheter) bør være uavhengig av en spesifikk skyplattform
* Åpne standarder bør benyttes i kode for standard oppførsel som logging (open telemetry).

## Kostnadskontroll