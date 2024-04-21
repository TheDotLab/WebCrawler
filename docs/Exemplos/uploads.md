```js title="upload.js"
upload("Decent Cracker.crc")
seconds_limit(60)
if (target.internet >= Mbits(50)) {

    //Verifica se o servidor de destino tem pelo menos 50 Mbits de velocidade de internet
    upload("Decent Cracker.crc")
    seconds_limit(60)
}
seconds_limit(120)
if (target.label == "NPC") {
    upload("Decent Cracker.crc")
} else {
    upload("Info.txt")
    upload("*.vspam") //É necessário o vspam mais alto (se disponível)
}
if (target.softwares("*").has("*.av") == false) { //Verifica se o servidor alvo possui antivírus
    upload("Generic DDoS.vddos", "install & hide", "1.5")
}
```