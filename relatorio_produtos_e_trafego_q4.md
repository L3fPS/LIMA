# Relatório de Produtos e Tráfego — Q4 (gerado em 10/10/2026)

## ⚠️ Leia antes: limites desta extração

- **Acesso direto bloqueado.** O proxy do ambiente nega facebook.com, similarweb.com e as lojas. Usei o `web_fetch` do Parallel Search, que devolve **snapshots em cache**, não consultas ao vivo.
- **Meta Ads Library — contagem por produto NÃO é confiável.** O snapshot só carrega os primeiros ~15–35 anúncios por busca (scroll infinito). Os links de destino só aparecem em parte dos anúncios, e as imagens/vídeos (CDN `scontent`) não vieram no texto. Por isso:
  - Os números por produto são **mínimos observados (lower bound)**, não totais.
  - **Não há URL de thumbnail/vídeo de anúncio** em nenhuma loja. Onde aparece imagem, é imagem do produto na loja, e isso está indicado.
  - Nenhum produto da kiddofinds passou no filtro ">3 anúncios" na amostra (30 anúncios lidos, 30 produtos diferentes, 1 anúncio cada).
- **Busca por keyword do domínio** traz anúncios de terceiros (afiliados, criadores), então o total da busca ≠ anúncios da loja.
- **SimilarWeb:** a maioria dos snapshots é de **set/2026**, mas neefty (abr/2025) e scomeri (mai/2025) são antigos. Wiggo's e Mini RC não têm página indexada. Visitas totais só vieram para 4 lojas.
- **Próximo passo recomendado:** rodar a Ad Library API oficial (token de acesso) ou Apify/AdSpy a partir de uma máquina sem bloqueio de rede, ou exportar manualmente. Aí o filtro >3 anúncios/produto fica confiável.

---

## 1. Kiddofinds
- **Domínio:** https://kiddofinds.com
- **Total de Ads Ativos da Loja:** ~120 (busca por keyword; snapshot em cache, data não informada, com anúncios até ago/2026)

### 📊 Benchmark de Tráfego (SimilarWeb, set/2026)
- **Visitas Mensais Estimadas:** ~12,3 mil (Prostats, fonte alternativa: ~3,7 mil visitantes únicos / 11 mil pageviews)
- **Principal Fonte de Tráfego:** Paid Social 29,2% (1º), Direct (2º), Organic Search (3º). Social vem majoritariamente do Facebook.
- **Engajamento:** Bounce 82,8% · 1,09 págs/visita · duração média 2s (sinal de tráfego pago de baixa qualidade ou bot)

### 🏆 Top Produtos Escalados
Nenhum produto passou o filtro >3 na amostra lida (30 de ~120 anúncios). Os produtos abaixo são os que apareceram com anúncio ativo; confirmar contagem real na Ad Library.

| Produto | Anúncios vistos | Hook/Ângulo | Link |
|---|---|---|---|
| Rainbow Spinning & Color Tower Toy | 1 | "Safe, colourful, educational toy" + "save up to 50%" | https://kiddofinds.com/products/rainbow-spinning-and-color-tower-toy |
| Hands-Free Nursing Pillow | 1 | Prova social ("thousands of happy parents") + 50% OFF | https://kiddofinds.com/products/hands-free-nursing-pillow-for-babies |
| Dancing Saxophone Caterpillar | 1 | Ritmo/coordenação, brinquedo musical | https://kiddofinds.com/products/dancing-saxophone-caterpillar |
| Peek-A-Boo Teddy | 1 | Bebê rindo, brinquedo que fala e ensina | https://kiddofinds.com/products/peek-a-boo-teddy-interactive-plush-toy |
| Kids Karaoke Machine | 1 | "Transforme a casa num palco" | https://kiddofinds.com/products/kids-karaoke-machine-with-microphone-stand-singing-fun-set |

- **Padrão de copy:** "KIDDOFINDS.COM #1 [produto] — Save 50% now! 🚨". Mesma estrutura para todos os produtos, sinal de **teste de catálogo amplo** e não de escala em um produto.
- **Preview:** não capturado (somente texto da biblioteca).

---

## 2. Stryka
- **Domínio:** https://stryka.shop
- **Total de Ads Ativos da Loja:** ~34 (snapshot de **out–nov/2025**, desatualizado)

