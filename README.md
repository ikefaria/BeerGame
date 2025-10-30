# Beer Game — Simulador de Cadeia de Suprimentos

Este projeto é uma versão em navegador do **Beer Game**, um jogo clássico usado em cursos de logística, supply chain e gestão de operações. Foi criado em HTML, CSS e JavaScript puro, sem necessidade de instalação ou servidor.

---

## 🎯 Objetivo
Simular o comportamento de uma cadeia de suprimentos (Varejista → Atacadista → Distribuidor → Fábrica), demonstrando o **efeito chicote (bullwhip effect)** que surge quando há variações e atrasos nas informações e pedidos.

---

## 🚀 Como jogar (localmente)
1. Baixe o arquivo [`index.html`](./index.html).
2. Abra o arquivo diretamente no seu navegador (Chrome, Edge, Firefox...).
3. Configure o jogo:
   - **Semanas:** número total de rodadas (ex.: 30)
   - **Lead Time:** tempo de reposição (ex.: 2)
   - **Demanda inicial:** unidades pedidas por semana (ex.: 4)
4. Clique em **Iniciar**.
5. Para cada rodada, ajuste os **pedidos** de cada papel e clique em **Próxima Semana**.
6. Acompanhe o gráfico de estoques e o log de eventos.
7. Use **Exportar CSV** para baixar o histórico e analisar os resultados.

---

## 🧩 Papéis da cadeia
- **Varejista:** atende a demanda do cliente final.
- **Atacadista:** repõe o varejista.
- **Distribuidor:** abastece o atacadista.
- **Fábrica:** produz e envia ao distribuidor.

Cada papel deve equilibrar seu **estoque** e evitar **atrasos (backorders)**. O desafio é coordenar toda a cadeia.

---

## 📈 Métricas e aprendizagem
- **Efeito chicote:** observe como pequenas variações na demanda amplificam os pedidos ao longo da cadeia.
- **Estoque x backorder:** o equilíbrio entre falta e excesso de produtos.
- **Custo total:** pode ser calculado no CSV exportado (estoque * custo de armazenagem + backorder * custo de atraso).

---

## 🌐 Publicar no GitHub Pages
1. Crie um repositório no GitHub (ex.: `beer-game`).
2. Faça upload do arquivo `index.html` (e opcionalmente este README.md).
3. Vá em **Settings → Pages**.
4. Em **Source**, escolha `Deploy from a branch` e selecione `main` e a pasta raiz (`/`).
5. Clique em **Save**.
6. Após alguns segundos, seu app estará disponível em:
   ```
   https://ikefaria.github.io/BeerGame/
   ```

---

## 💡 Próximos aprimoramentos
- Multiplayer em tempo real (WebSocket / Firebase)
- Modo automático com diferentes políticas de pedido
- Cálculo de custos semanais e KPI de variação
- Cenários pré-programados para sala de aula

---

**Autor:** Carlos Henrique Faria  
**Licença:** MIT  
**Tecnologias:** HTML5 + JavaScript + Chart.js
