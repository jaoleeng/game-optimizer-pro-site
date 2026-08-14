# Textos prontos pra divulgação

Só copiar e colar. Ajustei o tom pra cada lugar — comunidade de dev
(TabNews) gosta de detalhe técnico e humildade ("é beta, quero
feedback"); Reddit/Discord de hardware quer saber rápido o que o
troço faz.

**Antes de postar:** evita postar em vários lugares no mesmo dia — a
maioria dessas comunidades pune (shadowban/remove post) quem parece
estar "spamando" o mesmo link em vários fóruns ao mesmo tempo. Espaça
uns dias entre cada um.

---

## TabNews (tabnews.com.br) — comunidade BR de devs, ótimo fit

**Título:** Fiz um app de otimização de PC pra jogos no Windows (Electron + Node) — feedback bem-vindo

**Corpo:**
```
Passei as últimas semanas construindo um app desktop pra Windows que
aplica otimizações reais de sistema pra jogos: plano de energia
"Ultimate Performance" (o oculto, mais agressivo que Alto Desempenho),
GPU Scheduling acelerado por hardware, ajustes de latência de
mouse/teclado, prioridade de processos, overclock assistido via MSI
Afterburner, perfis salvos por jogo com um botão "Jogar" que aplica
tudo e já abre o executável, e um painel de monitoramento (CPU, GPU,
VRAM, temperatura, disco, rede) sem precisar de outro programa aberto.

Stack: Electron + Node no cliente, Express + Redis (Upstash) no
backend, pagamento recorrente via Mercado Pago pra conta Premium.
Free tier libera 2 ajustes básicos; o resto é assinatura.

Ainda é beta — instalador não assinado digitalmente ainda (então o
SmartScreen do Windows avisa "editor desconhecido", é normal nessa
fase), mas todo o resto funciona de verdade, testei ponta a ponta.

Site + download: https://jaoleeng.github.io/game-optimizer-pro-site/

Quero feedback sincero, principalmente de quem manja de Windows
internals — se algum dos tweaks parecer bobagem ou perigoso, quero
saber.
```

---

## Reddit — r/computadores, r/brasil, r/hardware (Brasil)

**Título:** Criei um otimizador de PC pra jogos (grátis pra testar) — Game Optimizer PRO

**Corpo:**
```
E aí! Fiz um programinha pra Windows que junta um monte de tweak de
otimização que geralmente a gente vai atrás um por um (plano de
energia oculto, GPU Scheduling, prioridade de processo, latência de
mouse/USB, etc) num painel só, com perfil salvo por jogo.

Também tem um monitor de CPU/GPU/RAM/disco/rede embutido, então não
precisa abrir outro programa do lado.

É gratuito pra testar (2 ajustes liberados sem conta), o resto é uma
assinatura de R$19,90/mês. Ainda tá em beta e o instalador não é
assinado digitalmente ainda, então o Windows vai avisar "editor
desconhecido" — é clicar em "Mais informações → Executar assim
mesmo".

Link: https://jaoleeng.github.io/game-optimizer-pro-site/

Quero saber se funcionou na máquina de vocês e se algum ajuste fez
diferença de verdade. Feedback (bom ou ruim) é bem-vindo.
```

---

## Discord (servidores de hardware/PC gamer, canal de showcase/projetos)

**Curto, pra colar direto:**
```
Fiz um app de otimização de PC pra jogos no Windows 🎮⚡
Plano de energia oculto, GPU Scheduling, ajuste de latência de
mouse/teclado, perfis por jogo (botão "Jogar" já aplica tudo e abre
o game) e um monitor de CPU/GPU/RAM/disco/rede embutido.

Grátis pra testar: https://jaoleeng.github.io/game-optimizer-pro-site/

Ainda em beta, iam ajudar demais testando e falando o que acharam!
```

---

## Dica extra: Product Hunt

Também dá pra listar de graça em producthunt.com — cadastro com
conta própria (GitHub serve pra logar), sem custo. É mais indicado
quando o produto já estiver com aparência mais "final" (ícone
próprio, instalador assinado) porque a audiência de lá é mais
exigente com polish. Guardo essa sugestão pra depois dessas duas
pendências.

---

## AlternativeTo.net

Cadastro gratuito em alternativeto.net/software/new (ou pelo menu
"Add app"). Pede login (dá pra usar Google/GitHub). Preenche assim:

- **App name:** Game Optimizer PRO
- **Short description / tagline:** Otimizador de PC para jogos no Windows, com monitor de hardware e perfis por jogo
- **Description (completa):**
  ```
  App desktop para Windows que aplica otimizações reais de sistema
  voltadas a jogos: plano de energia "Ultimate Performance" (o oculto
  do Windows, mais agressivo que Alto Desempenho), GPU Scheduling
  acelerado por hardware (HAGS), prioridade de processos, ajustes de
  latência de mouse/teclado (aceleração do mouse, USB Selective
  Suspend), redução de latência de rede (Nagle) e limpeza de sistema.

  Perfis salvos por jogo: guarda quais ajustes usar para cada game e
  aplica tudo com um clique — o botão "Jogar" já abre o executável do
  jogo na sequência. Overclock assistido troca entre perfis já
  configurados no MSI Afterburner (não escreve valores de
  clock/voltagem diretamente). Monitor embutido de CPU, GPU
  (temperatura, VRAM, clocks, consumo, fan), RAM, disco e rede, sem
  precisar de outro programa aberto.

  Grátis para testar (2 ajustes liberados sem conta); o restante é
  assinatura mensal via Mercado Pago.
  ```
- **Categoria/tags:** System Optimization, Game Boosters, System Utilities, Windows
- **"Alternative to" (marcar como similar a):** MSI Afterburner, Razer Cortex, Wise Game Booster, Advanced SystemCare, Process Lasso
- **Platform:** Windows
- **Licensing model:** Freemium
- **Official website:** https://jaoleeng.github.io/game-optimizer-pro-site/
- **Screenshot:** usa `assets/screenshot-monitor.png` do repositório do site

---

## Hacker News (Show HN)

Posta em news.ycombinator.com/submit, logado. O pessoal de lá valoriza
honestidade técnica e detesta tom de propaganda — o título/post abaixo
já está nesse tom.

**Título:**
```
Show HN: Windows game optimizer with a native hardware monitor (Electron + C#)
```

**URL:** `https://jaoleeng.github.io/game-optimizer-pro-site/`

**Primeiro comentário (poste logo após submeter, é praxe no Show HN
explicar o "porquê" e os detalhes técnicos):**
```
Built this over the past few weeks — a Windows desktop app that
applies real system-level optimizations for gaming (hidden "Ultimate
Performance" power plan, Hardware-Accelerated GPU Scheduling, mouse
acceleration / USB selective suspend disable, Nagle's algorithm
disable, process priority tweaks) plus a live hardware monitor.

The monitor part was the interesting problem: reading GPU temperature/
VRAM/clocks works fine cross-vendor via each GPU maker's own library,
but CPU temperature requires reading MSRs, which needs a kernel driver
— and Microsoft's Vulnerable Driver Blocklist (on by default since
Win11 22H2) blocks the common community drivers (WinRing0 etc.) that
every free hardware monitor relies on. Ended up bundling a small
self-contained .NET helper (using LibreHardwareMonitorLib) that the
Electron app spawns headlessly, so there's no separate app for the
user to install — CPU temp still fails on locked-down systems though,
which the UI explains rather than showing a silent "N/D".

Stack: Electron + Node client, Express + Redis (Upstash) backend,
Mercado Pago for recurring subscriptions. Free tier unlocks 2 basic
tweaks; the rest is a paid subscription.

Still beta — installer isn't code-signed yet, so Windows SmartScreen
warns about it. Happy to answer questions about any of the Windows
internals stuff.
```

---

## Fórum Adrenaline (adrenaline.com.br) e Clube do Hardware (clubedohardware.com.br)

Os dois têm uma seção de software/dicas onde esse tipo de post encaixa
bem. Mesmo texto serve pros dois (ajusta o título conforme o fórum
pedir):

**Título:** [Software] Criei um otimizador de PC para jogos — Game Optimizer PRO (grátis pra testar)

**Corpo:**
```
Fala, pessoal! Desenvolvi um programa para Windows que junta vários
ajustes de otimização para jogos num painel só, em vez de ter que ir
atrás de tutorial por tutorial:

- Plano de energia "Ultimate Performance" (o oculto do Windows)
- GPU Scheduling acelerado por hardware (HAGS)
- Prioridade de processos em primeiro plano
- Desativar aceleração do mouse e USB Selective Suspend (reduz
  microlag de mouse/teclado)
- Desativar algoritmo de Nagle (latência de rede em jogos online)
- Limpeza de temporários/Prefetch, flush de DNS, fechar processos em
  segundo plano

Também tem perfis salvos por jogo (aplica os ajustes certos e já abre
o jogo com um clique) e um monitor de CPU/GPU/RAM/disco/rede — dá pra
ver temperatura e uso de tudo sem abrir outro programa.

É gratuito para testar (libera 2 ajustes sem precisar de conta), o
resto é assinatura. Ainda tá em beta e o instalador não é assinado
digitalmente, então o Windows avisa "editor desconhecido" ao abrir —
é clicar em "Mais informações" → "Executar assim mesmo".

Link: https://jaoleeng.github.io/game-optimizer-pro-site/

Testei bastante na minha máquina, mas quero saber se funciona bem em
outras configurações e se algum ajuste fez diferença real pra vocês.
Críticas e sugestões são bem-vindas!
```

---

## Softpedia / MajorGeeks (diretórios de software)

Esses usam formulário de submissão mais longo — o link fica no rodapé
do site deles ("Submit Software" / "Add your software"), varia de vez
em quando então procura por esse texto no menu/rodapé. Campos comuns e
o que preencher:

- **Software name:** Game Optimizer PRO
- **Version:** 0.1.0
- **Short description (~150 caracteres):** Otimizador de sistema para jogos no Windows: energia, GPU Scheduling, latência de input, perfis por jogo e monitor de hardware.
- **Long description:** usa o mesmo texto da seção do AlternativeTo acima
- **Category:** System Utilities / Games → Game Enhancement / Optimization Tools
- **Operating system:** Windows 10, Windows 11 (64-bit)
- **License:** Freeware / Free to try (freemium — deixa claro que tem versão paga)
- **Homepage URL:** https://jaoleeng.github.io/game-optimizer-pro-site/
- **Download URL:** link direto do instalador — `https://github.com/jaoleeng/game-optimizer-pro-site/releases/latest/download/GameOptimizerPRO-Setup.exe`
- **Screenshots:** os três PNGs em `assets/` do repositório do site

**Aviso importante:** alguns desses diretórios rejeitam ou sinalizam
instaladores não assinados digitalmente (o nosso caso hoje). Se
acontecer, não é erro seu no formulário — é a falta de assinatura de
código mesmo, só resolve isso comprando um certificado. Vale tentar
mesmo assim; muitos aceitam com um aviso extra na ficha.
