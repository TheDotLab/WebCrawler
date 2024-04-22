Esse Modelo faz upload e instala 2 virus de uma vez. 
mude conforme seu gosto.

```js title="2_virus.js"
if (target.internet >= Mbits(500)) {
  upload("nome_virus.vwarez", "install", "3.0");
  upload("nome_virus.vddos", "install", "1.1");
  seconds_limit(120)
} else {
  upload("nome_virus.vminer", "install", "1.1");
  upload("nome_virus.vddos", "install", "1.1");
  seconds_limit(120)
}
```