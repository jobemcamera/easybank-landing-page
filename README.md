# Frontend Mentor - Easybank landing page

## Bem vindo! 👋

Este é um desafio Frontend Mentor!

## O desafio

Meu desafio foi criar esta landing page do EasyBank tentando se aproximar o máximo possível da versão sugerida. Neste projeto utilizei a metodologia Mobile First, onde começo a desenvolver toda a marcação por telas de menor à maior dimensão.

Você pode conferir o desafio na própria página do Frontend Mentor:
[Easybank landing page](https://www.frontendmentor.io/challenges/easybank-landing-page-WaUhkoDN)

## Mobile

![image](https://user-images.githubusercontent.com/109925623/210118312-f01a0fd6-3bb7-4b14-9b9e-60cb40243431.png)

## Desktop

![image](https://user-images.githubusercontent.com/109925623/210118070-a5c5705d-067e-4588-a5d5-fd124cd92b34.png)


### O que eu aprendi

Neste projeto pude me desafiar a manipular imagens sobrepostas, tanto no HTML quanto inseridas diretas no CSS como background-image.

Para a versão Mobile:

```css
.banner__imagens {
    background-image: url('../../img/bg-intro-mobile.svg');
    background-repeat: no-repeat;
    background-position-y: -2.1rem;
    background-size: cover;
    height: 22rem;
    width: 100vw;
}

.banner__imagem {
    display: flex;
    height: 40rem;
    object-fit: contain;
    position: absolute;
    transform: translateY(-13.5rem);
    width: 100vw;
}
```

Para a versão Desktop:

``` css
    .banner__imagens {
        background-image: url('../../img/bg-intro-desktop.svg');
        display: block;
        width: 250%;
        height: 37rem;
        background-position: 17rem -6rem;
        background-repeat: no-repeat; 
    }
    
    .banner__imagem {
        position: absolute;
        width: 50%;
        height: 55rem;
        top: 8rem;
        right: 0;
    }
```

Também aprendi a manipular bordas com linear-gradient para o hover dos links

``` css
    .lista-opcoes__link:hover {
        color: var(--azul-escuro);
    }

    .lista-opcoes__link:hover::before {
        content: '';
        width: 100%;
        height: 5px;
        position: absolute;
        left: 0;
        top: 270%;
        background-image: var(--degrade);
    }
```

