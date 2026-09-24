# Criador de Vagas — GLP Laboratórios / SCI-AGRO

Ferramenta interna, single-file (HTML + CSS + JS, sem build e sem backend), para montar vagas de emprego, gerar o texto pronto para publicar e exportar a arte de divulgação em JPG (padrão visual SCI-AGRO / GLP Laboratórios).

## Como usar

Basta abrir o `index.html` em qualquer navegador — não precisa de servidor, instalação ou build.

Para publicar via **GitHub Pages**:

1. Suba este repositório no GitHub.
2. Em **Settings → Pages**, selecione a branch `main` e a pasta raiz (`/`).
3. O link ficará algo como `https://<seu-usuario>.github.io/<repositorio>/`.

## Funcionalidades

- Formulário de vaga (cargo, departamento, tipo de contrato, modalidade, horário, faixa salarial, requisitos, atividades, benefícios, contato — com opção de um segundo e-mail/link de contato).
- Toggle entre as duas empresas (SCI-AGRO e GLP Laboratórios), que ajusta automaticamente cidade, logo e benefícios padrão.
- Logos das duas empresas no topo da página.
- Geração de texto pronto para publicar (formato completo e formato para redes sociais, com hashtags).
- Geração e exportação da arte de divulgação em JPG (via html2canvas), no padrão visual da marca, com plano de fundo em padrão gráfico que cobre a arte inteira independentemente do tamanho do texto da vaga.
- Lista de vagas salvas, com busca e filtros por empresa, departamento e status (aberta/fechada).
- Dados salvos no `localStorage` do navegador (não há backend — cada navegador guarda as suas próprias vagas).

## Stack

- HTML, CSS e JavaScript puro, tudo em um único arquivo (`index.html`).
- [html2canvas](https://html2canvas.hertzen.com/) (via CDN) para exportar a arte da vaga como imagem.
- Fonte [Poppins](https://fonts.google.com/specimen/Poppins) (Google Fonts, via CDN).

## Limitações conhecidas

- Sem login e sem dados compartilhados entre usuários — cada pessoa que abre a ferramenta em um navegador diferente vê apenas as vagas que ela mesma salvou ali.
- Não há backend/banco de dados; tudo roda no navegador.
