# MANUAL
## 1. USANDO O CDN:
Via CDN é a forma mais rápida de começar a usar o Swiper. Você só precisa incluir os links do Swiper diretamente no HTML do seu projeto.  

### ADICIONE OS ARQUIVOS CDN AO SEU HTML:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Swiper - Primeiro Projeto</title>
    <!-- Estilos do Swiper -->
    <link rel="stylesheet" href="https://unpkg.com/swiper/swiper-bundle.min.css">
</head>
<body>
    <!-- Aqui vai o conteúdo -->
    
    <!-- Script do Swiper -->
    <script src="https://unpkg.com/swiper/swiper-bundle.min.js"></script>
</body>
</html>
```


## 2. CRIANDO O PRIMEIRO PROJETO:
### ESTRUTURA BÁSICA NO HTML:
1. Crie um contêiner para o slider (`.swiper`) e defina os slides dentro dele.
2. Inclua classes como `swiper-wrapper` e `swiper-slide` para organizar os elementos.

```html
<div class="swiper">
    <div class="swiper-wrapper">
        <div class="swiper-slide">Slide 1</div>
        <div class="swiper-slide">Slide 2</div>
        <div class="swiper-slide">Slide 3</div>
    </div>
    <!-- Botões de navegação -->
    <div class="swiper-button-next"></div>
    <div class="swiper-button-prev"></div>
    <!-- Paginação -->
    <div class="swiper-pagination"></div>
</div>
```

### ADICIONE O JAVASCRIPT PARA INICIALIZAR O SWIPER:
No script, inicialize o Swiper com opções básicas.  

```html
<script>
    // Inicializando o Swiper
    const swiper = new Swiper('.swiper', {
        // Configurações básicas
        loop: true, // Permite que os slides sejam cíclicos
        navigation: { // Botões de navegação
            nextEl: '.swiper-button-next',
            prevEl: '.swiper-button-prev',
        },
        pagination: { // Paginação
            el: '.swiper-pagination',
            clickable: true,
        },
        autoplay: { // Troca automática
            delay: 3000,
            disableOnInteraction: false,
        },
    });
</script>
```

## 3. CÓDIGO COMPLETO:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Swiper - Primeiro Projeto</title>
    <!-- Estilos do Swiper -->
    <link rel="stylesheet" href="https://unpkg.com/swiper/swiper-bundle.min.css">
    <style>
        /* Estilo adicional para centralizar */
        .swiper {
            width: 80%;
            height: 300px;
            margin: 50px auto;
        }
        .swiper-slide {
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 24px;
            color: white;
            background: #007aff;
        }
    </style>
</head>
<body>
    <!-- Slider -->
    <div class="swiper">
        <div class="swiper-wrapper">
            <div class="swiper-slide">Slide 1</div>
            <div class="swiper-slide">Slide 2</div>
            <div class="swiper-slide">Slide 3</div>
        </div>
        <!-- Botões de navegação -->
        <div class="swiper-button-next"></div>
        <div class="swiper-button-prev"></div>
        <!-- Paginação -->
        <div class="swiper-pagination"></div>
    </div>

    <!-- Script do Swiper -->
    <script src="https://unpkg.com/swiper/swiper-bundle.min.js"></script>
    <script>
        // Inicializando o Swiper
        const swiper = new Swiper('.swiper', {
            loop: true,
            navigation: {
                nextEl: '.swiper-button-next',
                prevEl: '.swiper-button-prev',
            },
            pagination: {
                el: '.swiper-pagination',
                clickable: true,
            },
            autoplay: {
                delay: 3000,
                disableOnInteraction: false,
            },
        });
    </script>
</body>
</html>
```

## 4. TESTANDO O PROJETO:
1. Copie o código completo para um arquivo chamado `index.html`.
2. Abra o arquivo em um navegador.  
3. Você verá o carrossel funcionando com navegação, paginação e autoplay.

