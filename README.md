# 0376RA4PR1 - Exercicis de DOM

## Descripció
Pràctica d'exercicis de manipulació del DOM amb JavaScript.

## 1_Selecció: Usa querySelector per canviar el color d'un <h1> quan la pàgina carregui.
```js
document.querySelector('#titol-principal').style.color = 'red';
```
# Aqui estic fent que el titol, el text,  sigui d'un color en concret, en aquest cas, vermell #

## 2_Contingut: Fes que un paràgraf <p> mostri "Hola Món" usant textContent.
```js
 document.getElementById('paragraf-hola').textContent = "Hola Món";
```
# Aqui estic canviant el texte del paragraf #

## 3_Atributs: Canvia la 'src' d'una imatge <img> usant setAttribute.
```js
document.getElementById('imatge-canviant').setAttribute('src', 'https://via.placeholder.com/150/0000FF/808080');
```
# Aqui s'esta seleccionant una imatge a una que he posat yo, o sigui, canvia la imatge #

## 4_Estils: Canvia el color de fons (backgroundColor) d'un element en fer-li clic.
```js
let caixa = document.getElementById('caixa-estil');
caixa.addEventListener('click', function() {
    caixa.style.backgroundColor = 'lightgreen';
});
```
# Aqui al fer interaccio amb una caixa, canvia l'estil que tenia per una altre al fer-hi click #

## 5_Classes: Crea un botó que afegeixi/tregui la classe 'actiu' amb classList.toggle.
```js
let botoToggle = document.getElementById('boto-toggle');
let textClasse = document.getElementById('text-classe');
        
botoToggle.addEventListener('click', function() {
    textClasse.classList.toggle('actiu');
});
```
# Aqui al fer click a un boto, trec o afegeixo la classe actiu #

## 6_Esdeveniments: Afegeix un addEventListener a un botó perquè tregui una alerta (alert).
```js
let botoAlerta = document.getElementById('boto-alerta');
botoAlerta.addEventListener('click', function() {
    alert("Has fet clic al botó d'alerta!");
});
```
# Aqui al fer click al boto, em surt una alerta on m'ha avisa que li he clickat al boto #

## 7_Estructura: Crea un nou <li> amb createElement i afegeix-lo a una <ul> amb appendChild.
```js
let botoAfegir = document.getElementById('boto-afegir');
let llista = document.getElementById('llista-compra');

botoAfegir.addEventListener('click', function() {
    let nouItem = document.createElement('li');
    nouItem.textContent = "Ous";
    llista.appendChild(nouItem);
});
```
# Al fer-hi click crea un li nou #

## 8_Eliminació: Fes que un element desaparegui en fer-li clic usant el mètode remove().
```js
let elementEliminar = document.getElementById('element-eliminar');
        
elementEliminar.addEventListener('click', function() {
    this.remove();
});
```
# Aqui al clicar-hi al boto, elimina un element #