### 📊 Benchmark de Tráfego (SimilarWeb, set/2026)
- **Visitas Mensais Estimadas:** não exibida no snapshot (variação +4,05% vs. mês anterior)
- **Principal Fonte de Tráfego:** Paid Social 51,6% (1º), Organic Social (2º), Paid Search (3º)
- **Engajamento:** Bounce 92,1% · 1,03 págs/visita

### 🏆 Top Produtos Escalados
1. **STRYKA™ SkillZone — Football Target Game**
   * Quantidade de Anúncios Ativos: **~34 (loja de produto único: praticamente todos os anúncios)**. Contagem do snapshot de 2025. Verificar se continuam ativos.
   * Hook/Ângulo: "Create memories, NOT screen time ⚽", "40% OFF TODAY", "⚠️ WARNING: May trigger all-out family tournaments". Atualmente "WORLD CUP SALE".
   * Link de Destino: https://stryka.shop (loja de 1 produto; URL de produto específica não capturada)
   * Preview (imagem do produto na loja, **não** o criativo do anúncio): https://stryka.shop/cdn/shop/files/STRYKASQUARE_1.png?v=1781790400

---

## 3. Neefty
- **Domínio:** https://neefty.co
- **Total de Ads Ativos da Loja:** não obtido (Ad Library não retornou resultados no snapshot)

### 📊 Benchmark de Tráfego (SimilarWeb, **abr/2025**, desatualizado)
- **Visitas Mensais Estimadas:** 5,5 mil
- **Principal Fonte de Tráfego:** Direct 44,6%, Organic Search 28,7%
- **Engajamento:** Bounce 48,8% · 1,64 págs/visita

### 🏆 Top Produtos Escalados
Sem dados. A home do site só mostra "The Ultimate Fun Store".

---

## 4. Toddla
- **Domínio:** https://toddla.co
- **Total de Ads Ativos da Loja:** a busca retorna ~1.100 resultados, mas isso inclui páginas de terceiros ("Mia's Mom Hacks" etc.) e criadores. Não é o total da loja. Snapshot de 30/06/2026, com anúncios até 13/09/2026.

### 📊 Benchmark de Tráfego (SimilarWeb, set/2026)
- **Visitas Mensais Estimadas:** ~265,9 mil (−3,06% vs. mês anterior)
- **Principal Fonte de Tráfego:** Paid Social 36,7% (1º), Paid Search (2º), Display (3º). 59% do tráfego de keywords é pago.
- **Engajamento:** Bounce 68,4% · 2,54 págs/visita · 1m27s

### 🏆 Top Produtos Escalados
Os links de destino não vieram no snapshot, então a contagem por produto é **não determinada**. Produtos/ângulos identificáveis pela copy:
1. **Toddla™ Octopus Bath Toy**: "50% OFF ENDS TONIGHT 🚨" (aparece em ≥3 anúncios com a mesma copy, datas 30/06 e 23/07/2026; mínimo observado, ~3). Link: não capturado.
2. **Cortador de unhas de bebê**: "Trimming a newborn's nails shouldn't feel like defusing a bomb". Link: não capturado.
3. **Brinquedo sensorial com zíperes/fivelas (busy board)**: "If your toddler is constantly reaching for zippers, buckles…". Link: não capturado.
- **Padrão:** copy em primeira pessoa/UGC, parcerias com creators ("with Tasha Torres", "with Savannah Bell"), tema sazonal de Natal já em setembro.
- **Preview:** não capturado.

---

## 5. The Familys Place
- **Domínio:** https://thefamilysplace.com
- **Total de Ads Ativos da Loja:** não obtido (Ad Library vazia no snapshot)

### 📊 Benchmark de Tráfego (SimilarWeb, set/2026)
- **Visitas Mensais Estimadas:** ~24,4 mil (+35,4% vs. mês anterior)
- **Principal Fonte de Tráfego:** Paid Social 41,9% (1º), Organic Social (2º), Organic Search (3º)
- **Engajamento:** Bounce 81,4% · 1,88 págs/visita · 43s

### 🏆 Top Produtos Escalados
Sem contagem de anúncios. Destaques da home (catálogo com 126 produtos):
1. **Peek a boo Talking Elephant**: $34,99 (de $70). Preview (imagem na loja): https://thefamilysplace.com/cdn/shop/files/3_1_1800x1800.jpg?v=1734982184
2. Reusable Kids Magic Water Book · Baby Neck Support Pillow · Baby Bottle Spoon ($11,99).

