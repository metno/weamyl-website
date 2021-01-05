---
permalink: /about_ro/
title: "Despre proiectul WeaMyL"
---

[EN](/about/){: .btn .btn--primary}

Proiectul WeaMyL își propune să îmbunătățească acuratețea, performanța și fiabilitatea sistemelor naționale de avertizare nowcasting prin utilizarea tehnicilor de învățare automată (ML) aplicate pe observațiile radarului, satelitului și stațiilor meteo. Accentul se va pune pe obținerea unei precizii mai mari în prezicerea apariției și a zonelor afectate de fenomene meteorologice severe, precum și pe obținerea unor timpi de decizie mai mici (în comparație cu timpi de decizie actuali, exclusiv umani). Scopul principal al proiectului este de a automatiza sistemele de avertizare nowcasting prin crearea unei platforme bazate pe ML pentru prognoza timpurie și precisă a fenomenelor severe. Astfel, se urmărește să fie coloana vertebrală a unui nou cadru pentru detectarea iminentă a vremii severe, adaptat posibilităților tehnologice actuale.

## Obiective principale

Principalele obiective ale proiectului sunt următoarele:

* Dezvoltarea și validarea științifică a noilor modele și tehnici de calcul ML adaptate special pentru nowcasting de precizie. Modele de învățare nesupervizate (UL), cum ar fi analiza componentelor principale, _clustering_ și _autoencodere_ sunt avute în vedere ca instrumente inteligente pentru analiza mai multor surse de date, care pot fi relevante pentru nowcasting: date meteorologice (radar, satelit, observațiile stațiilor meteorologice) și datele geografice (altitudine, expunere, vegetație, elemente hidrologice, elemente antropice). În urma analizei datelor în mod nesupervizat, vor fi dezvoltate atât metode de învățare supervizate online, cât și off-line, cum ar fi rețelele neuronale convoluționale, rețelele U, rețelele de tip LSTM, XGBoost și mașinile restricționate Boltzmann, pentru a ajuta meteorologii să furnizeze alerte precise de nowcasting.


* Dezvoltarea și evaluarea de către utilizator a Atlasului adnotat de observații meteorologice, o bază de date mare care conține date meteorologice (radar, satelit și alte observații meteorologice relevante) fiind utilizată ca sursă de date pentru tehnicile de învățare profundă dezvoltate în cadrul proiectului (extragerea, prelucrarea și clasificarea datelor). După finalizarea proiectului, Atlasul adnotat va fi disponibil pentru analize de date meteorologice, redactări  de lucrări științifice, instruire a personalului și diseminarea publică a datelor meteorologice. Atlasul va oferi:
  1. gestionarea observațiilor meteorologice adnotate (adăugarea, actualizarea, salvarea, încărcarea, adnotarea și validarea înregistrărilor meteorologice) și
  2. tehnici inteligente de recuperare a informațiilor pentru recuperarea informațiilor istorice relevante pentru meteorologi în timp real. Aceasta include identificarea timpurie a zonelor predispuse la inițierea convecției pe baza datelor statistice, precum și identificarea modelelor de furtună convectivă pe baza datelor istorice. Diferite interogări și vizualizări pentru observații specifice vor fi accesibile și le vor include pe cele furnizate de metodele nesupervizate dezvoltate ca parte a O1 împreună cu diferite rezultate de raportare.


* Dezvoltarea platformei open-source WeaMyL pentru prognoza timpurie a fenomenelor meteorologice severe. Obiectivul este de a oferi o platformă de prognoză bazată pe _big data_, care să includă metodele de învățare supervizată dezvoltate și care să sprijine meteorologii în îmbunătățirea calității alertelor emisie acum.

* Integrarea platformei WeaMyL în cadrul sistemelor naționale de avertizare meteorologică din Norvegia și România. Platforma WeaMyL va fi integrată cu sistemele software relevante ale Serviciilor Meteorologice Naționale. Această integrare va facilita în mod direct activitatea meteorologilor, asistându-i în procesul de decizie nowcasting și va accelera procedurile de emitere a alertelor.

* Contribuiția la dezvoltarea cunoștințelor științifice prin diseminarea rezultatelor științifice obținute prin publicații științifice, site-ul web al proiectului și social media.

## Platforma software WeaMyL

Platforma software WeaMyL este formată din trei componente:

