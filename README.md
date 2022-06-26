# fix_agartool_24_06_22
Un pequeño scritp para reparar un bug existente en éstas fechas en agartool.
Sucede que se rompen los vínculos a las hojas de estilo y por ese motivo se rompe el formato de la app y no se puede jugar.
Pegando este script en la consola de las herrameintas de desarrollador de chromium o sus derivadas se le de solución temporal al problema.


document.getElementsByTagName("body")[0].style.overflow = 'hidden';
document.getElementsByTagName("body")[0].style.margin = 0;
document.getElementsByClassName("offerwall-btn")[0].style.display = 'none';
let canvas = document.getElementsByTagName("canvas")[0];
canvas.style.position = 'absolute';
canvas.style.margin = 0;
