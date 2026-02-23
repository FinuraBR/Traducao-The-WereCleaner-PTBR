# 🇧🇷 Tradução Parcial / Open-Source - The WereCleaner (PT-BR)

**Status do Projeto:** ⚠️ Pausado / Incompleto (Jogável)
**Iniciado por:** ツFinuraBR

Este repositório contém todo o meu progresso na tradução do jogo **The WereCleaner** para o Português do Brasil. Decidi publicar os arquivos abertamente no GitHub para que qualquer pessoa possa jogar o que já foi feito ou, caso tenha interesse, assumir o projeto e finalizá-lo.

---

## 📌 Estado Atual da Tradução

- **Está jogável:** Uma boa parte do jogo já está em português.
- **Incompleto e Não Testado:** O jogo não foi 100% traduzido e não passou por testes rigorosos. Podem haver erros de digitação, frases sem sentido ou textos que ainda estão em inglês.
- **Por que parei?** A estrutura de textos deste jogo é muito desorganizada. Os desenvolvedores espalharam os textos por vários arquivos (`level0`, `level1`, etc.) e há **MUITAS repetições** da mesma frase. O progresso estava muito lento e exaustivo.

> **💡 Dica Importante:** A maior parte dos textos vitais do jogo está no arquivo `level0`. Apenas aplicando a tradução desse arquivo, o jogo já ficará bem compreensível. O resto dos arquivos é recomendado aplicar por precaução.

---

## 🛠️ Como Instalar a Tradução (Para Jogadores)

Como a tradução altera os arquivos vitais do jogo, você precisará usar um programa chamado **UABEA** para injetar os textos traduzidos no seu jogo.

### Pré-requisitos
1. Baixe o **UABEA (Unity Assets Bundle Extractor Avalonia)** [AQUI](https://github.com/nesrak1/UABEA) (baixe a versão mais recente para seu sistema operacional).
2. Baixe os arquivos deste repositório clicando no botão verde `Code > Download ZIP`. Extraia a pasta no seu computador.
3. **Faça um backup** da pasta `The WereCleaner_Data` que fica nos arquivos locais do seu jogo!

### Passo a Passo da Instalação

A instalação exige que você abra os arquivos `assets` originais do jogo e importe a minha pasta pronta.

1. Abra o `UABEA.exe` e clique em **File > Open**.
2. Vá até a pasta do seu jogo (`The WereCleaner_Data`) e abra o arquivo correspondente (Ex: `level0`).
3. Com o arquivo aberto, clique na aba superior em **View > Search by Name** (ou pressione `Ctrl+A` para selecionar tudo na lista).
4. No menu lateral direito, clique no botão **Import Dump**.
5. ⚠️ **MUITO IMPORTANTE:** Se o programa perguntar o formato do arquivo, **selecione JSON** (e não TXT). **(apenas o `level0` está em TXT)**
6. O programa vai pedir para você selecionar uma pasta. Escolha a pasta `3_Traduzidos/level0` que você baixou do meu GitHub. O programa vai injetar automaticamente os textos.
7. Vá em **File > Save** (ou `Save All`) e salve por cima do arquivo original.
8. **Repita esse processo** para os outros arquivos (abrindo o `level1` no UABEA e importando os Dumps da pasta `3_Traduzidos/level1`, e assim por diante).

---

## 🤝 Para Futuros Tradutores (Quer continuar o projeto?)

Se você entende de UABEA e quer continuar essa tradução, fique à vontade para fazer um *Fork* deste repositório! Deixei todo o meu "Workspace" organizado e até scripts em Python que usei para agilizar o processo.

### 🗂️ Entendendo a Estrutura do Projeto
- `1_Dump_Temporario/`: Onde eu jogava os dumps brutos exportados do UABEA (muito "lixo" misturado).
- `2_Selecionados/`: Os arquivos que eu filtrei e vi que realmente tinham textos possivelmente úteis para traduzir.
- `3_Traduzidos/`: Os arquivos finais em português (já no formato JSON), separados por pastas com o nome dos assets originais (ex: `level0`, `level1`). É daqui que o UABEA puxa a tradução.
- `4_Versão_Final/`: Arquivos finalizados/prontos **(não finalizado)**.
- `limpar_arquivos.py` / `traduzir_tudo.py`: Scripts em Python que criei para me ajudar a limpar o código inútil dos dumps e automatizar parte do trabalho. Sinta-se livre para usá-los!

### 💡 Dica de Ouro para quem for continuar:
Para economizar muito tempo, saiba que **todos os textos do jogo estão no formato `MonoBehaviour`**.
Quando você for extrair coisas novas do jogo no UABEA, não exporte tudo. Filtre a lista pela coluna `Type`, selecione apenas os arquivos `MonoBehaviour` e dê Export Dump. Isso vai te poupar horas de trabalho analisando arquivos inúteis.

E lembre-se: prepare-se para ver muita repetição de texto. A organização nativa do jogo é bem caótica.

### 📜 Licença e Créditos
Este projeto é de código aberto para a comunidade. A única exigência caso você continue o projeto, publique atualizações ou crie um instalador automático no futuro é **manter o meu nome nos créditos como criador original da base da tradução**.

**Créditos Iniciais:** ツFinuraBR
