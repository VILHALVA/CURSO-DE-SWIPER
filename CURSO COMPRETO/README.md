# CARRUSEL DE CARDS CON SWIPER JS
Este projeto é um **carrossel de cards responsivo** utilizando o **SwiperJS**, onde cada slide exibe informações visuais e textuais organizadas em um formato de card. Vamos analisar os componentes e o funcionamento:

## 1. ESTRUTURA DO PROJETO:
### HTML:
1. **Estrutura principal do SwiperJS**:
   - `swiper-container`: Contêiner principal do carrossel.
   - `swiper-wrapper`: Elemento que agrupa os slides.
   - `swiper-slide`: Cada slide dentro do carrossel.
2. **Conteúdo de cada slide**:
   - Imagens (`img`) com textos descritivos e um link interativo (`Ver más`).
   - Cada card contém títulos (`card-title`), descrições (`card-text`) e botões (`card-link`).
3. **Navegação**:
   - Botões para avançar e retroceder (`swiper-button-next` e `swiper-button-prev`).
   - Paginação configurada para mostrar indicadores de progresso.

### 2. ESTILIZAÇÃO (CSS):
1. **Layout geral**:
   - O corpo (`body`) é centralizado vertical e horizontalmente com `flexbox`.
   - O contêiner principal (`container`) usa um design responsivo com padding para ajustar o espaço.
2. **Estilização dos slides**:
   - Os cards têm bordas arredondadas, sombra para destacar os elementos e um fundo branco.
   - As imagens no topo de cada card são ajustadas com `object-fit: cover` para manter o aspecto visual.
3. **Navegação personalizada**:
   - Os botões de navegação são reposicionados com `right` e `left`.
4. **Responsividade**:
   - O layout é ajustado para diferentes larguras de tela usando *breakpoints* no CSS e no JavaScript.

### 3. CONFIGURAÇÃO DO SWIPERJS (JAVASCRIPT):
O script configura e inicializa o SwiperJS com as seguintes funcionalidades:
1. **Navegação**:
   - `navigation`: Configura os botões de navegação (`nextEl` e `prevEl`).
2. **Slides por visualização**:
   - `slidesPerView`: Determina quantos slides são exibidos ao mesmo tempo.
   - `spaceBetween`: Define o espaço entre os slides.
3. **Paginação**:
   - `pagination`: Adiciona um controle clicável abaixo do carrossel.
4. **Breakpoints**:
   - Ajusta o número de slides exibidos com base na largura da tela:
     - **620px**: 1 slide por vez.
     - **680px**: 2 slides.
     - **920px**: 3 slides.
     - **1240px**: 4 slides.
5. **Responsividade inteligente**:
   - As configurações de `breakpoints` tornam o carrossel altamente adaptável a diferentes dispositivos.

## 4. PRINCIPAIS CARACTERÍSTICAS:
1. **Design Responsivo**:
   - O carrossel ajusta a exibição automaticamente conforme a largura da tela.
2. **Experiência de Usuário Suave**:
   - Navegação intuitiva com botões e paginação.
   - Desempenho otimizado por SwiperJS.
3. **Apresentação de Cards**:
   - Ideal para mostrar informações organizadas, como produtos ou galerias de fotos.
4. **Customização Fácil**:
   - CSS simples e modular para estilizar o carrossel.

## 5. COMO FUNCIONA?
- Quando o usuário acessa a página, o SwiperJS inicializa e cria o carrossel com base na estrutura do HTML.
- A navegação pode ser feita clicando nos botões ou nos indicadores de paginação.
- O layout dos slides muda automaticamente dependendo do tamanho da tela graças aos *breakpoints*.
