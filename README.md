<div align="center">

<img src="banner.svg" alt="Second Brain" width="800"/>

**Uma IA que jÃ¡ sabe quem vocÃª Ã© antes de vocÃª digitar uma palavra.**

![macOS](https://img.shields.io/badge/macOS-âœ“-8A2BE2?style=flat-square) ![Windows](https://img.shields.io/badge/Windows-âœ“-8A2BE2?style=flat-square) ![Linux](https://img.shields.io/badge/Linux-âœ“-8A2BE2?style=flat-square) ![Free](https://img.shields.io/badge/custo-grÃ¡tis-8A2BE2?style=flat-square) ![One command](https://img.shields.io/badge/setup-um_comando-8A2BE2?style=flat-square)

[Obsidian](https://obsidian.md) + [Claude Code](https://claude.ai/code) Â· Local Â· Privado Â· Um comando

```
  Seus arquivos (PDFs, docs, notas)
          â”‚
          â–¼
  â”Œâ”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”
  â”‚   Obsidian vault  â”‚  â† arquivos .md no seu computador
  â”‚  inbox/  daily/   â”‚
  â”‚  projects/  ...   â”‚
  â””â”€â”€â”€â”€â”€â”€â”€â”€â”¬â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”˜
           â”‚  Claude Code lÃª esta pasta
           â–¼
  â”Œâ”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”
  â”‚   Claude Code     â”‚  â† conhece seus projetos, voz, contexto
  â”‚   /vault-setup    â”‚     antes de vocÃª digitar uma palavra
  â”‚   /daily  /tldr   â”‚
  â””â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”˜
           â”‚
           â–¼
    IA que se acumula.
    SessÃ£o 1: conhece suas pastas.
    SessÃ£o 20: sabe mais sobre
    seu trabalho do que vocÃª lembra conscientemente.
```

*Se isso te economizou horas, deixe uma â­ â€” ajuda outros a encontrar.*

</div>

---

## InÃ­cio RÃ¡pido

### macOS

**OpÃ§Ã£o A â€” Uma linha** (cole no Terminal e pressione Enter):

```bash
curl -fsSL https://raw.githubusercontent.com/earlyaidopters/second-brain/main/setup.sh -o setup.sh && bash setup.sh
```

**OpÃ§Ã£o B â€” Clonar o repo:**

Abra o **Terminal** (pressione `âŒ˜ Space`, digite `Terminal`, Enter) e rode:

```bash
git clone https://github.com/earlyaidopters/second-brain.git
cd second-brain
./setup.sh
```

> **NÃ£o tem git?** Rode `xcode-select --install` primeiro e tente novamente.

---

### Linux

**OpÃ§Ã£o A â€” Uma linha:**

```bash
curl -fsSL https://raw.githubusercontent.com/earlyaidopters/second-brain/main/setup.sh -o setup.sh && bash setup.sh
```

**OpÃ§Ã£o B â€” Clonar o repo:**

```bash
git clone https://github.com/earlyaidopters/second-brain.git
cd second-brain
./setup.sh
```

> **PrÃ©-requisitos:** `git`, `python3` e `pip` devem estar instalados. Na maioria das distros jÃ¡ vÃªm por padrÃ£o. Se nÃ£o:
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

> **Obsidian no Linux** â€” o script instala automaticamente via Snap, Flatpak ou AppImage. Se preferir instalar manualmente:
> ```bash
> # Snap
> sudo snap install obsidian --classic
>
> # Flatpak
> flatpak install flathub md.obsidian.Obsidian
>
> # AppImage â€” baixe em https://obsidian.md/download
> chmod +x Obsidian-*.AppImage && ./Obsidian-*.AppImage
> ```

---

### Windows

> **Primeiro: vocÃª tem git?**
> Abra o **PowerShell** (pressione `Win`, digite `powershell`, Enter) e rode:
> ```powershell
> git --version
> ```
> Se aparecer um nÃºmero de versÃ£o, estÃ¡ ok. SenÃ£o, instale pelo [git-scm.com](https://git-scm.com/download/win) â€” use todas as opÃ§Ãµes padrÃ£o e reabra o PowerShell.

**OpÃ§Ã£o A â€” Uma linha** (cole no PowerShell e pressione Enter):

```powershell
Invoke-WebRequest -Uri "https://raw.githubusercontent.com/earlyaidopters/second-brain/main/setup.ps1" -OutFile setup.ps1; powershell -ExecutionPolicy Bypass -File setup.ps1
```

**OpÃ§Ã£o B â€” Clonar o repo:**

```powershell
git clone https://github.com/earlyaidopters/second-brain.git
cd second-brain
powershell -ExecutionPolicy Bypass -File setup.ps1
```

> **Erro "execuÃ§Ã£o de scripts desabilitada"?** Ã‰ uma configuraÃ§Ã£o de seguranÃ§a do Windows. O `-ExecutionPolicy Bypass` no comando acima ignora isso apenas para este script â€” nÃ£o muda nada permanente no seu computador.

> **Python nÃ£o encontrado?** Baixe em [python.org/downloads](https://python.org/downloads) â€” na primeira tela do instalador, marque **"Add Python to PATH"** antes de clicar em Install. Depois rode o script de setup novamente.

---

O script cuida do resto: instala Obsidian, instala Claude Code, cria seu vault e opcionalmente importa seus arquivos existentes.

---

## Por que Isso Existe

VocÃª jÃ¡ tentou criar um segundo cÃ©rebro antes.

Talvez Notion. Talvez Apple Notes. Talvez uma pasta de arquivos markdown que vocÃª jurou que ia organizar.

Toda vez, o mesmo resultado: vocÃª configurava, usava por uma semana, e depois esquecia completamente que existia.

O problema nunca foi a ferramenta. **Era que vocÃª precisava lembrar de usÃ¡-la.**

Isto conecta o **Obsidian** (seu vault local de conhecimento) ao **Claude Code** (seu agente de IA) para que:

- Claude Code **leia suas notas** antes de responder â€” ele conhece seus projetos, seus clientes, sua voz
- Claude Code **escreva suas notas** depois de trabalhar â€” seu vault se constrÃ³i sozinho a partir das sessÃµes
- Seus arquivos existentes (PDFs, docs, slides) sÃ£o **sintetizados e importados automaticamente** via Gemini 3 Flash
- Tudo fica **local, privado e seu** â€” sem lock-in de nuvem, sem assinaturas crescentes

O resultado: uma IA que sabe quem vocÃª Ã© desde o primeiro prompt de cada sessÃ£o. NÃ£o porque vocÃª contou. Porque ela leu seu vault.

---

## O que Ã© Instalado

| Ferramenta | O que Ã© | Para quÃª |
|------------|---------|----------|
| **Obsidian** | App gratuito de notas | Suas notas vivem como arquivos `.md` no seu computador â€” sem nuvem, sem assinatura, seus para sempre |
| **Claude Code** | Terminal IA da Anthropic | LÃª e escreve arquivos diretamente no seu vault â€” sem copiar/colar, sem trocar de aba |
| **Pacotes Python** | Bibliotecas de fundo | Usadas pelo Gemini 3 Flash para ler e sintetizar seus arquivos existentes (PDFs, docs, slides) |
| **Vault skills** | Slash commands | `/vault-setup` `/daily` `/tldr` `/file-intel` â€” ensinam o Claude a trabalhar com seu vault |
| **Obsidian Skills** *(opcional)* | Skills oficiais do [Kepano](https://github.com/kepano) (CEO do Obsidian) | Permite ao Claude navegar, ler e escrever seu vault nativamente usando a CLI do Obsidian |

> **Nada Ã© enviado para servidores.** Seu vault Ã© uma pasta no seu computador. Claude Code lÃª localmente. A Ãºnica chamada de rede opcional Ã© o processamento via Gemini â€” e Ã© totalmente pulÃ¡vel.

---

## O que o Script de Setup Faz

```
Passo 1 â€” Verificar dependÃªncias       (Homebrew no Mac / winget no Windows / apt/dnf/pacman no Linux)
Passo 2 â€” Instalar Obsidian            (app gratuito de notas local)
Passo 3 â€” Instalar Claude Code CLI     (terminal IA da Anthropic)
Passo 4 â€” Instalar pacotes Python      (para processamento de arquivos via Gemini)
Passo 5 â€” Criar seu vault              (inbox, daily, projects, research, archive + skills)
Passo 6 â€” Importar arquivos existentes (opcional â€” Gemini lÃª e sintetiza)
Passo 7 â€” Obsidian Skills              (opcional â€” skills oficiais do Kepano, CEO do Obsidian)
           â””â”€> Abre o Obsidian apontando para seu novo vault
```

---

## Depois do Setup

### 1. Habilitar a CLI do Obsidian
```
Obsidian â†’ Settings â†’ General â†’ Enable Command Line Interface
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

O Claude Code vai te entrevistar sobre seu papel e trabalho, depois gerar um `CLAUDE.md` personalizado e sugerir slash commands para seu fluxo de trabalho especÃ­fico. Um empresÃ¡rio recebe pastas diferentes de um desenvolvedor. Um criador de conteÃºdo recebe comandos diferentes de um consultor.

---

## Slash Commands

Quatro comandos vÃªm prÃ©-instalados. Mais sÃ£o adicionados conforme vocÃª usa o sistema.

| Comando | O que faz |
|---------|-----------|
| `/vault-setup` | Te entrevista (papel, projetos, objetivos) e gera estrutura personalizada do vault + CLAUDE.md + slash commands customizados |
| `/daily` | ComeÃ§a seu dia â€” lÃª a nota de hoje ou cria uma, mostra prioridades, pergunta no que vocÃª estÃ¡ trabalhando |
| `/tldr` | No final de qualquer sessÃ£o, salva um resumo estruturado na pasta certa do vault automaticamente |
| `/file-intel` | Aponte para qualquer pasta â€” Gemini lÃª cada arquivo e gera resumos prontos para Obsidian no seu inbox |

> **Importante:** Slash commands sÃ³ ativam quando o Claude Code Ã© aberto de dentro da pasta do vault. Sempre faÃ§a `cd` para o vault antes de rodar `claude`.
>
> ```bash
> cd ~/second-brain              # Mac / Linux
> cd $env:USERPROFILE\second-brain   # Windows
> claude
> ```
>
> **Quer que funcionem em qualquer lugar?** Dentro do Claude Code, peÃ§a:
> *"FaÃ§a esses slash commands globais para funcionarem em qualquer pasta"*
> O Claude Code vai copiar os skills para `~/.claude/skills/`.

---

## Importando Arquivos Existentes

Tem anos de PDFs, documentos Word e apresentaÃ§Ãµes guardados em pastas? NÃ£o converta manualmente.

```bash
python3 scripts/process_docs_to_obsidian.py ~/seus-arquivos ~/second-brain/inbox
```

**O que acontece:**
1. Cada arquivo Ã© lido pelo **Gemini 3 Flash** (`gemini-3-flash-preview`)
2. O sinal Ã© extraÃ­do, o ruÃ­do Ã© descartado (boilerplate jurÃ­dico, cabeÃ§alhos, enchimento)
3. Uma nota Markdown limpa e compacta Ã© salva no seu `inbox/` (300â€“600 palavras mÃ¡x.)

Depois abra o Claude Code e diga: *"Organize tudo no inbox/ nas pastas certas."*

Ele lÃª seu CLAUDE.md, entende a estrutura do vault e encaminha cada nota para onde pertence.

**Formatos suportados:** `.pdf` `.docx` `.pptx` `.txt` `.md`

> **Tem arquivos Excel, CSV ou JSON tambÃ©m?** Use o script mais abrangente:
> ```bash
> python3 scripts/process_files_with_gemini.py ~/seus-arquivos
> ```
> Ele processa `.xlsx` `.csv` `.json` `.xml` `.py` `.js` `.html` e a maioria dos arquivos baseados em texto. Resultados ficam em `outputs/file_summaries/` com um `MASTER_SUMMARY.md` resumindo tudo.

---

## Como a MemÃ³ria Funciona

Seu vault Ã© estruturado para que o Claude Code encontre o contexto certo para qualquer tarefa:

```
~/second-brain/
â”œâ”€â”€ CLAUDE.md        â† O cÃ©rebro do cÃ©rebro. Lido no inÃ­cio de cada sessÃ£o.
â”œâ”€â”€ memory.md        â† Log de sessÃµes. Atualizado pelo Claude Code apÃ³s cada conversa.
â”œâ”€â”€ inbox/           â† Zona de entrada. Qualquer coisa nova cai aqui primeiro.
â”œâ”€â”€ daily/           â† Notas diÃ¡rias (YYYY-MM-DD.md). Seu log contÃ­nuo.
â”œâ”€â”€ projects/        â† Projetos ativos. Claude lÃª o relevante antes de ajudar.
â”œâ”€â”€ research/        â† Conhecimento sintetizado. Fontes, notas, ideias.
â””â”€â”€ archive/         â† Trabalho concluÃ­do. Nunca delete â€” apenas archive.
```

**O efeito composto:**
- SessÃ£o 1: Claude conhece a estrutura das suas pastas
- SessÃ£o 5: Claude conhece seus projetos, sua voz, suas preferÃªncias
- SessÃ£o 20: Claude Ã© seu sistema operacional personalizado â€” sabe mais sobre sua base de conhecimento do que vocÃª lembra conscientemente

> **Nota:** A atualizaÃ§Ã£o da memÃ³ria **nÃ£o Ã© automÃ¡tica**. VocÃª precisa rodar `/tldr` no final de cada sessÃ£o para salvar o resumo, e `/daily` no inÃ­cio do dia para carregar o contexto. Os arquivos nÃ£o se atualizam sozinhos em background.

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
| Chave API Google | Todas | [aistudio.google.com/apikey](https://aistudio.google.com/apikey) â€” grÃ¡tis |
| Conta Claude | Todas | [claude.ai](https://claude.ai) â€” Pro recomendado para uso intenso |

---

## Estrutura do RepositÃ³rio

```
second-brain/
â”œâ”€â”€ setup.sh                              â† Setup macOS/Linux (um comando)
â”œâ”€â”€ setup.ps1                             â† Setup Windows (um comando)
â”œâ”€â”€ CLAUDE.md                             â† Arquivo de sistema do vault (personalizado pelo /vault-setup)
â”œâ”€â”€ memory.md                             â† MemÃ³ria de sessÃ£o (atualizado pelo Claude Code)
â”œâ”€â”€ requirements.txt                      â† DependÃªncias Python
â”œâ”€â”€ .env.example                          â† Copie para .env, adicione sua chave API Google
â”œâ”€â”€ .gitignore                            â† MantÃ©m .env e .venv fora do git
â”œâ”€â”€ scripts/
â”‚   â”œâ”€â”€ process_docs_to_obsidian.py      â† Sintetizador de arquivos via Gemini 3 Flash
â”‚   â””â”€â”€ process_files_with_gemini.py     â† Processador batch Gemini
â”œâ”€â”€ skills/
â”‚   â”œâ”€â”€ vault-setup/SKILL.md             â† Configurador interativo do vault
â”‚   â”œâ”€â”€ daily/SKILL.md                   â† Comando de standup diÃ¡rio
â”‚   â”œâ”€â”€ tldr/SKILL.md                    â† Comando de resumo de sessÃ£o
â”‚   â””â”€â”€ file-intel/SKILL.md              â† Processar qualquer pasta via Gemini
â””â”€â”€ vault-template/
    â”œâ”€â”€ inbox/   daily/   projects/
    â”œâ”€â”€ research/   archive/
```

---

## Setup Manual

<details>
<summary>Prefere instalar cada peÃ§a manualmente? Clique para expandir o passo a passo completo para todas as plataformas.</summary>

---

### macOS â€” Passos Manuais

**1. Instalar Homebrew** (instalador de apps do macOS â€” pule se jÃ¡ tem)
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

### Linux â€” Passos Manuais

**1. Instalar dependÃªncias**
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
# OpÃ§Ã£o 1: Snap (Ubuntu e derivados)
sudo snap install obsidian --classic

# OpÃ§Ã£o 2: Flatpak
flatpak install flathub md.obsidian.Obsidian

# OpÃ§Ã£o 3: AppImage
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

**5. Instalar dependÃªncias Python**
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

### Windows â€” Passos Manuais

Abra o **PowerShell** para todos os comandos abaixo.

**1. Instalar Obsidian**
```powershell
winget install Obsidian.Obsidian
```

**2. Instalar Claude Code**
```powershell
winget install Anthropic.ClaudeCode
```
Feche e reabra o PowerShell apÃ³s este passo.

**3. Instalar Python** (se nÃ£o tem)

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

**5. Instalar dependÃªncias Python**
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

**Meus dados sÃ£o privados?**
Sim. O Obsidian armazena tudo como arquivos markdown locais no seu computador. Nada Ã© enviado para nenhum servidor. O Claude Code processa seus arquivos localmente na pasta onde vocÃª o abre. A Ãºnica vez que algo sai da sua mÃ¡quina Ã© quando vocÃª chama a API do Gemini para processar arquivos existentes â€” e isso Ã© opcional.

**Preciso de uma conta Claude paga?**
O tier gratuito funciona para uso leve. Para uso diÃ¡rio com sessÃµes longas, o Claude Pro (US$ 20/mÃªs) oferece substancialmente mais uso do que custos equivalentes de API em outras ferramentas.

**E se eu jÃ¡ tiver um vault do Obsidian?**
O script de setup pergunta onde fica seu vault. Aponte para o vault existente â€” ele vai copiar o template do CLAUDE.md, skills e scripts sem tocar nas suas notas existentes.

**Posso usar sem o processamento de arquivos?**
Com certeza. A chave API do Gemini e o processamento de arquivos sÃ£o opcionais. O sistema central (Obsidian + Claude Code + CLAUDE.md + slash commands) funciona sem isso.

**O Obsidian Ã© obrigatÃ³rio?**
NÃ£o. O vault Ã© feito de arquivos Markdown comuns. VocÃª pode usar qualquer editor (VS Code, Typora, Neovim, etc.). O Obsidian agrega valor pelo graph view, plugins da comunidade e CLI integrada, mas nÃ£o Ã© requisito.

**As notas se atualizam sozinhas?**
NÃ£o. VocÃª precisa rodar `/daily` no inÃ­cio do dia e `/tldr` no final de cada sessÃ£o. NÃ£o hÃ¡ automaÃ§Ã£o em background â€” tudo Ã© acionado manualmente por comando.

---

<div align="center">

*Se isso te ajudou a criar seu segundo cÃ©rebro, deixe uma â­ â€” ajuda outros a encontrar.*

</div>

---

Projeto adaptado da comunidade INEMA TDS - Marca Arckhe