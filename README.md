# 📚 Adaptado de UFRGS - ABNT 6023:2025 e 10520:2023 com DOI

Este repositório contém um estilo CSL customizado para uso no **Mendeley Cite**, adaptado a partir do estilo **UFRGS-ABNT**.

O objetivo desta adaptação é preservar a estrutura geral do estilo UFRGS-ABNT e acrescentar ajustes voltados ao uso acadêmico conforme a **ABNT NBR 6023:2025**, para referências, e a **ABNT NBR 10520:2023**, para citações.

---

## 📑 Sumário

- [📄 Arquivos CSL e compatibilidade](#-arquivos-csl-e-compatibilidade)
- [✨ Principais adaptações](#-principais-adaptações)
- [📐 Formatação da bibliografia](#-formatação-da-bibliografia)
- [🔗 URL Raw do estilo principal](#-url-raw-do-estilo-principal)
- [⚙️ Instalação no Mendeley Cite](#️-instalação-no-mendeley-cite)
- [🔄 Atualização do estilo no documento](#-atualização-do-estilo-no-documento)
- [🧾 DOI, ISBN e ISSN](#-doi-isbn-e-issn)
- [⚠️ Limitação conhecida: *et al.* em citações textuais](#️-limitação-conhecida-et-al-em-citações-textuais)
- [📝 Recomendação de uso](#-recomendação-de-uso)
- [⚖️ Licença](#️-licença)
- [👤 Créditos](#-créditos)

---

## 📄 Arquivos CSL e compatibilidade

O **arquivo principal e canônico** para novas instalações é:

```text
abnt-adaptado-ufrgs-6023-2025-10520-2023-doi.csl
```

Este é o arquivo que deve receber as novas correções e evoluções do estilo.

O repositório também mantém o arquivo:

```text
adaptado-ufrgs-abnt-2025-com-doi-github.csl
```

Esse segundo arquivo existe por **compatibilidade com documentos antigos**. Versões anteriores do estilo usaram essa URL, e o Mendeley Cite pode armazenar no próprio documento do Word o endereço exato do arquivo CSL. Se o arquivo antigo deixar de existir no GitHub, documentos já vinculados a ele podem deixar de carregar o estilo corretamente.

> **Não excluir o arquivo legado.** Ele deve permanecer disponível para preservar a compatibilidade com documentos que já registraram a URL antiga.

Para novos documentos, use sempre o arquivo canônico `abnt-adaptado-ufrgs-6023-2025-10520-2023-doi.csl`.

### Resumo

| Arquivo | Função | Uso recomendado |
|---|---|---|
| `abnt-adaptado-ufrgs-6023-2025-10520-2023-doi.csl` | Arquivo principal/canônico | Novas instalações e futuras atualizações |
| `adaptado-ufrgs-abnt-2025-com-doi-github.csl` | Arquivo legado de compatibilidade | Documentos antigos que já armazenaram essa URL |

---

## ✨ Principais adaptações

- Inclusão de DOI nas referências.
- Priorização do DOI quando disponível.
- Tratamento de ISBN e ISSN conforme o tipo documental.
- Prioridade de identificadores por tipo de documento:
  - artigos: DOI prioritário;
  - livros: DOI prioritário, com ISBN como alternativa;
  - capítulos: DOI prioritário, com ISBN como alternativa;
  - trabalhos em evento: DOI prioritário, depois ISBN ou ISSN;
  - teses, dissertações, relatórios, documentos, páginas web, datasets e softwares: DOI quando disponível.
- Supressão de URL e data de acesso em artigos que possuem DOI.
- Exibição de `Disponível em:` apenas quando há URL cadastrada e aplicável ao tipo documental.
- Preservação da estrutura autor-data do estilo UFRGS-ABNT.
- Preservação dos créditos dos autores e contribuidores originais.
- Identificador próprio para evitar conflito com o estilo UFRGS original no Mendeley.

---

## 📐 Formatação da bibliografia

O bloco `<bibliography>` controla parte da apresentação da lista de referências.

Para referências com **espaçamento simples entre linhas e sem uma linha em branco entre entradas**, o estilo canônico deve usar:

```xml
<bibliography et-al-min="4" et-al-use-first="1" line-spacing="1" entry-spacing="0">
```

- `line-spacing="1"` define espaçamento simples dentro de cada referência.
- `entry-spacing="0"` remove a linha adicional entre uma referência e outra.

### Espaçamento de parágrafo de 6 pt

A configuração desejada para documentos acadêmicos deste projeto é:

- **Antes:** 0 pt
- **Depois:** 6 pt
- **Entrelinhas:** simples

O CSL atual permite controlar `line-spacing` e `entry-spacing`, mas o padrão CSL define `entry-spacing` como um número inteiro de alturas de linha. Por isso, o CSL válido não possui um atributo próprio para declarar exatamente `6 pt` após cada parágrafo.

No Word, aplique o espaçamento de **0 pt antes e 6 pt depois** ao parágrafo da bibliografia. O arquivo CSL permanece responsável pelo espaçamento simples e pela ausência de uma linha em branco adicional.

> Algumas implementações antigas aceitaram valores fracionários, como `entry-spacing="0.5"`, mas esse valor não atende ao esquema CSL atual. O arquivo canônico evita essa solução para preservar a validade e a compatibilidade do estilo.

---

## 🔗 URL Raw do estilo principal

Use esta URL para novas instalações:

```text
https://raw.githubusercontent.com/gislainecosta/abnt-csl-mendeley/refs/heads/main/abnt-adaptado-ufrgs-6023-2025-10520-2023-doi.csl
```

Essa é a URL direta do arquivo `.csl`.

> **Importante:** não use a URL visual do GitHub no formato `github.com/.../blob/...`, pois ela aponta para a página do arquivo, e não para o conteúdo bruto que o Mendeley Cite precisa acessar.

A URL antiga permanece disponível apenas para compatibilidade:

```text
https://raw.githubusercontent.com/gislainecosta/abnt-csl-mendeley/refs/heads/main/adaptado-ufrgs-abnt-2025-com-doi-github.csl
```

---

## ⚙️ Instalação no Mendeley Cite

1. Abra o Word.
2. Abra o painel do **Mendeley Cite**.
3. Acesse **Citation Settings**.
4. Clique em **Change citation style**.
5. Escolha a opção para adicionar um estilo customizado.
6. Cole a URL Raw do arquivo canônico:

```text
https://raw.githubusercontent.com/gislainecosta/abnt-csl-mendeley/refs/heads/main/abnt-adaptado-ufrgs-6023-2025-10520-2023-doi.csl
```

7. Confirme a inclusão.
8. Selecione o estilo correspondente na lista do Mendeley Cite.

---

## 🔄 Atualização do estilo no documento

Após uma alteração no CSL:

1. Confirme se o documento usa a URL e o estilo desejados.
2. Use o comando de atualização do Mendeley Cite.
3. Atualize a bibliografia.
4. Confira novamente as referências no Word.

O Mendeley Cite pode preservar dados do estilo no próprio arquivo `.docx`. Por esse motivo, a exclusão ou a troca de uma URL antiga pode afetar documentos existentes, mesmo que uma nova versão do CSL já esteja disponível no GitHub.

Se uma referência específica não refletir uma correção feita no cadastro do Mendeley, apague apenas essa citação, insira-a novamente pelo Mendeley Cite e atualize a bibliografia.

---

## 🧾 DOI, ISBN e ISSN

Este estilo prioriza o DOI quando ele está disponível, pois o DOI identifica o documento digital específico.

| Identificador | Uso principal |
|---|---|
| **DOI** | Documento específico, como artigo, capítulo, dataset ou relatório digital |
| **ISBN** | Livros e publicações monográficas |
| **ISSN** | Periódicos, revistas, jornais e publicações seriadas |

Em artigos científicos, o DOI tem prioridade sobre o ISSN, pois o ISSN identifica o periódico como um todo, enquanto o DOI identifica o artigo específico.

---

## ⚠️ Limitação conhecida: *et al.* em citações textuais

### O problema

O estilo aplica itálico ao elemento `<et-al>`. Nas citações parentéticas, o Mendeley respeita essa formatação, por exemplo:

> (Li *et al.*, 2019; Norton *et al.*, 2019)

Em citações textuais, o Mendeley Cite pode ignorar o itálico:

> Segundo Wang et al. (2024), ...

Essa limitação ocorre no processador do Mendeley Cite e não decorre da regra escrita no CSL.

### Correção no Word desktop

O arquivo `Macro.txt` deste repositório contém uma macro VBA que aplica itálico às ocorrências de `et al.` no documento.

Para executar:

1. Abra o Word desktop.
2. Pressione `Alt + F11` e adicione a macro ao modelo desejado.
3. Pressione `Alt + F8`.
4. Selecione `ItalicizarEtAl`.
5. Clique em **Executar**.

Use a macro após a conclusão das citações e antes da entrega final do documento.

### Word para a web

O Word para a web não executa macros VBA. Nesse caso, abra o arquivo no Word desktop para aplicar a macro ou faça a correção manual no documento final.

---

## 📝 Recomendação de uso

Mesmo com um estilo CSL customizado, revise a bibliografia antes da entrega do trabalho. O resultado depende tanto das regras do CSL quanto do preenchimento correto dos metadados no Mendeley.

Confira, quando aplicável:

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

Também confira registros duplicados, pois uma citação do Word pode estar vinculada a uma versão antiga ou incompleta de um item bibliográfico.

---

## ⚖️ Licença

Este estilo é uma adaptação do estilo UFRGS-ABNT e preserva a licença original **Creative Commons Attribution-ShareAlike 3.0**.

```xml
<rights license="http://creativecommons.org/licenses/by-sa/3.0/">This work is licensed under a Creative Commons Attribution-ShareAlike 3.0 License</rights>
```

Mais informações:

```text
https://creativecommons.org/licenses/by-sa/3.0/
```

---

## 👤 Créditos

Este estilo foi adaptado a partir do modelo UFRGS-ABNT. Os autores e contribuidores originais permanecem registrados no arquivo `.csl`.

Adaptação por:

```text
Gislaine Costa Pereira
https://github.com/gislainecosta
```
