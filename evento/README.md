# Convite Evento - OSCG com vendedores individuais

Projeto estático para GitHub Pages.

## Como publicar

1. Envie todos os arquivos para o repositório `convite-evento`.
2. No GitHub, acesse `Settings > Pages`.
3. Selecione a branch principal e a pasta raiz.
4. O site ficará disponível em:

```txt
https://renison-f.github.io/convite-evento/
```

## Como cadastrar vendedores

Abra o arquivo `index.html` e procure por:

```js
const sellers = [
```

Cada vendedor segue este formato:

```js
{
  slug: "joao",
  name: "João",
  whatsapp: "5564999999999",
  phoneLabel: "(64) 99999-9999"
}
```

Campos:

- `slug`: nome usado no link, sem espaço e sem acento.
- `name`: nome que aparece na página e na mensagem.
- `whatsapp`: número com DDI + DDD + número, somente números.
- `phoneLabel`: número formatado para aparecer visualmente.

## Links por vendedor

Exemplos:

```txt
https://renison-f.github.io/convite-evento/?vendedor=joao
https://renison-f.github.io/convite-evento/?vendedor=maria
https://renison-f.github.io/convite-evento/?vendedor=ana
```

## Painel simples para copiar links

Depois de publicar, acesse:

```txt
https://renison-f.github.io/convite-evento/?admin=vendedores
```

Esse modo mostra todos os links cadastrados e permite copiar cada um.

## Observação importante

Este projeto direciona o WhatsApp para cada vendedor e identifica o vendedor na mensagem. Ele não registra vendas automaticamente em banco de dados. Para controle de pulseiras, use uma planilha com:

- vendedor;
- quantidade recebida;
- quantidade vendida;
- quantidade devolvida;
- valor recebido;
- observações.

## Logos dos apoiadores

Os arquivos ficam em:

```txt
assets/img/apoiadores/
```

Nomes esperados pelo HTML:

```txt
maplebear.png
camargo-guarnieri.png
if-goiano.png
```

Substitua as imagens de exemplo pelas artes oficiais quando necessário.
