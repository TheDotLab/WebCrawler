## inputs:
```js
upload("name_of_program" ,"actions", "version")
```

- **name_of_program:** Nome ou trecho do nome. Para escolher o maior disponível use "*"
- **actions:** Existem duas ações disponíveis: "install" e "hide". Por padrão, é atribuído como "install & hide".
- **version:** Versão do programa como "1.5"

## Exemplo:

```js
upload("*.crc", "", "1.5")
```

Ele configurou um upload do cracker superior disponível, que é a versão 1.5. Não será instalado nem oculto. Esta função é usada para definir um software a ser carregado. Cada chamada para esta função anexa um software na fila de upload.