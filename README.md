# React Redux:

## 1. Definirea acțiunilor:

Se definesc acțiunile pe care dorim sa le faca aplicația: `addTask`, `deleteTask`, `toggleCompleted`, `setStatusFilter` Aceste `actiuni` sunt `obiecte JavaScript` care descriu evenimentele care au loc în aplicație. De obicei, sunt definite ca `constante` pentru a le face ușor de referit și de gestionat. Aceste acțiuni comunică schimbările de stare și evenimentele către reduceri sau alte părți ale aplicației. Vezi fisierul `actions.jsx`.

## 2. Crearea reducerilor:

Se creează `reduceri` care sunt `funcții pure`. Reducerii preiau `starea` curentă și o `acțiune` și returnează o nouă stare în funcție de acțiunea primită. Aceste `functii reducer` sunt responsabile pentru actualizarea stării aplicației în funcție de acțiunile care au loc.

## 3. Crearea store-ului Redux:

Se creează un magazin Redux (`store`) care combină reducerii și definește starea inițială a aplicației. Acesta este responsabil pentru gestionarea întregii stări a aplicației și distribuirea acțiunilor către reduceri pentru a actualiza starea.

## 4. Conectarea componentelor React la store:

Componentele React sunt conectate la magazinul Redux (`store`) pentru a accesa starea aplicației și pentru a trimite (dispatch) acțiuni către store atunci când este necesar.

## Concluzie:

În această schemă, `acțiunile` sunt trimise la `store` folosind funcția `dispatch`, iar `starea` aplicației este accesată folosind hook-ul `useSelector`. Aceasta este o modalitate simplificată de a descrie modul în care `Redux` poate fi utilizat într-o aplicație `React` pentru a gestiona starea și funcționalitatea aplicației.
