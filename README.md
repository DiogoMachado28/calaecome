[README.md](https://github.com/user-attachments/files/27475233/README.md)
# O que há para jantar? 🍽️

App simples para decidir o jantar. Escolhe a base (arroz, batata ou massa) e a proteína — a app sorteia um prato da base de dados.

## Como usar

Abre o `index.html` diretamente no browser, ou coloca num servidor estático (GitHub Pages, por exemplo).

## Adicionar pratos

Abre o `index.html` e encontra a secção `BASE DE DADOS` no script. Para adicionar um prato, copia este bloco:

```js
{
  name: "Nome do prato",
  base: ["arroz"],         // "arroz", "batata" ou "massa"
  proteins: ["feijao"]     // ver lista abaixo
},
```

**Opções de base:** `arroz` · `batata` · `massa`

**Opções de proteína:** `cogumelos` · `feijao` · `grao` · `carne` · `atum` · `peixe` · `queijo` · `ovo`

Um prato pode ter mais do que uma base ou proteína:

```js
{
  name: "Puré com grão de bico, cogumelos e manteiga de amendoim",
  base: ["batata"],
  proteins: ["grao", "cogumelos"]
},
```

## Roadmap

- [ ] Histórico para evitar repetições recentes
- [ ] Avaliação de pratos
- [ ] Modo "o que há no frigorífico"