---

## 6. Scomeri
- **Domínio:** https://scomeri.com
- **Total de Ads Ativos da Loja:** ~65 (snapshot de **10/10/2026**, atual). Anúncios iniciados de abr a out/2026, incluindo 2 que começaram hoje.

### 📊 Benchmark de Tráfego (SimilarWeb, **mai/2025**, desatualizado)
- **Visitas Mensais Estimadas:** 152 (praticamente zero; sem dado mais recente)
- **Principal Fonte de Tráfego:** Direct 41,8%, Organic Search 34,6%
- **Engajamento:** Bounce 94,3% · 1,00 pág/visita

### 🏆 Top Produtos Escalados
Os links de destino não vieram, então a contagem por produto é **não determinada**. Catálogo generalista (estilo "loja de achadinhos"). Hero da home:
1. **Bone Conduction Smart Hearing Aid Bluetooth Earphones** — $99,99 (de $299,99, −66%). Link: https://scomeri.com/products/bone-conduction-smart-hearing-aid-bluetooth-earphones
- Outros itens: Electric Fabric Lint Remover, Wood Furniture Repair Paint, Car Spray 3-in-1.
- Há pares "2 ads use this creative", indicando criativos duplicados em escala.

---

## 7. HeyWondr (antiga Blumi)
- **Domínio:** https://heywondr.com
- **Total de Ads Ativos da Loja:** não obtido (snapshot de 08/10/2026 sem a lista carregada)

### 📊 Benchmark de Tráfego (SimilarWeb, set/2026)
- **Visitas Mensais Estimadas:** não exibida, mas crescimento de **+520,7%** vs. mês anterior
- **Principal Fonte de Tráfego:** Direct 27,8% (1º), Paid Social (2º), Organic Search (3º)
- **Engajamento:** Bounce 58,9% · 1,69 págs/visita · 1m10s

### 🏆 Top Produtos Escalados
Sem contagem de anúncios. Bestsellers da home:
1. SplashyEyes™ Goggles — https://heywondr.com/products/splashyeyes ($39,99)
2. SplashyEyes™ Goggles (Full Nose Cover) — https://heywondr.com/products/splashynose
3. MagicMani™ Nail Art Pens — https://heywondr.com/products/magicmani
4. TinyTote™ Foldable Tote — https://heywondr.com/products/tinytote
5. FamilyStick™ Retro Game Console — https://heywondr.com/products/familystick

---

## 8. Click Blocks
- **Domínio:** https://click-blocks.com
- **Total de Ads Ativos da Loja:** a busca retorna ~18.000 resultados, mas é ruído (a keyword "click blocks" casa com anúncios de terceiros). Snapshot de 08/10/2026 lista ~15 anúncios da página oficial "Click Blocks" + páginas satélite ("The Playroom Times", "Happy Home Hacks", "Dragons & Dice").

### 📊 Benchmark de Tráfego (SimilarWeb, set/2026)
- **Visitas Mensais Estimadas:** ~62 mil (+28,3% vs. mês anterior). Prostats mostra 8,8 mil visitantes únicos.
- **Principal Fonte de Tráfego:** Display 21,9% (1º), Mail (2º), Direct (3º). 81% das keywords são orgânicas.
- **Engajamento:** Bounce 64,4% · 2,94 págs/visita · 2m07s (o melhor engajamento do grupo)

### 🏆 Top Produtos Escalados
1. **Original Build-A-World Magnets**
   * Anúncios ativos: ≥2 com link visível (mínimo; ~8 anúncios da página oficial usam a copy "The Original Magnetic Building Blocks, Only Available On The Official Click Blocks Website" / "OVER 50% OFF | Hundreds of 5 star reviews")
   * Hook: "Little minds, huge creativity!"; prova social + 50% OFF
   * Link: https://click-blocks.com/products/click-blocks-build-a-world-magnets
2. **Tabletop Gaming 1" Build-A-World Magnets**
   * Anúncios ativos: ≥4 com a copy "Blocks made with DND in mind 🛡️" (via página satélite "Dragons & Dice", iniciados em 08/10/2026); mínimo observado
   * Hook: nicho D&D/tabletop, "For the table, not for kids 🎲"
   * Link: https://click-blocks.com/products/tabletop-blocks
