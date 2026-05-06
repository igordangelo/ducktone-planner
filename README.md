# DuckTone Board Planner

Planejador de pedalboard com gerador de orçamento integrado.

## Estrutura do projeto

```
ducktone-planner/
├── index.html              ← App principal
├── data/
│   ├── pedals.json         ← Base de 8221 pedais (PedalPlayground)
│   └── pedalboards.json    ← Base de 245 boards (PedalPlayground)
├── assets/
│   ├── logo-gold.png       ← Logo DuckTone (fundo escuro)
│   └── logo-dark.png       ← Logo DuckTone (fundo claro)
└── public/
    └── images/
        ├── pedals/         ← PNGs dos pedais (copiar do PedalPlayground)
        └── pedalboards/    ← PNGs dos boards (copiar do PedalPlayground)
```

## Como usar localmente

1. Copie a pasta `public/images/` do PedalPlayground para dentro deste projeto
2. Abra `index.html` num servidor local (ex: `python -m http.server`)
3. Nunca abra diretamente como `file://` — o fetch dos JSONs não funciona assim

## Como publicar no GitHub Pages

1. Crie um repositório no GitHub: `ducktone-planner`
2. Faça upload de todos os arquivos desta pasta
3. Vá em **Settings → Pages → Source: main branch**
4. Acesse via `https://seuusuario.github.io/ducktone-planner`

## Funcionalidades

- Biblioteca de 8221 pedais com busca por nome e marca
- 245 boards de marcas reais + board personalizado por dimensão
- Drag & drop com containment no board
- Rotação de pedais (R ou botão)
- Signal chain visual com conexões SVG (clique e arraste de porta a porta)
- Cálculo automático do comprimento de cada cabo patch
- Painel de orçamento com tabela de preços interna (não visível ao cliente)
- PDF com layout + cadeia de sinal + lista de pedais + orçamento detalhado
- Bilíngue: PT-BR / EN

## Built for DuckTone Custom Boards
