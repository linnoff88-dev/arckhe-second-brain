ï»¿<div align="center">

<img src="banner.svg" alt="Second Brain" width="800"/>

**Uma IA que jêÂ¡ sabe quem vocêÂª êÂ© antes de vocêÂª digitar uma palavra.**

![macOS](https://img.shields.io/badge/macOS-ê¢Åâ-8A2BE2?style=flat-square) ![Windows](https://img.shields.io/badge/Windows-ê¢Åâ-8A2BE2?style=flat-square) ![Linux](https://img.shields.io/badge/Linux-ê¢Åâ-8A2BE2?style=flat-square) ![Free](https://img.shields.io/badge/custo-grêÂ¡tis-8A2BE2?style=flat-square) ![One command](https://img.shields.io/badge/setup-um_comando-8A2BE2?style=flat-square)

[Obsidian](https://obsidian.md) + [Claude Code](https://claude.ai/code) êÂ· Local êÂ· Privado êÂ· Um comando

```
  Seus arquivos (PDFs, docs, notas)
          ê¢ââ
          ê¢âÂ¼
  ê¢âÅê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢âÂ
  ê¢ââ   Obsidian vault  ê¢ââ  ê¢â Â arquivos .md no seu computador
  ê¢ââ  inbox/  daily/   ê¢ââ
  ê¢ââ  projects/  ...   ê¢ââ
  ê¢ââê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢âÂ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢âË
           ê¢ââ  Claude Code lêÂª esta pasta
           ê¢âÂ¼
  ê¢âÅê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢âÂ
  ê¢ââ   Claude Code     ê¢ââ  ê¢â Â conhece seus projetos, voz, contexto
  ê¢ââ   /vault-setup    ê¢ââ     antes de vocêÂª digitar uma palavra
  ê¢ââ   /daily  /tldr   ê¢ââ
  ê¢ââê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢ââ¬ê¢âË
           ê¢ââ
           ê¢âÂ¼
    IA que se acumula.
    SessêÂ£o 1: conhece suas pastas.
    SessêÂ£o 20: sabe mais sobre
    seu trabalho do que vocêÂª lembra conscientemente.
```

*Se isso te economizou horas, deixe uma ê¢Â­Â ê¢â¬â ajuda outros a encontrar.*

</div>

---

## InêÂ­cio RêÂ¡pido

### macOS

**OpêÂ§êÂ£o A ê¢â¬â Uma linha** (cole no Terminal e pressione Enter):

```bash
curl -fsSL https://raw.githubusercontent.com/earlyaidopters/second-brain/main/setup.sh -o setup.sh && bash setup.sh
```

**OpêÂ§êÂ£o B ê¢â¬â Clonar o repo:**

Abra o **Terminal** (pressione `ê¢ÅË Space`, digite `Terminal`, Enter) e rode:

```bash
git clone https://github.com/earlyaidopters/second-brain.git
cd second-brain
./setup.sh
```

> **NêÂ£o tem git?** Rode `xcode-select --install` primeiro e tente novamente.

---

### Linux

**OpêÂ§êÂ£o A ê¢â¬â Uma linha:**

```bash
curl -fsSL https://raw.githubusercontent.com/earlyaidopters/second-brain/main/setup.sh -o setup.sh && bash setup.sh
```

**OpêÂ§êÂ£o B ê¢â¬â Clonar o repo:**

```bash
git clone https://github.com/earlyaidopters/second-brain.git
cd second-brain
./setup.sh
```

> **PrêÂ©-requisitos:** `git`, `python3` e `pip` devem estar instalados. Na maioria das distros jêÂ¡ vêÂªm por padrêÂ£o. Se nêÂ£o:
> ```bash
> # Ubuntu/Debian
> sudo apt install git python3 python3-pip python3-venv
>
> # Fedora
> sudo dnf install git python3 python3-pip
>
> # Arch
> sudo pacman -S git python python-pip
> ```

> **Obsidian no Linux** ê¢â¬â o script instala automaticamente via Snap, Flatpak ou AppImage. Se preferir instalar manualmente:
> ```bash
> # Snap
> sudo snap install obsidian --classic
>
> # Flatpak
> flatpak install flathub md.obsidian.Obsidian
>
> # AppImage ê¢â¬â baixe em https://obsidian.md/download
> chmod +x Obsidian-*.AppImage && ./Obsidian-*.AppImage
> ```

---

### Windows

> **Primeiro: vocêÂª tem git?**
> Abra o **PowerShell** (pressione `Win`, digite `powershell`, Enter) e rode:
> ```powershell
> git --version
> ```
> Se aparecer um nêÂºmero de versêÂ£o, estêÂ¡ ok. SenêÂ£o, instale pelo [git-scm.com](https://git-scm.com/download/win) ê¢â¬â use todas as opêÂ§êÂµes padrêÂ£o e reabra o PowerShell.

**OpêÂ§êÂ£o A ê¢â¬â Uma linha** (cole no PowerShell e pressione Enter):

```powershell
Invoke-WebRequest -Uri "https://raw.githubusercontent.com/earlyaidopters/second-brain/main/setup.ps1" -OutFile setup.ps1; powershell -ExecutionPolicy Bypass -File setup.ps1
```

**OpêÂ§êÂ£o B ê¢â¬â Clonar o repo:**

```powershell
git clone https://github.com/earlyaidopters/second-brain.git
cd second-brain
powershell -ExecutionPolicy Bypass -File setup.ps1
```

> **Erro "execuêÂ§êÂ£o de scripts desabilitada"?** êâ° uma configuraêÂ§êÂ£o de seguranêÂ§a do Windows. O `-ExecutionPolicy Bypass` no comando acima ignora isso apenas para este script ê¢â¬â nêÂ£o muda nada permanente no seu computador.

> **Python nêÂ£o encontrado?** Baixe em [python.org/downloads](https://python.org/downloads) ê¢â¬â na primeira tela do instalador, marque **"Add Python to PATH"** antes de clicar em Install. Depois rode o script de setup novamente.

---

O script cuida do resto: instala Obsidian, instala Claude Code, cria seu vault e opcionalmente importa seus arquivos existentes.

---

## Por que Isso Existe

VocêÂª jêÂ¡ tentou criar um segundo cêÂ©rebro antes.

Talvez Notion. Talvez Apple Notes. Talvez uma pasta de arquivos markdown que vocêÂª jurou que ia organizar.

Toda vez, o mesmo resultado: vocêÂª configurava, usava por uma semana, e depois esquecia completamente que existia.

O problema nunca foi a ferramenta. **Era que vocêÂª precisava lembrar de usêÂ¡-la.**

Isto conecta o **Obsidian** (seu vault local de conhecimento) ao **Claude Code** (seu agente de IA) para que:

- Claude Code **leia suas notas** antes de responder ê¢â¬â ele conhece seus projetos, seus clientes, sua voz
- Claude Code **escreva suas notas** depois de trabalhar ê¢â¬â seu vault se constrêÂ³i sozinho a partir das sessêÂµes
- Seus arquivos existentes (PDFs, docs, slides) sêÂ£o **sintetizados e importados automaticamente** via Gemini 3 Flash
- Tudo fica **local, privado e seu** ê¢â¬â sem lock-in de nuvem, sem assinaturas crescentes

O resultado: uma IA que sabe quem vocêÂª êÂ© desde o primeiro prompt de cada sessêÂ£o. NêÂ£o porque vocêÂª contou. Porque ela leu seu vault.

---

## O que êÂ© Instalado

| Ferramenta | O que êÂ© | Para quêÂª |
|------------|---------|----------|
| **Obsidian** | App gratuito de notas | Suas notas vivem como arquivos `.md` no seu computador ê¢â¬â sem nuvem, sem assinatura, seus para sempre |
| **Claude Code** | Terminal IA da Anthropic | LêÂª e escreve arquivos diretamente no seu vault ê¢â¬â sem copiar/colar, sem trocar de aba |
| **Pacotes Python** | Bibliotecas de fundo | Usadas pelo Gemini 3 Flash para ler e sintetizar seus arquivos existentes (PDFs, docs, slides) |
| **Vault skills** | Slash commands | `/vault-setup` `/daily` `/tldr` `/file-intel` ê¢â¬â ensinam o Claude a trabalhar com seu vault |
| **Obsidian Skills** *(opcional)* | Skills oficiais do [Kepano](https://github.com/kepano) (CEO do Obsidian) | Permite ao Claude navegar, ler e escrever seu vault nativamente usando a CLI do Obsidian |

> **Nada êÂ© enviado para servidores.** Seu vault êÂ© uma pasta no seu computador. Claude Code lêÂª localmente. A êÂºnica chamada de rede opcional êÂ© o processamento via Gemini ê¢â¬â e êÂ© totalmente pulêÂ¡vel.

---

## O que o Script de Setup Faz

```
Passo 1 ê¢â¬â Verificar dependêÂªncias       (Homebrew no Mac / winget no Windows / apt/dnf/pacman no Linux)
Passo 2 ê¢â¬â Instalar Obsidian            (app gratuito de notas local)
Passo 3 ê¢â¬â Instalar Claude Code CLI     (terminal IA da Anthropic)
Passo 4 ê¢â¬â Instalar pacotes Python      (para processamento de arquivos via Gemini)
Passo 5 ê¢â¬â Criar seu vault              (inbox, daily, projects, research, archive + skills)
Passo 6 ê¢â¬â Importar arquivos existentes (opcional ê¢â¬â Gemini lêÂª e sintetiza)
Passo 7 ê¢â¬â Obsidian Skills              (opcional ê¢â¬â skills oficiais do Kepano, CEO do Obsidian)
           ê¢ââê¢ââ¬> Abre o Obsidian apontando para seu novo vault
```

---

## Depois do Setup

### 1. Habilitar a CLI do Obsidian
```
Obsidian ê¢â â Settings ê¢â â General ê¢â â Enable Command Line Interface
```
Isso adiciona o comando `obsidian` ao seu PATH para abrir o vault pelo terminal. ([Docs da CLI](https://help.obsidian.md/cli))

### 2. Abrir o Claude Code no seu vault
```bash
cd ~/second-brain
claude
```

### 3. Rodar seu primeiro comando
```
/vault-setup
```

O Claude Code vai te entrevistar sobre seu papel e trabalho, depois gerar um `CLAUDE.md` personalizado e sugerir slash commands para seu fluxo de trabalho especêÂ­fico. Um empresêÂ¡rio recebe pastas diferentes de um desenvolvedor. Um criador de conteêÂºdo recebe comandos diferentes de um consultor.

---

## Slash Commands

Quatro comandos vêÂªm prêÂ©-instalados. Mais sêÂ£o adicionados conforme vocêÂª usa o sistema.

| Comando | O que faz |
|---------|-----------|
| `/vault-setup` | Te entrevista (papel, projetos, objetivos) e gera estrutura personalizada do vault + CLAUDE.md + slash commands customizados |
| `/daily` | ComeêÂ§a seu dia ê¢â¬â lêÂª a nota de hoje ou cria uma, mostra prioridades, pergunta no que vocêÂª estêÂ¡ trabalhando |
| `/tldr` | No final de qualquer sessêÂ£o, salva um resumo estruturado na pasta certa do vault automaticamente |
| `/file-intel` | Aponte para qualquer pasta ê¢â¬â Gemini lêÂª cada arquivo e gera resumos prontos para Obsidian no seu inbox |

> **Importante:** Slash commands sêÂ³ ativam quando o Claude Code êÂ© aberto de dentro da pasta do vault. Sempre faêÂ§a `cd` para o vault antes de rodar `claude`.
>
> ```bash
> cd ~/second-brain              # Mac / Linux
> cd $env:USERPROFILE\second-brain   # Windows
> claude
> ```
>
> **Quer que funcionem em qualquer lugar?** Dentro do Claude Code, peêÂ§a:
> *"FaêÂ§a esses slash commands globais para funcionarem em qualquer pasta"*
> O Claude Code vai copiar os skills para `~/.claude/skills/`.

---

## Importando Arquivos Existentes

Tem anos de PDFs, documentos Word e apresentaêÂ§êÂµes guardados em pastas? NêÂ£o converta manualmente.

```bash
python3 scripts/process_docs_to_obsidian.py ~/seus-arquivos ~/second-brain/inbox
```

**O que acontece:**
1. Cada arquivo êÂ© lido pelo **Gemini 3 Flash** (`gemini-3-flash-preview`)
2. O sinal êÂ© extraêÂ­do, o ruêÂ­do êÂ© descartado (boilerplate jurêÂ­dico, cabeêÂ§alhos, enchimento)
3. Uma nota Markdown limpa e compacta êÂ© salva no seu `inbox/` (300ê¢â¬â600 palavras mêÂ¡x.)

Depois abra o Claude Code e diga: *"Organize tudo no inbox/ nas pastas certas."*

Ele lêÂª seu CLAUDE.md, entende a estrutura do vault e encaminha cada nota para onde pertence.

**Formatos suportados:** `.pdf` `.docx` `.pptx` `.txt` `.md`

> **Tem arquivos Excel, CSV ou JSON tambêÂ©m?** Use o script mais abrangente:
> ```bash
> python3 scripts/process_files_with_gemini.py ~/seus-arquivos
> ```
> Ele processa `.xlsx` `.csv` `.json` `.xml` `.py` `.js` `.html` e a maioria dos arquivos baseados em texto. Resultados ficam em `outputs/file_summaries/` com um `MASTER_SUMMARY.md` resumindo tudo.

---

## Como a MemêÂ³ria Funciona

Seu vault êÂ© estruturado para que o Claude Code encontre o contexto certo para qualquer tarefa:

```
~/second-brain/
ê¢âÅê¢ââ¬ê¢ââ¬ CLAUDE.md        ê¢â Â O cêÂ©rebro do cêÂ©rebro. Lido no inêÂ­cio de cada sessêÂ£o.
ê¢âÅê¢ââ¬ê¢ââ¬ memory.md        ê¢â Â Log de sessêÂµes. Atualizado pelo Claude Code apêÂ³s cada conversa.
ê¢âÅê¢ââ¬ê¢ââ¬ inbox/           ê¢â Â Zona de entrada. Qualquer coisa nova cai aqui primeiro.
ê¢âÅê¢ââ¬ê¢ââ¬ daily/           ê¢â Â Notas diêÂ¡rias (YYYY-MM-DD.md). Seu log contêÂ­nuo.
ê¢âÅê¢ââ¬ê¢ââ¬ projects/        ê¢â Â Projetos ativos. Claude lêÂª o relevante antes de ajudar.
ê¢âÅê¢ââ¬ê¢ââ¬ research/        ê¢â Â Conhecimento sintetizado. Fontes, notas, ideias.
ê¢ââê¢ââ¬ê¢ââ¬ archive/         ê¢â Â Trabalho concluêÂ­do. Nunca delete ê¢â¬â apenas archive.
```

**O efeito composto:**
- SessêÂ£o 1: Claude conhece a estrutura das suas pastas
- SessêÂ£o 5: Claude conhece seus projetos, sua voz, suas preferêÂªncias
- SessêÂ£o 20: Claude êÂ© seu sistema operacional personalizado ê¢â¬â sabe mais sobre sua base de conhecimento do que vocêÂª lembra conscientemente

> **Nota:** A atualizaêÂ§êÂ£o da memêÂ³ria **nêÂ£o êÂ© automêÂ¡tica**. VocêÂª precisa rodar `/tldr` no final de cada sessêÂ£o para salvar o resumo, e `/daily` no inêÂ­cio do dia para carregar o contexto. Os arquivos nêÂ£o se atualizam sozinhos em background.

---

## Requisitos

| Ferramenta | Plataforma | Como obter |
|------------|-----------|------------|
| Obsidian | macOS | `brew install --cask obsidian` |
| Obsidian | Windows | `winget install Obsidian.Obsidian` |
| Obsidian | Linux | `snap install obsidian --classic` ou `flatpak install flathub md.obsidian.Obsidian` ou [AppImage](https://obsidian.md/download) |
| Claude Code | macOS / Linux | `curl -fsSL https://claude.ai/install.sh \| sh` |
| Claude Code | Windows | `winget install Anthropic.ClaudeCode` |
| Python 3.8+ | Todas | [python.org](https://python.org) |
| Chave API Google | Todas | [aistudio.google.com/apikey](https://aistudio.google.com/apikey) ê¢â¬â grêÂ¡tis |
| Conta Claude | Todas | [claude.ai](https://claude.ai) ê¢â¬â Pro recomendado para uso intenso |

---

## Estrutura do RepositêÂ³rio

```
second-brain/
ê¢âÅê¢ââ¬ê¢ââ¬ setup.sh                              ê¢â Â Setup macOS/Linux (um comando)
ê¢âÅê¢ââ¬ê¢ââ¬ setup.ps1                             ê¢â Â Setup Windows (um comando)
ê¢âÅê¢ââ¬ê¢ââ¬ CLAUDE.md                             ê¢â Â Arquivo de sistema do vault (personalizado pelo /vault-setup)
ê¢âÅê¢ââ¬ê¢ââ¬ memory.md                             ê¢â Â MemêÂ³ria de sessêÂ£o (atualizado pelo Claude Code)
ê¢âÅê¢ââ¬ê¢ââ¬ requirements.txt                      ê¢â Â DependêÂªncias Python
ê¢âÅê¢ââ¬ê¢ââ¬ .env.example                          ê¢â Â Copie para .env, adicione sua chave API Google
ê¢âÅê¢ââ¬ê¢ââ¬ .gitignore                            ê¢â Â MantêÂ©m .env e .venv fora do git
ê¢âÅê¢ââ¬ê¢ââ¬ scripts/
ê¢ââ   ê¢âÅê¢ââ¬ê¢ââ¬ process_docs_to_obsidian.py      ê¢â Â Sintetizador de arquivos via Gemini 3 Flash
ê¢ââ   ê¢ââê¢ââ¬ê¢ââ¬ process_files_with_gemini.py     ê¢â Â Processador batch Gemini
ê¢âÅê¢ââ¬ê¢ââ¬ skills/
ê¢ââ   ê¢âÅê¢ââ¬ê¢ââ¬ vault-setup/SKILL.md             ê¢â Â Configurador interativo do vault
ê¢ââ   ê¢âÅê¢ââ¬ê¢ââ¬ daily/SKILL.md                   ê¢â Â Comando de standup diêÂ¡rio
ê¢ââ   ê¢âÅê¢ââ¬ê¢ââ¬ tldr/SKILL.md                    ê¢â Â Comando de resumo de sessêÂ£o
ê¢ââ   ê¢ââê¢ââ¬ê¢ââ¬ file-intel/SKILL.md              ê¢â Â Processar qualquer pasta via Gemini
ê¢ââê¢ââ¬ê¢ââ¬ vault-template/
    ê¢âÅê¢ââ¬ê¢ââ¬ inbox/   daily/   projects/
    ê¢âÅê¢ââ¬ê¢ââ¬ research/   archive/
```

---

## Setup Manual

<details>
<summary>Prefere instalar cada peêÂ§a manualmente? Clique para expandir o passo a passo completo para todas as plataformas.</summary>

---

### macOS ê¢â¬â Passos Manuais

**1. Instalar Homebrew** (instalador de apps do macOS ê¢â¬â pule se jêÂ¡ tem)
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

**2. Instalar Obsidian**
```bash
brew install --cask obsidian
```

**3. Instalar Claude Code**
```bash
curl -fsSL https://claude.ai/install.sh | sh
```

**4. Baixar e configurar o vault**
```bash
git clone https://github.com/earlyaidopters/second-brain.git
mkdir -p ~/second-brain/{inbox,daily,projects,research,archive,.claude/skills/vault-setup,.claude/skills/daily,.claude/skills/tldr,.claude/skills/file-intel,scripts}
cp second-brain/CLAUDE.md second-brain/memory.md ~/second-brain/
cp second-brain/skills/vault-setup/SKILL.md ~/second-brain/.claude/skills/vault-setup/
cp second-brain/skills/daily/SKILL.md ~/second-brain/.claude/skills/daily/
cp second-brain/skills/tldr/SKILL.md ~/second-brain/.claude/skills/tldr/
cp second-brain/skills/file-intel/SKILL.md ~/second-brain/.claude/skills/file-intel/
cp second-brain/scripts/* ~/second-brain/scripts/
cp second-brain/.env.example ~/second-brain/.env
```

**5. Adicionar sua chave API Google**

Abra `~/second-brain/.env` em qualquer editor e substitua `your_key_here` pela sua chave de [aistudio.google.com/apikey](https://aistudio.google.com/apikey).

**6. (Opcional) Instalar Obsidian Skills do Kepano**
```bash
git clone --depth=1 https://github.com/kepano/obsidian-skills.git /tmp/obs-skills
for d in /tmp/obs-skills/skills/*/; do
  name=$(basename "$d")
  mkdir -p ~/second-brain/.claude/skills/$name
  cp "$d/SKILL.md" ~/second-brain/.claude/skills/$name/
done
rm -rf /tmp/obs-skills
```

**7. Abrir Claude Code no vault**
```bash
cd ~/second-brain && claude
```

---

### Linux ê¢â¬â Passos Manuais

**1. Instalar dependêÂªncias**
```bash
# Ubuntu/Debian
sudo apt update && sudo apt install -y git python3 python3-pip python3-venv curl

# Fedora
sudo dnf install -y git python3 python3-pip curl

# Arch
sudo pacman -S --noconfirm git python python-pip curl
```

**2. Instalar Obsidian**
```bash
# OpêÂ§êÂ£o 1: Snap (Ubuntu e derivados)
sudo snap install obsidian --classic

# OpêÂ§êÂ£o 2: Flatpak
flatpak install flathub md.obsidian.Obsidian

# OpêÂ§êÂ£o 3: AppImage
# Baixe o .AppImage em https://obsidian.md/download
chmod +x Obsidian-*.AppImage
./Obsidian-*.AppImage
```

**3. Instalar Claude Code**
```bash
curl -fsSL https://claude.ai/install.sh | sh
```

**4. Baixar e configurar o vault**
```bash
git clone https://github.com/earlyaidopters/second-brain.git
mkdir -p ~/second-brain/{inbox,daily,projects,research,archive,.claude/skills/vault-setup,.claude/skills/daily,.claude/skills/tldr,.claude/skills/file-intel,scripts}
cp second-brain/CLAUDE.md second-brain/memory.md ~/second-brain/
cp second-brain/skills/vault-setup/SKILL.md ~/second-brain/.claude/skills/vault-setup/
cp second-brain/skills/daily/SKILL.md ~/second-brain/.claude/skills/daily/
cp second-brain/skills/tldr/SKILL.md ~/second-brain/.claude/skills/tldr/
cp second-brain/skills/file-intel/SKILL.md ~/second-brain/.claude/skills/file-intel/
cp second-brain/scripts/* ~/second-brain/scripts/
cp second-brain/.env.example ~/second-brain/.env
```

**5. Instalar dependêÂªncias Python**
```bash
python3 -m venv ~/.second-brain-venv
~/.second-brain-venv/bin/pip install -r second-brain/requirements.txt
```

**6. Adicionar sua chave API Google**

Abra `~/second-brain/.env` em qualquer editor e substitua `your_key_here` pela sua chave de [aistudio.google.com/apikey](https://aistudio.google.com/apikey).

**7. (Opcional) Instalar Obsidian Skills do Kepano**
```bash
git clone --depth=1 https://github.com/kepano/obsidian-skills.git /tmp/obs-skills
for d in /tmp/obs-skills/skills/*/; do
  name=$(basename "$d")
  mkdir -p ~/second-brain/.claude/skills/$name
  cp "$d/SKILL.md" ~/second-brain/.claude/skills/$name/
done
rm -rf /tmp/obs-skills
```

**8. Abrir Claude Code no vault**
```bash
cd ~/second-brain && claude
```

---

### Windows ê¢â¬â Passos Manuais

Abra o **PowerShell** para todos os comandos abaixo.

**1. Instalar Obsidian**
```powershell
winget install Obsidian.Obsidian
```

**2. Instalar Claude Code**
```powershell
winget install Anthropic.ClaudeCode
```
Feche e reabra o PowerShell apêÂ³s este passo.

**3. Instalar Python** (se nêÂ£o tem)

Baixe de [python.org/downloads](https://python.org/downloads). Na primeira tela do instalador, marque **"Add Python to PATH"** antes de clicar em Install.

**4. Baixar e configurar o vault**
```powershell
git clone https://github.com/earlyaidopters/second-brain.git
$vault = "$env:USERPROFILE\second-brain"
New-Item -ItemType Directory -Force -Path "$vault\inbox","$vault\daily","$vault\projects","$vault\research","$vault\archive","$vault\scripts","$vault\.claude\skills\vault-setup","$vault\.claude\skills\daily","$vault\.claude\skills\tldr","$vault\.claude\skills\file-intel" | Out-Null
Copy-Item "second-brain\CLAUDE.md","second-brain\memory.md" $vault
Copy-Item "second-brain\skills\vault-setup\SKILL.md" "$vault\.claude\skills\vault-setup\"
Copy-Item "second-brain\skills\daily\SKILL.md" "$vault\.claude\skills\daily\"
Copy-Item "second-brain\skills\tldr\SKILL.md" "$vault\.claude\skills\tldr\"
Copy-Item "second-brain\skills\file-intel\SKILL.md" "$vault\.claude\skills\file-intel\"
Copy-Item "second-brain\scripts\*" "$vault\scripts\"
Copy-Item "second-brain\.env.example" "$vault\.env"
```

**5. Instalar dependêÂªncias Python**
```powershell
pip install -r second-brain\requirements.txt
```

**6. Adicionar sua chave API Google**

Abra `%USERPROFILE%\second-brain\.env` no Bloco de Notas e substitua `your_key_here` pela sua chave de [aistudio.google.com/apikey](https://aistudio.google.com/apikey).

**7. (Opcional) Instalar Obsidian Skills do Kepano**
```powershell
$tmp = "$env:TEMP\obs-skills"
git clone --depth=1 https://github.com/kepano/obsidian-skills.git $tmp
Get-ChildItem "$tmp\skills" -Directory | ForEach-Object {
    $dest = "$env:USERPROFILE\second-brain\.claude\skills\$($_.Name)"
    New-Item -ItemType Directory -Force -Path $dest | Out-Null
    Copy-Item "$($_.FullName)\SKILL.md" "$dest\" -Force
}
Remove-Item $tmp -Recurse -Force
```

**8. Abrir Claude Code no vault**
```powershell
cd "$env:USERPROFILE\second-brain"
claude
```

</details>

---

## Perguntas Frequentes

**Meus dados sêÂ£o privados?**
Sim. O Obsidian armazena tudo como arquivos markdown locais no seu computador. Nada êÂ© enviado para nenhum servidor. O Claude Code processa seus arquivos localmente na pasta onde vocêÂª o abre. A êÂºnica vez que algo sai da sua mêÂ¡quina êÂ© quando vocêÂª chama a API do Gemini para processar arquivos existentes ê¢â¬â e isso êÂ© opcional.

**Preciso de uma conta Claude paga?**
O tier gratuito funciona para uso leve. Para uso diêÂ¡rio com sessêÂµes longas, o Claude Pro (US$ 20/mêÂªs) oferece substancialmente mais uso do que custos equivalentes de API em outras ferramentas.

**E se eu jêÂ¡ tiver um vault do Obsidian?**
O script de setup pergunta onde fica seu vault. Aponte para o vault existente ê¢â¬â ele vai copiar o template do CLAUDE.md, skills e scripts sem tocar nas suas notas existentes.

**Posso usar sem o processamento de arquivos?**
Com certeza. A chave API do Gemini e o processamento de arquivos sêÂ£o opcionais. O sistema central (Obsidian + Claude Code + CLAUDE.md + slash commands) funciona sem isso.

**O Obsidian êÂ© obrigatêÂ³rio?**
NêÂ£o. O vault êÂ© feito de arquivos Markdown comuns. VocêÂª pode usar qualquer editor (VS Code, Typora, Neovim, etc.). O Obsidian agrega valor pelo graph view, plugins da comunidade e CLI integrada, mas nêÂ£o êÂ© requisito.

**As notas se atualizam sozinhas?**
NêÂ£o. VocêÂª precisa rodar `/daily` no inêÂ­cio do dia e `/tldr` no final de cada sessêÂ£o. NêÂ£o hêÂ¡ automaêÂ§êÂ£o em background ê¢â¬â tudo êÂ© acionado manualmente por comando.

---

<div align="center">

*Se isso te ajudou a criar seu segundo cêÂ©rebro, deixe uma ê¢Â­Â ê¢â¬â ajuda outros a encontrar.*

</div>

---

Projeto  - ARCKHÉe