- **Padrão:** rede de páginas satélite dedicadas por nicho (D&D, mães/playroom, home hacks). Estratégia a replicar.
- **Preview:** não capturado.

---

## 9. Wiggo's Toy Factory
- **Domínio:** https://wiggostoyfactory.com
- **Total de Ads Ativos da Loja:** ~70 (snapshot de 20/09/2026; anúncios até 06/10/2026)

### 📊 Benchmark de Tráfego
- **Visitas mensais / fontes:** indisponível (SimilarWeb não tem página indexada para o domínio)

### 🏆 Top Produtos Escalados
Contagens abaixo são **mínimos** (só ~35 dos ~70 anúncios carregaram, e vários não mostram o link). Vários anúncios apontam para **toysandpetsaustralia.com**, loja irmã, o que sugere uma operação multi-loja.
1. **Mega Lifters™ (RC construction machines)**
   * Quantidade de Anúncios Ativos: **≥12** ✅ (passa o filtro)
   * Hook: presente para marido/namorado/avô ("I think I accidentally found the perfect gift for my husband 😂🚜", "Adult Money Well Spent", "Bad news for our warehouse crew… Construction Sale is BACK"), mais Natal ("Santa Approved. Wallet Approved.")
   * Link de Destino: https://wiggostoyfactory.com/products/mega-lifters™ (também via toysandpetsaustralia.com/products/mega-lifters™)
   * Preview: não capturado (anúncios em vídeo de 12 a 29s)
2. **1:64 Scale Remote Tiny Lifters™**
   * Quantidade de Anúncios Ativos: **≥4** ✅ (passa o filtro)
   * Hook: "desk toy" ("The Desk Toy You'll Actually Use", "Terrible For Productivity", "Worst thing I've ever bought…"), "Last Chance 50% off"
   * Link de Destino: https://wiggostoyfactory.com/products/1-64-scale-remote-tiny-lifters™
   * Preview: não capturado

---

## 10. Mini RC Toys
- **Domínio:** https://minirctoys.com
- **Total de Ads Ativos da Loja:** não obtido (Ad Library vazia)

### 📊 Benchmark de Tráfego
- **Visitas mensais / fontes:** indisponível (sem página indexada no SimilarWeb)

### 🏆 Top Produtos Escalados
Sem contagem. Catálogo da home: 12V Electric Wiggle Car ($219), Remote Control Excavator (a partir de $69,90), KART Pro 24V Electric Drift Kart ($409,97), 12V Ride-On Tractor ($349).

---

## Resumo cruzado (anúncios × tráfego)

| Loja | Visitas/mês (SW) | Fonte #1 | Anúncios (obs.) | Observação |
|---|---|---|---|---|
| Toddla | ~266 mil | Paid Social 36,7% | ~1.100 (ruidoso) | Maior tráfego; escala em UGC e creators |
| Click Blocks | ~62 mil | Display 21,9% | ~15 oficiais + satélites | Melhor engajamento; rede de páginas por nicho |
| The Familys Place | ~24 mil | Paid Social 41,9% | n/d | Crescendo +35% |
| Kiddofinds | ~12 mil | Paid Social 29,2% | ~120 | Muito catálogo, pouco anúncio por produto; bounce 83% |
| Wiggo's | n/d | n/d | ~70 | Único com produtos que passam >3 (Mega Lifters ≥12) |
| Stryka | n/d | Paid Social 51,6% | ~34 (2025) | Produto único, bounce 92% |
| Scomeri | 152 (mai/2025) | Direct | ~65 (hoje) | Dado de tráfego velho; loja generalista |
| HeyWondr | n/d | Direct 27,8% | n/d | +520% em tráfego no mês |
| Neefty | 5,5 mil (abr/2025) | Direct | n/d | Sem dados atuais |
| Mini RC Toys | n/d | n/d | n/d | Sem dados |

## Próximas ações sugeridas
1. **Refazer a Fase 1 com a Ad Library API** (ou Apify) fora desta sandbox, agrupando por URL de destino. É o único jeito de fechar o filtro >3 e obter as URLs de thumbnail/vídeo.
2. **Priorizar Wiggo's (Mega Lifters) e Click Blocks (tabletop/D&D)** como os dois sinais mais fortes de escala em produto específico.
3. **Salvar este arquivo no backlog do DASHBOARD.md (AurionOS)** e marcar as 6 lojas sem dados para reextração.
