# desafio3-curso2-ONE-ALURA-G7
Desarrollo de ejercicios del desafio 3 curso 2 
// 1. 
Crea una función que calcule el índice de masa corporal (IMC) de una persona a partir de su altura en metros y peso en kilogramos, que se recibirán como parámetros.

 function indiceMasaCorporal(peso, estatura) {
   return (peso /(estatura*estatura));
 }
   let resultado = indiceMasaCorporal(60,1.60)

  console.log(`El indice de Masa Corporal es ${resultado}`);

//2.
Crea una función que calcule el valor del factorial de un número pasado como parámetro.
function calcularFactorial(numero) {
    // Verificar si el número es negativo, cero o positivo
    if (numero < 0) {
        return "El factorial no está definido para números negativos";
    } else if (numero === 0) {
        return 1;
    } else {
        let resultado = 1;
        for (let i = 1; i <= numero; i++) {
            resultado *= i;
        }
        return resultado;
    }
}

// Ejemplo de uso
let numero = 3; // Puedes cambiar este valor para probar con otros números
let resultado = calcularFactorial(numero);
console.log(`El factorial de ${numero} es ${resultado}`);



//3.
Crea una función que convierta un valor en dólares, pasado como parámetro, y devuelva el valor equivalente en reales(moneda brasileña,si deseas puedes hacerlo con el valor del dólar en tu país). Para esto, considera la cotización del dólar igual a R$4,80.

function convertirDolaresAReales(dolares) {
  var cotizacionDolar = 4.80; // Cotización fija del dólar
  var reales = dolares * cotizacionDolar;
  return reales;
}

// Ejemplo de uso
var dolares = 10; 
var reales = convertirDolaresAReales(dolares);
console.log(`$${dolares} dólares equivalen a R$${reales.toFixed(2)} reales.`);

//4. 
Crea una función que muestre en pantalla el área y el perímetro de una sala rectangular, utilizando la altura y la anchura que se proporcionarán como parámetros.
function calcularAreaYPerimetro(altura, ancho) {
  // Calcular el área
  var area = (altura * ancho);
  
  // Calcular el perímetro
  var perimetro = (2 * (altura + ancho));
  
  console.log(`El área de la sala es: ${area} metros cuadrados`);
  console.log(`El perímetro de la sala es: ${perimetro} metros`);
}

// Ejemplo de uso
var altura = 5; 
var ancho = 10; 
calcularAreaYPerimetro(altura, ancho);

//5.
Crea una función que muestre en pantalla el área y el perímetro de una sala circular, utilizando su radio que se proporcionará como parámetro. Considera Pi = 3,14.

function calcularAreaYPerimetroCircular(radio) {
  const pi = 3.14;
  // Calcular el área
  var area = pi * (radio * radio);
  
  // Calcular el perímetro
  var perimetro = (2 * pi) * radio;
  
  console.log(`El área de la sala circular es: ${area.toFixed(2)} metros cuadrados`);
  console.log(`El perímetro (circunferencia) de la sala circular es: ${perimetro.toFixed(2)} metros`);
}

// Ejemplo de uso
var radio= 10; 
calcularAreaYPerimetroCircular(radio);

//6.Crea una función que muestre en pantalla la tabla de multiplicar de un número dado como parámetro.

function tablaDeMultiplicar(numero) {
  console.log(`Tabla de multiplicar del ${numero}:`);
  for (let i = 1; i <= 10; i++) {
      let resultado = numero * i;
      console.log(`${numero} x ${i} = ${resultado}`);
  }
}

// Ejemplo de uso
let numero = 5;
tablaDeMultiplicar(numero);
