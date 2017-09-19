# Css

### Como pasar un archivo **SASS** o **SCSS** a **CSS**

1. Entrar al siguinte link: [sassmeister](https://www.sassmeister.com/)
2. Copiar el codigo **sass** o **scss** y automáticamente se transcribe a **CSS**   

Código de ejemplo SCSS:
```scss
body{
    font-family: sans-serif;
}

.er-modal{
    position: fixed;
    width: 100%;
    height: 100%;
    left: 0;
    top: 0;
    background: rgba(#000, .9);
    display: flex;
}

.er-closeModal{
    position: absolute;
    top: 1em;
    right: 1em;
    cursor: pointer;
    width: 1.5rem;
    height: 1.5rem;
    opacity: .5;


    &::before,
    &::after {
        content: "";
        width: 2.12rem;
        height: 2px;
        background: #fff;
        position: absolute;
        top: 0;
        transform: rotate(45deg);
        transform-origin: top left;
    }

    &::before{
        left: 0;
    }

    &::after{
        right: 0;
        transform: rotate(-45deg);
        transform-origin: top right;
    }
}

.modalContent {
    width: 90%;
    max-width: 1000px;
    margin: auto;
}

.video{
    width: 100%;
    position: relative;
    height: 0;
    padding-bottom: 56.25%;
    overflow: hidden;

    iframe {
        width: 100%;
        position: absolute;
        top: 0;
        left: 0;
        height: 100%;
    }
}
```
