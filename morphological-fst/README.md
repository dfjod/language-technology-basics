# Morfoloģiskās gramatikas dokumentācija

Šajā projektā izstrādāta morfoloģiskā gramatika latviešu valodai, izmantojot HFST (Helsinki Finite-State Toolkit). Implementētā gramatika fokusējas uz lietvārdu deklināciju modelēšanu. Risinājums sastāv no HFST leksikona (`.lexc` formātā) un papildināts ar Jupyter piezīmju grāmatiņu, kas parāda gramatikas kompilēšanas un testēšanas procesu.

## Implementētā gramatika

Gramatika modelē latviešu valodas lietvārdu dzimtas un locījumu galotnes. Leksikonā tiek definētas šādas galvenās komponentes:

- **Sākuma stāvoklis:** šeit tiek norādīti visi ievades vārdi un to ceļš uz atbilstošajām paradigmas klasēm (1Dekl, 2Dekl, 4Dekl un 6Dekl).
- **Paradigmas:** katrai deklināciju klasei definētas atbilstošās locījuma galotnes (vienskaitlis, daudzskaitlis, nominatīvs, ģenitīvs utt.).
- **Galotnes:** definētas kā atsevišķas vienības, kuras tiek pievienotas vārda saknei, lai izveidotu morfoloģiskās formas.

Jupyter piezīmju grāmatiņā tiek:

- Kompilēts leksikons (`lexicon.lexc`) uz HFST transducētāju.
- Testēti dažādi vārdi, lai pārbaudītu gramatikas darbību.
- Tiek izpildīti ievietošanas un aizstāšanas likumi.
