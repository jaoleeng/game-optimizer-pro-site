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
