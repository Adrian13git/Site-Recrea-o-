# Estratégia

> O que importa agora. Prioridades, metas, prazos.
> O Claude usa isso pra decidir o que sugerir primeiro e o que adiar.
> Atualize sempre que as prioridades mudarem.

## Fase

Começando agora. Primeiro projeto (teste/portfólio) em andamento: site pra Era Uma Vez - Recreação Infantil. Ainda sem carteira de clientes fechada.

## Prioridade principal

Entregar o site da Era Uma Vez - Recreação Infantil: serviços prestados, galeria das recreações, links diretos pro WhatsApp e Instagram, usando a paleta de cores definida.

**Status (01/09/2026):** site em `clientes/era-uma-vez/` estruturado e funcional
(header, hero, sobre, serviços, recreações, feedbacks, contato, footer), fundo
roxo da marca, logos aplicados, textos revisados, menu reordenado batendo com a
ordem das seções (Sobre, Serviços, Recreações, Feedbacks, Contato). Header mobile
corrigido (menu hambúrguer entra mais cedo, antes de espremer). WhatsApp
(+55 19 99121-5121) e Instagram (@_eraumavezrecreacao) conectados em todos os
botões, com ícone e mensagem pré-preenchida no WhatsApp. Seção "Recreações" já
tem 2 vídeos reais das oficinas (`video/`); seção nova "O que nossos clientes
dizem" com 6 prints de feedback reais (`img/feedbacks/`), alternando fundo
claro/escuro, navegação por setas. Área de atendimento adicionada no Contato:
"Atendemos Mococa (SP) e cidades próximas com taxa de deslocamento."

**Atualização (21/09/2026):** galeria "Recreações" com 6 vídeos reais das
oficinas (comprimidos com ffmpeg, 36MB→15,7MB sem perda visível de qualidade),
em formato vertical 9:16 (igual ao original, sem corte) numa fileira única
navegada por setas — mesmo padrão da seção "Feedbacks", que já tem 8 prints
reais. Cards de "Serviços" ganharam foto de fundo bem clara, uma por serviço
(`img/servico-*`). Seção "Sobre" ganhou foto de fundo clara também
(`img/sobre-bg.jpg`). Falta pra ficar 100% pronto pra publicar:

- Confirmar/ajustar a lista de serviços (4 cards atuais ainda podem ser exemplo)

Checklist completo em `clientes/era-uma-vez/README.md`.

**Nota técnica:** ffmpeg e ImageMagick foram instalados no sistema (via winget)
pra processar vídeo/imagem — úteis pra próximas compressões, recortes ou
remoção de fundo (o ImageMagick com floodfill a partir dos cantos é o método
que funcionou bem pra remover fundo falso/checkerboard sem furar detalhes
brancos do personagem, tipo dentes e olhos).

**Atualização (22/09/2026):** adicionada mascote ilustrada da Era Uma Vez
(gerada em IA, `_memoria`/pasta `animações` do usuário) flutuando no espaço
roxo entre as seções — 3 poses aplicadas: pintando o rosto de uma criança
(entre Sobre/Serviços), jogo do paraquedas colorido (entre Serviços/Recreações)
e corrida de saco (entre Recreações/Feedbacks). Também foram adicionadas
formas decorativas flutuantes (bolinhas e estrelas em CSS puro, sem imagem)
no fundo roxo do Hero, do CTA final e do rodapé. Nota de cuidado: algumas
poses testadas tiveram um bug visual de corte/faixa roxa no meio da imagem
ao usar sobreposição com margem negativa (`.floating-mascote--right`) —
poses com braços/pernas muito abertos perto da borda do recorte pareciam
disparar isso; poses mais compactas (corpo mais "fechado", sem membros
esticados perto da borda) resolveram na prática. Se o problema voltar a
aparecer, vale revisitar a técnica de posicionamento (a versão sem margem
negativa/sombra, mais simples, nunca chegou a ser confirmada como resolvendo
ou não, pois o usuário preferiu voltar ao visual anterior antes de testar).

## O que pode esperar

- Identidade visual própria (marca pessoal do Adrian) — ainda não definida, fica pra depois
- Processo formal de proposta/orçamento/onboarding de cliente

## Contexto com prazo

Nenhum prazo definido ainda.

## Pra tirar das costas (candidatas a skill via `/mapear-rotinas`)

- Criar proposta
- Criar orçamento
- Onboarding de cliente novo
