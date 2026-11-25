# MEX Mobile

**Biblioteca ta Jellyfin, pregătită pentru vizionare pe Android.**

[English](README.md) · [Descarcă versiunea beta](https://github.com/minuteoneminute/mex-mobile-releases/releases) · [Raportează o problemă](https://github.com/minuteoneminute/mex-mobile-releases/issues)

MEX Mobile este un client Android independent pentru propriul tău server [Jellyfin](https://jellyfin.org/). Poți răsfoi filmele și serialele, relua vizionarea și pregăti descărcări pentru drum, într-o interfață adaptată telefonului.

**Stadiu: beta.** Funcțiile sunt încă testate și pot avea comportamente diferite în funcție de server, fișiere, telefon și rețea. Apreciem feedbackul și rapoartele de probleme.

## Povestea aplicației

MEX Mobile a pornit de la o nevoie practică: o bibliotecă Jellyfin personală care să fie mai ușor de folosit pe telefon, inclusiv când ești plecat de acasă sau conexiunea nu este stabilă. Proiectul pornește de la [Jellyflix](https://github.com/jellyflix-app/jellyflix) și adaugă interfața MEX pentru mobil și funcții pentru navigare, redare și descărcări.

Este un **client neoficial și independent**, fără afiliere sau aprobare din partea Jellyfin ori Jellyflix. Aplicația nu oferă filme, seriale, server sau cont: te conectezi la un server Jellyfin la care ai deja acces.

## Ce poți face

### Găsești ce vrei să urmărești

- Răsfoiești bibliotecile de filme și seriale, cauți titluri și folosești filtre și sortare. Poți căuta și după actor, regizor sau gen, când serverul oferă metadatele necesare.
- Vezi pe elementele compatibile marcaje pentru conținut vizionat, numărul de episoade nevizionate și indicatoare pentru descărcări.
- Reiei vizionarea, vezi episoadele următoare, descoperi recomandări și păstrezi o listă „De văzut”. Recomandările depind de răspunsul serverului.
- Pe pagina Acasă de pe telefon, episoadele adăugate recent sunt grupate după serial.
- Ascunzi local biblioteci pentru un profil și le reactivezi când vrei. Este o preferință de afișare, nu o metodă de control al accesului; biblioteca rămâne pe server, iar descărcările existente rămân pe telefon.
- Tragi în jos pentru reîmprospătare în Acasă, Library și Downloads.

### Descarci și urmărești offline

- Descarci filme și episoade compatibile în calitate **Original**, **Balanced** sau **Economy**. Conversia depinde de suportul serverului. Dimensiunile estimate sunt orientative și nu sunt întotdeauna disponibile.
- Folosești coada de descărcare cu pauză, reluare, ordonare, reîncercare și istoric de erori. Unele întreruperi temporare sunt reîncercate automat.
- Alegi o limită de spațiu, poți restricționa transferul la rețele nemăsurate și poți cere încărcarea telefonului sau un interval de pornire. Android poate amâna lucrul în fundal, iar unele schimbări de rețea se aplică doar descărcărilor noi.
- Episoadele sunt grupate după serial; poți căuta în descărcări, verifica spațiul și verifica fișierele înainte de plecare. Verificarea controlează existența și dimensiunea fișierelor, fără să garanteze redarea integrală.
- Reiei un titlu offline de la poziția salvată pe telefon. Progresul offline este pus în așteptare pentru sincronizare cu serverul, când este posibil.
- Poți activa descărcarea automată a următorului sau a următoarelor două episoade nevizionate pentru serialele alese și poți proteja descărcări de curățarea automată opțională.

### Redare și instrumente utile

- Alegi pistele audio și subtitrările disponibile, setezi limbi preferate și ajustezi calitatea redării.
- Oprești redarea și revii la titlu, blochezi comenzile sau setezi un cronometru de somn. Poți continua cu episodul următor când este disponibil.
- Folosești profiluri de redare, un widget pentru reluare, diagnosticul conexiunii și notificări opționale pentru episoade noi, terminarea cozii sau revenirea serverului.
- Gestionezi profiluri pentru mai multe servere și te conectezi prin Quick Connect acolo unde este disponibil.
- Poți copia un export limitat al setărilor sau un rezumat de diagnostic după ce îl verifici. Rezumatul nu include credențiale, adrese de server sau titluri.

Unele funcții necesită conexiune la server, iar notificările și activitatea în fundal depind de restricțiile Android. Descărcările și preferințele sunt păstrate pe telefon, dacă nu se precizează altfel. Înainte de plecare, testează descărcările importante în modul avion.

## Ce este diferit față de aplicația oficială Jellyfin?

Ambele aplicații se conectează la un server Jellyfin și permit navigarea și redarea conținutului propriu. [Clientul oficial Jellyfin pentru Android](https://github.com/jellyfin/jellyfin-android) integrează interfața web Jellyfin; MEX Mobile folosește propria interfață Flutter, bazată pe Jellyflix, cu accent pe coada de descărcări, utilizarea offline și prezentarea pe mobil descrise mai sus.

Este o diferență de abordare, nu un tabel complet de funcții. Unele funcții se suprapun sau se pot schimba între versiuni. De exemplu, descărcările offline și cele convertite există și în proiectul [Jellyflix](https://github.com/jellyflix-app/jellyflix). Clientul oficial are propriile avantaje, inclusiv suport Chromecast în distribuția sa proprietară; alege varianta potrivită pentru tine.

## Instalare și conectare

1. Pe un telefon cu **Android 7.0 sau mai nou**, deschide [Releases](https://github.com/minuteoneminute/mex-mobile-releases/releases) și descarcă cel mai nou **APK beta**.
2. Deschide fișierul APK și, dacă Android solicită, permite instalarea din aplicația cu care l-ai descărcat. Instalează MEX Mobile.
3. Introdu adresa propriului server Jellyfin și autentifică-te cu un cont care are acces. Instalările noi nu au o adresă de server precompletată.
4. Pentru acces din afara casei, serverul trebuie să fie accesibil prin configurația ta de rețea. Accesul și conversia conținutului sunt gestionate de instalarea ta Jellyfin.

Pentru actualizare, instalează un APK MEX Mobile mai nou, semnat cu aceeași cheie, peste aplicația existentă și confirmă în Android. Păstrează copii ale datelor importante și citește notele versiunii. Versiunile beta sunt listate în Releases și pot să nu apară sub eticheta stabilă „Latest” de pe GitHub.

## Feedback și confidențialitate

Pentru probleme și propuneri, folosește [GitHub Issues](https://github.com/minuteoneminute/mex-mobile-releases/issues). Include versiunea aplicației, versiunea Android, ce ai făcut și ce s-a întâmplat. **Nu publica parole, tokenuri, adrese private de server sau alte date sensibile.**

## Credite și cod sursă

MEX Mobile este bazat pe [Jellyflix](https://github.com/jellyflix-app/jellyflix), proiect distribuit sub [GPL-3.0](https://github.com/jellyflix-app/jellyflix/blob/main/LICENSE). Mulțumim contributorilor Jellyflix, Jellyfin și celorlalte proiecte open-source care au făcut posibilă aplicația.

Acest repository găzduiește momentan APK-urile publice și documentația. Codul MEX Mobile este întreținut separat; repository-ul Jellyflix original nu conține modificările specifice MEX.
