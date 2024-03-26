# Redux

## instalare:

- `npm install redux`
- `npm install react-redux`

## actions:

1. Stabilim si compunem actiunile (`action`) pe care trebuie sa le faca codul nostru. (`addTask `, `deleteTask `, `editTask `, `filterTask`)

```jsx
export const addTask = (value) => {
  return {
    type: "tasks/addTask",
    payload: value,
  };
};
```

## reducers:

2. Compunem reducerii. Reducerii sunt functii pure care, prin intermediul operatorului `switch`, reduc actiunile la una singura. Reducerii primesc `state` și `action` ca argument. In fiecare caz din instrucțiunea `switch` stabilim logica modificarii state-ului și returnam un nou state. Apoi combinam reducerii (`combineReducers`) si transmitem, prin intermediul lui `rootReducer`, noul state-ul catre store.

## store:

3. Crearea store-ului: Folosind `createStore` din Redux, cream un obiect store care conține întregul arbore al stării aplicației. `rootReducer` este pasat ca argument pentru a inițializa starea inițială a store-ului.
4. Utilizarea store-ului: Store-ul este utilizat în întreaga aplicație pentru a accesa și a actualiza starea aplicației. Prin intermediul `Provider` din `react-redux`, store-ul este făcut disponibil în întreaga ierarhie de componente React.

## selectors:

5. Definim selectorii astfel incat sa extragem state-ul care ne intereseaza din starea globala a aplicatiei.

## dispatch:

6. Folosim funcția dispatch și hook-ul useDispatch pentru a trimite, din componentele React, acțiuni către store-ul Redux.
