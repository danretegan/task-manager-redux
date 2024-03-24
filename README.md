# React Redux:

## 1. Definirea acțiunilor:

Se definesc acțiunile pe care dorim să le facă aplicația: `addTask`, `deleteTask`, `toggleCompleted`, `setStatusFilter`. Aceste acțiuni sunt obiecte JavaScript care descriu evenimentele care au loc în aplicație și sunt definite ca constante pentru a le face ușor de referit și gestionat. Aceste acțiuni comunică schimbările de stare și evenimentele către reduceri sau alte părți ale aplicației. Vezi fișierul `actions.jsx`.

## 2. Crearea reducerilor:

Se creează reducerii, care sunt funcții pure. Reducerii preiau starea curentă și o acțiune și returnează o nouă stare în funcție de acțiunea primită. Aceste funcții reducer sunt responsabile pentru actualizarea stării aplicației în funcție de acțiunile care au loc. Vezi fișierul `reducers.jsx`.

## 3. Crearea selectorilor:

Se definesc selectorii pentru a extrage și deriva date din starea globală a aplicației Redux. Selectorii sunt funcții pure care preiau starea Redux și returnează date specifice necesare componentelor React pentru afișare sau alte scopuri. Aceștia pot ajuta la gestionarea formei și structurii stării, la optimizarea performanței și la abstractizarea detaliilor de implementare. Vezi fișierul `selectors.jsx`.

## 4. Crearea store-ului Redux:

Se creează un magazin Redux (store) care combină reducerii și definește starea inițială a aplicației. Acesta este responsabil pentru gestionarea întregii stări a aplicației și distribuirea acțiunilor către reduceri pentru a actualiza starea. Vezi fișierul `store.jsx`.

## 5. Conectarea componentelor React la store:

Componentele React sunt conectate la magazinul Redux (store) pentru a accesa starea aplicației și pentru a trimite (dispatch) acțiuni către store atunci când este necesar. Vezi fișierul `App.jsx`.

## Concluzie:

În această schemă, `acțiunile` sunt trimise la `store` folosind funcția `dispatch`, iar `starea` aplicației este accesată folosind hook-ul `useSelector`. Aceasta este o modalitate simplificată de a descrie modul în care `Redux` poate fi utilizat într-o aplicație `React` pentru a gestiona starea și funcționalitatea aplicației.
