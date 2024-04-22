Modelo pra usar quando um NPC tiver internet maior ou igual a 500MB se nao tiver instala outro virus de sua preferencia .
mude os MB da internet para seu gosto, o padrao é 500MB

```js title="Internet.js"
if (target.internet >= Mbits(500)) {
  upload("nome_virus.vwarez", "install", "1.0");
  seconds_limit(120)
} else {
  upload("nome_virus.vminer", "install", "1.0");
  seconds_limit(120)
}
```