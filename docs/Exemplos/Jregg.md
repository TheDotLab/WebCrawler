Esse era um modelo que o Jregg usava.

``` js title="jregg.js"
//Este script requer que você tenha pelo menos um dos seguintes vírus (desinstalados) para funcionar corretamente: spam, warez, vminer e vddos. É desejável um hdr (hidder) também.
//Se o destino tiver menos de 10 MB
if (target.freehd < MB(10)) {
    //Se o destino tiver pelo menos 4 MB
    if (target.freehd >= MB(4))
        //Upload spam
        upload("*.vspam")
} else
    //Se a máquina tiver mais de 10MB
     //Se a máquina tiver mais de 10Mbits
    if (target.internet > Mbits(10)) {
        //Se os vírus warez que já estão na máquina estiverem recebendo menos de 10 Mbits
        if ((target.internet / target.softwares("*.vwarez", true).list.length) < Mbits(10)) {
            //Se a máquina já tiver um miner
            if (target.softwares().has_installed(".vminer")) {
                //Se a máquina tiver pelo menos 1 GB de espaço livre
                if (target.freehd >= GB(1)) {
                    //Faz o upload de um ddos ou um miner
                    switch (Math.floor((Math.random() * 2) + 1)) {
                        case 1:
                            upload("*.vddos")
                            break
                        case 2:
                            upload("*.vminer")
                            break
                        default:
                            break
                    }
                }
                //Se a máquina tiver menos de 1GB livre, faz o upload do ddos
                else
                    upload("*.vddos")
            }
            //Se a máquina não tiver um minerador instalado, faz o upload
            else
                upload("*.vminer")
        }
        //Se o warez estiver recebendo 10 Mbits cada, faz o upload do warez
        else
            upload("*.vwarez")
    }
else
    //Se a máquina não tiver 10Mbits
     //Se houver um miner instalado
    if (target.softwares().has_installed(".vminer")) {
        //Se a máquina tiver mais de 1GB de espaço
        if (target.freehd >= GB(1)) {
            //upload DDoS ou miner
            switch (Math.floor((Math.random() * 2) + 1)) {
                case 1:
                    upload("*.vddos")
                    break
                case 2:
                    upload("*.vminer")
                    break
                default:
                    break
            }
        }
        //Se a máquina tiver menos de 1GB de espaço, upload o ddos
        else
            upload("*.vddos")
    }
//Se a máquina não tiver um miner instalado, instale um
else
    upload("*.vminer")
```

Para usá-lo com eficiência, substitua as instruções "if (target.freehd[…])" por tamanhos adequados ao seu software.