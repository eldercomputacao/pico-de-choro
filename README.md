# Simulador do Pico de Choro do Bebê

Ferramenta educativa que calcula e exibe graficamente o **Período PURPLE** — a fase de choro mais intensa em bebês saudáveis de 0 a 4 meses. Suporta bebês prematuros com cálculo automático por idade corrigida.

Acesse em: [picodechorobebe.com.br](https://picodechorobebe.com.br)

## Funcionalidades

- Cálculo das datas-chave do Período PURPLE a partir da data de nascimento e semanas de gestação
- Gráfico interativo de intensidade de choro semana a semana (Chart.js)
- Barra de progresso com a fase atual (escalada, pico, declínio ou encerrado)
- Suporte a bebês prematuros via idade corrigida
- FAQ com 9 perguntas com rich results para o Google (Schema FAQPage)
- PWA: pode ser instalado na tela inicial do celular (Android e iOS)

## Estrutura do projeto

```
├── index.html        # Página principal
├── manifest.json     # PWA manifest
├── robots.txt        # Diretivas para crawlers
├── sitemap.xml       # Mapa do site
├── css/
│   └── style.css     # Estilos e design system
├── js/
│   └── script.js     # Lógica de cálculo e geração do gráfico
└── assets/
    ├── favicon.svg
    ├── social-card.png
    ├── icon-192.png
    ├── icon-512.png
    └── apple-touch-icon.png
```

## Executar localmente

Sem build step — basta servir os arquivos estáticos:

```bash
# Python (nativo)
python3 -m http.server 8080

# Node.js
npx serve .
```

Acesse `http://localhost:8080` no navegador.

## Baseado em

Modelo **Período PURPLE** — Dr. Ronald Barr, SickKids Hospital.  
Ferramenta educativa — não substitui orientação médica profissional.
