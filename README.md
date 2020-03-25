

# duplicate identifier error

I have type `Todo` defined both in `src/reducers/generated/TodosReducer-gen.ts`  and `src/reducers/TodosReducer.ts` 

when i try to compile i am getting following error

```ts
src/reducers/generated/TodosReducer-gen.ts:3:6 - error TS2300: Duplicate identifier 'Todo'.

3 type Todo = {}
       ~~~~

  src/reducers/TodosReducer.ts:2:6
    2 type Todo = {}
           ~~~~
    'Todo' was also declared here.

src/reducers/TodosReducer.ts:2:6 - error TS2300: Duplicate identifier 'Todo'.

2 type Todo = {}
       ~~~~

  src/reducers/generated/TodosReducer-gen.ts:3:6
    3 type Todo = {}
           ~~~~
    'Todo' was also declared here.
```

if i add any import on first line then error going away :s ...