* **Platformă de prognoză.** Având în vedere că acuratețea modulului de predicție este primordială pentru precizia sistemului, aceasta este componenta centrală a WeaMyL. Platforma de prognoză utilizează atât date istorice cât și date în timp real și este responsabilă cu estimarea locației, a timpului și a gravității fenomenelor meteorologice care se așteaptă să aibă loc în viitorul apropiat (0-6 ore). Algoritmii noștri vor modela situația meteorologică pe baza situațiilor meteorologice anterioare. Modelele de învățare antrenate vor găsi modele în datele meteorologice care se aplică circumstanțelor specifice și astfel se îmbunătățesc pe măsură ce devin disponibile din ce în ce mai multe date, făcând astfel modulul de prognoză autoadaptativ. Pentru a procesa cantitatea disponibilă de date meteorologice și pentru a accelera analiza științifică și extragerea informațiilor, vor fi vizate abordările _big data_.

* **Atlas adnotat de observații meteorologice.** Componenta Atlas adnotat va furniza o bază de date semantică asupra volumului mare de date istorice din surse variate, inclusiv observațiile stațiilor meteo, radar și imagini prin satelit. Principalele sale obiective sunt de a facilita studiul condițiilor din trecut utilizând analize statistice și comparative, furnizarea de informații inteligente bazate pe un model de date semantice și furnizarea unui model de adnotare personalizat, extensibil, între tipurile și sursele de observație. Componenta Atlas va oferi două funcționalități principale: (a) gestionarea Atlasului și (b) vizualizări, statistici și rapoarte bazate pe datele meteorologice istorice stocate în Atlas.
* **Modul de integrare.** Pentru ca componentele de mai sus să ofere informații acționabile, acestea trebuie să fie integrate cu sistemele software existente. Scopul acestui modul este de a oferi o serie de conectori pentru consumatori și furnizori de date care pot fi integrați în sistemele existente. Atât Platforma de prognoză, cât și Atlasul adnotat vor acționa ca consumatori pentru datele meteorologice generate în timp real, în timp ce platforma de prognoză va furniza date relevante pentru vremea severă viitoare.

## Pachete de lucru

Programul de lucru este împărțit în cinci pachete de lucru (WPs), urmând etapele obișnuite necesare pentru atingerea principalului obiectiv de cercetare, și anume dezvoltarea platformei software WeaMyL. Acestea sunt:

### WP1 - Documentație, cerințe de sistem și arhitectură
În acest pachet de lucru, vom efectua mai întâi o documentare, un studiu și analize de literatură. Apoi, vom identifica limitările abordărilor și soluțiilor de ultimă generație existente în tehnologia nowcasting. Ulterior, ne propunem să definim cerințele funcționale și nefuncționale pentru WeaMyL, inclusiv cerințele utilizatorului final, precum și principalele condiții pentru buna funcționare a sistemului, pentru a stabili arhitectura generală și proiectarea platformei software WeaMyL.

### WP2 - Modele de învățare automată pentru nowcasting
Cel de-al doilea pachet de lucru constă în definirea unui model teoretic pentru nowcasting împreună cu (2) Dezvoltarea de modele ML scalabile special adaptate pentru nowcasting precis. (3) Validarea științifică a modelelor ML dezvoltate utilizând analiza și interpretarea rezultatelor experimentale, precum și comparația cu alte abordări din literatură.

### WP3 - Dezvoltare software, testare și integrare
WP3 se concentrează pe dezvoltarea de software, testarea și integrarea platformei cu sistemele naționale de avertizare. Platforma de prognoză este alcătuită din componentele ML (accesibile printr-un API) împreună cu front-end-ul. Se depune un efort privind integrarea WeaMyL cu sistemele naționale de avertizare. Prototipul platformei va fi dezvoltat într-o manieră incrementală, iterativă, având ca obiectiv final integrarea cu succes în sistemele de avertizare meteorologică din România și Norvegia.


### WP4 - Evaluare, interpretare și analiză meteorologică
Activitățile WP4 includ extragerea, adnotarea și validarea datelor meteorologice relevante din bazele de date NMA și MET și pilotarea platformei în locațiile ANM și MET. Aceste activități vor fi coordonate de ANM în strânsă cooperare cu MET-ML. Rezultatele privind acuratețea, performanța și fiabilitatea platformei vor fi discutate cu MET-IT și UBB. Feedback-ul va fi utilizat pentru a îmbunătăți continuu modulele ML, componentele front-end și Atlasul adnotat.
