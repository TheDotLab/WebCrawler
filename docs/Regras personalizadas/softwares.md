```js
softwares(["name_or_snippet", "only_installed"])
```

- **name_or_snippet:** Por padrão é atribuído como "*", ou seja, todos os softwares.

 - **only_installed (bool):** Por padrão é atribuído como falso. Faz a função de trazer softwares recém-instalados. Esta função retorna um objeto que contém a lista dos softwares.

## Atributos e métodos

- **list:** Contém um array com todos os softwares encontrados.

- **has("name_or_snippet"):** A função retorna verdadeiro ou falso. Ele verifica se existe algum software específico na lista.

- **has_installed("name_or_snippet"):** Exatamente como o nome sugere;)

## Exemplos:

```js
console.log(softwares(".crc").list)

if (target.softwares().has_installed("*.av")) {
    window.alert("Não vou instalar nada aqui")
}
```