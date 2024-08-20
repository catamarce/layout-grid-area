Practica Grid

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=flat&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=flat&logo=css3&logoColor=white)

### LAYOUT BASICO
Este es un layout basico usando  las propiedades de GRID:
- grid-area - display - grid-template-areas - gap
```css
/*-----------------definicion nombres items(hijos)---------------------------*/
.header {
  grid-area: header;/*define nombre al container .header*/
  background-color: darkviolet;
}
.menu {
  grid-area: menu;/*define nombre al container .menu*/
  background-color: darkviolet;
}
.main {
  grid-area: main;/*define nombre al container .main*/
  background-color: darkviolet;
}
.footer {
  grid-area: footer;/*define nombre al container .footer*/
  background-color: darkviolet;
}
/*---------------------------------------------------------------------------*/

.grid-container {
  height: 100vh;
  display: grid;/*habilita este container a modo grilla*/
  grid-template-areas:/*posiciona items(hijos) usando los nombres arriba definidos*/
   "header header header"
   "menu main main"
   "footer footer footer";
  gap: 10px;/*define espaciado horizontal-vertical entre items(hijos)*/
}
```
Para mas detalles Reviza el archivo: _style.css_
