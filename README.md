# Tailwind Playground

## Objetivo

Este repositorio se utiliza para practicar Tailwind CSS de forma organizada.

Permite:

- Desarrollar componentes individuales (cards, navbars, etc.)
- Construir páginas completas (landing pages, dashboards)
- Mantener un entorno limpio y escalable para aprendizaje

La idea es separar cada práctica en su propia carpeta y evitar desorden en la raíz del proyecto.

---

## Estructura del proyecto

```plaintext
tailwind-playground/
│
├── README.md
├── .gitignore
│
├── src/
│   ├── input.css
│   └── output.css
│
├── assets/
│   ├── images/
│   ├── icons/
│   └── fonts/
│
└── projects/
    ├── practica-01-card/
    │   └── index.html
    │
    ├── practica-02-navbar/
    │   └── index.html
    │
    ├── practica-03-landing/
    │   └── index.html
    │
    └── proyecto-real/
        ├── index.html
        ├── pages/
        └── assets/
            └── images/

Atajos rapidos a documentacion oficial: 

1. Crear variables personalizadas:
- Implementacion: https://tailwindcss.com/docs/theme
- Lista de variables predeterminadas: https://tailwindcss.com/docs/theme#default-theme-variable-reference



Importante: cada vez que anbrimos el proyecto nuevamente debemos indicarle a tailwind Importante: npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch mediante la terminal para que lea los estilos, pero una practica recomendada es crear un scripts en package.json para que ejecute automaticamente:

1. Agregar en package.json:
{
.... ,
"scripts": {
  "build:styles": "tailwindcss -i ./src/input.css -o ./src/output.css --watch"
}
}
2. Ejecutar en bash:  npm run build:styles
