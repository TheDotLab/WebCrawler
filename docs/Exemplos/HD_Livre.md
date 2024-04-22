Modelo pra usar quando um NPC tiver Espço em disco maior ou igual a 300MB instavala VDDOS 5.0 se nao tiver instala um 1.0 ou de sua preferencia .
mude os MB da HD para seu gosto, o padrao é 300MB

```js title="HD_livre.js"
if (target.freehd >= MB(300)) {
  upload("Advanced DDoS.vddos", "install", "5.0");
  seconds_limit(120)
} else {
  upload("Advanced DDoS.vddos", "install", "1.0");
  seconds_limit(120)
}
```

outro modelo 

```js
if (target.freehd >= MB(300)) {
  upload("nome_virus.vwarez", "install", "5.1");
  seconds_limit(180)
} 
else {
  upload("nome_virus.vspam", "install", "1.0");
  seconds_limit(120)
}

```