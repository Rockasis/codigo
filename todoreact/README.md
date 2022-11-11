LocalStorage
Es una funcion de JS la cual nos permite guardar informacion en memeoria del navegador, es decir, en el disco duro del usuario.

Como funciona?
LocalStorage tiene dos metodos principales:

setItem: Guarda un valor en el LocalStorage
Ejemplo

// 'nombre' => key
// 'Juan' => value
localStorage.setItem('nombre', 'Juan');
Podemos guardar un objeto en el LocalStorage

const persona = {
  nombre: 'Juan',
  edad: 30
};

localStorage.setItem('persona', JSON.stringify(persona));
getItem: Obtiene un valor del LocalStorage por el key
Ejemplo

const nombre = localStorage.getItem('nombre');
console.log(nombre); // Juan

const persona = JSON.parse(localStorage.getItem('persona')); 
Como eliminar un valor del LocalStorage?
LocalStorage tiene un metodo para eliminar un valor por el key

removeItem: Elimina un valor del LocalStorage por el key
Ejemplo

localStorage.removeItem('nombre');
Como eliminar todos los valores del LocalStorage?
LocalStorage tiene un metodo para eliminar todos los valores

clear: Elimina todos los valores del LocalStorage
Ejemplo

localStorage.clear();