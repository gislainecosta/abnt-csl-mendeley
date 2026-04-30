# 📚 Adaptado de UFRGS - ABNT 6023:2025 e 10520:2023 com DOI

Este repositório contém um estilo CSL customizado para uso no **Mendeley Cite**, adaptado a partir do estilo **UFRGS-ABNT**.

O objetivo desta adaptação é manter a estrutura geral do estilo UFRGS-ABNT e acrescentar ajustes voltados ao uso acadêmico conforme a **ABNT 6023:2025**, para referências, e a **ABNT 10520:2023**, para citações.

---

## 📑 Sumário

- [📄 Arquivo do estilo](#-arquivo-do-estilo)
- [✨ Principais adaptações](#-principais-adaptações)
- [🔗 URL Raw do estilo](#-url-raw-do-estilo)
- [🧭 Como obter a URL Raw pelo GitHub](#-como-obter-a-url-raw-pelo-github)
- [⚙️ Como instalar no Mendeley Cite usando a URL](#️-como-instalar-no-mendeley-cite-usando-a-url)
- [🔄 Passo importante após instalar ou trocar o estilo](#-passo-importante-após-instalar-ou-trocar-o-estilo)
- [✅ Como conferir se o estilo correto foi instalado](#-como-conferir-se-o-estilo-correto-foi-instalado)
- [🧾 Observações sobre DOI, ISBN e ISSN](#-observações-sobre-doi-isbn-e-issn)
- [📝 Recomendação de uso](#-recomendação-de-uso)
- [⚖️ Licença](#️-licença)
- [👤 Créditos](#-créditos)

---

## 📄 Arquivo do estilo

O arquivo principal deste repositório é:

```text
adaptado-ufrgs-abnt-2025-com-doi-github.csl
```

---

## ✨ Principais adaptações

- Inclusão de DOI nas referências.
- Priorização do DOI quando disponível.
- Tratamento de ISBN e ISSN conforme o tipo documental.
- Prioridade de identificadores por tipo de documento:
  - artigos: DOI prioritário; ISSN apenas como alternativa;
  - livros: DOI prioritário; ISBN como alternativa;
  - capítulos: DOI prioritário; ISBN como alternativa;
  - trabalhos em evento: DOI prioritário; depois ISBN ou ISSN;
  - teses, dissertações, relatórios, documentos, páginas web, datasets e softwares: DOI quando disponível.
- Correção da macro de acesso eletrônico para exibir `Disponível em:` apenas quando houver URL cadastrada.
- Preservação da estrutura autor-data do estilo UFRGS-ABNT.
- Preservação dos créditos dos autores e contribuidores originais no arquivo `.csl`.
- Inclusão da adaptação como versão customizada, com identificador próprio para evitar conflito com o estilo UFRGS original no Mendeley.

---

## 🔗 URL Raw do estilo

O Mendeley Cite pode solicitar uma URL do estilo customizado, em vez de upload manual do arquivo.

Use a URL Raw do GitHub:

```text
https://raw.githubusercontent.com/gislainecosta/abnt-csl-mendeley/main/adaptado-ufrgs-abnt-2025-com-doi-github.csl
```

Essa é a URL direta do arquivo `.csl`.

> **Importante:** não use a URL visual do GitHub no formato `github.com/.../blob/...`, porque ela aponta para a página do arquivo, não para o conteúdo bruto exigido pelo Mendeley Cite.

---

## 🧭 Como obter a URL Raw pelo GitHub

Para copiar a URL correta pelo GitHub:

1. Abra este repositório no GitHub.
2. Clique no arquivo:

```text
adaptado-ufrgs-abnt-2025-com-doi-github.csl
```

3. Com o arquivo aberto, clique em **Raw**.
4. O navegador abrirá o conteúdo bruto do arquivo.
5. Copie a URL da barra de endereço.
6. Cole essa URL no Mendeley Cite quando ele solicitar a URL do estilo customizado.

A URL Raw também pode aparecer neste formato:

```text
https://raw.githubusercontent.com/gislainecosta/abnt-csl-mendeley/refs/heads/main/adaptado-ufrgs-abnt-2025-com-doi-github.csl
```

As duas formas apontam para o arquivo na branch `main`.

---

## ⚙️ Como instalar no Mendeley Cite usando a URL

Para usar este estilo no Mendeley Cite:

1. Abra o Word.
2. Abra o painel do **Mendeley Cite**.
3. Vá em **Citation Settings**.
4. Clique em **Change citation style**.
5. Escolha a opção para adicionar estilo customizado.
6. Cole a URL Raw do arquivo `.csl`:

```text
https://raw.githubusercontent.com/gislainecosta/abnt-csl-mendeley/main/adaptado-ufrgs-abnt-2025-com-doi-github.csl
```

7. Confirme a inclusão do estilo.
8. Após o envio, selecione o estilo:

```text
Adaptado de UFRGS - ABNT 6023:2025 e 10520:2023 com DOI
```

---

## 🔄 Passo importante após instalar ou trocar o estilo

Depois de instalar o estilo customizado ou trocar o estilo de citação no Mendeley Cite, é importante fazer uma atualização geral.

No Mendeley Cite:

1. Vá em **Citation Settings**.
2. Confira se o estilo ativo é:

```text
Adaptado de UFRGS - ABNT 6023:2025 e 10520:2023 com DOI
```

3. Clique no ícone de atualização geral do Mendeley Cite.
4. Se necessário, abra o menu de três pontos e clique em **Update Bibliography**.

Esse passo é importante porque o Word/Mendeley Cite pode manter referências em cache. Em alguns casos, o DOI, ISBN, ISSN ou outros ajustes do estilo só aparecem corretamente depois dessa atualização geral.

Se uma referência específica ainda não atualizar, uma alternativa é apagar a citação daquele item no Word, inserir novamente pelo Mendeley Cite e atualizar a bibliografia.

---

## ✅ Como conferir se o estilo correto foi instalado

Depois de instalar no Mendeley Cite, confira se aparece na lista de estilos o nome:

```text
Adaptado de UFRGS - ABNT 6023:2025 e 10520:2023 com DOI
```

Esse nome vem da tag `<title>` dentro do arquivo `.csl`.

Se aparecer outro nome, ou se o estilo ficar duplicado com o nome da UFRGS, verifique se o arquivo instalado é a versão adaptada e se o `<id>` do arquivo está diferente do estilo UFRGS original.

---

## 🧾 Observações sobre DOI, ISBN e ISSN

Este estilo prioriza o DOI quando ele está disponível, porque o DOI identifica o documento digital específico.

Em termos gerais:

| Identificador | Uso principal |
|---|---|
| **DOI** | Identifica um documento específico, como artigo, capítulo, dataset ou relatório digital. |
| **ISBN** | Identifica livros e publicações monográficas. |
| **ISSN** | Identifica periódicos, revistas, jornais e publicações seriadas. |

Por isso, em artigos científicos, o DOI é priorizado em relação ao ISSN, já que o ISSN identifica a revista como um todo, enquanto o DOI identifica o artigo específico.

---

## 📝 Recomendação de uso

Mesmo utilizando um estilo CSL customizado, recomenda-se revisar as referências finais antes da entrega de trabalhos acadêmicos, especialmente quando houver exigências específicas de programa, orientador, banca ou periódico.

Os gerenciadores de referência dependem do preenchimento correto dos campos bibliográficos. Para melhor resultado, confira se cada item no Mendeley possui, quando aplicável:

- autor;
- ano;
- título;
- periódico ou editora;
- volume;
- número;
- páginas;
- DOI;
- ISBN;
- ISSN;
- URL;
- data de acesso.

Também é importante conferir se não há registros duplicados no Mendeley, porque a citação no Word pode estar vinculada a uma versão antiga ou incompleta do item bibliográfico.

---

## ⚖️ Licença

Este estilo é uma adaptação do estilo UFRGS-ABNT e mantém a licença original **Creative Commons Attribution-ShareAlike 3.0**.

A adaptação preserva os créditos dos autores e contribuidores originais no arquivo `.csl`.

A licença original declarada no arquivo é:

```xml
<rights license="http://creativecommons.org/licenses/by-sa/3.0/">This work is licensed under a Creative Commons Attribution-ShareAlike 3.0 License</rights>
```

Mais informações sobre a licença:

```text
https://creativecommons.org/licenses/by-sa/3.0/
```

---

## 👤 Créditos

Este estilo foi adaptado a partir do modelo UFRGS-ABNT.

Os autores e contribuidores originais foram preservados no arquivo `.csl`.

Adaptação por:

```text
Gislaine Costa Pereira
https://github.com/gislainecosta
```
