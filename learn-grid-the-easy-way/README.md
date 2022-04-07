# learn-grid-the-easy-way
Tutorial en video de casi 40 minutos por Kevin Powell, sobre CSS Grid con un repositorio para trabajar junto al video. Más abajo está el enlace al video, el repositorio se puede clonar fácilmente desde el terminal con el siguiente comando (requiere la herramienta gh-cli):  

```
gh repo clone kevin-powell/learn-grid-the-easy-way
``` 

## Los enlaces: 
* [Repositorio](https://github.com/kevin-powell/learn-grid-the-easy-way)
* [gh-cli](https://cli.github.com)
* [Video](https://www.youtube.com/watch?v=rg7Fvvl3taU) 
### Notas: 
- 3.45 item elements of a grid or flex container have no longer collapsable margins.
- 9.00 uso de `grid-template-columns` y de la funcion `repeat(howmany, size)` con la unidad específica de grid `fr` 'fraction': 
- `grid-template-columns: repeat(4, 1fr)`
- 11.00 implicit and explicit columns/rows
- 12.00 recomienda no declarar [columnas] filas explícitamente si el layout lo permite.
- 22.00 momento de magia negra con `grid-row-end` para corregir layout
- 28.00 se agrega @media, pero lo interesante es que no solo agrega una. Para ese layout, CSS Grid hace el resto del trabajo.
- 30.00 WOOW más magia negra con `grid-template-areas` **INVESTIGAR BIEN**

### Propiedades más comunes: 
- `display: grid` (container)
- `gap: 2rem` (container)
- `grid-column-template: repeat(4, 1fr)` (container)
- `grid-column: span 2 | 2 4 | 2` (items) (shorthand de las 2 siguientes)
- `grid-column-start: 2` (items)
- `grid-column-end: 5` (items)
- `grid-row: 1 / span 2` (items) (shorthand de las 2 siguientes)
- `grid-row-start: 5` (items)
- `grid-row-end: 5` (items)
- SUPER MAGIA NEGRA PARA CREAR LAYOUTS:
  - `grid-template-areas: 'strings1 string2,...'` (container)
  - `grid-area: string1`  (items)
  - `grid-auto-columns|rows: 1fr` (container)
  - esta ultima crea columnas o filas automáticas a partir del layout definido en grid-template-areas
   