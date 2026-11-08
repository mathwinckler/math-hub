# matheuswinckler.com.br

Site pessoal de Matheus Winckler. Estático, sem build: HTML e CSS puros, publicados como estão
pelo GitHub Pages (branch `main`, raiz; domínio no `CNAME`).

| caminho | o que é | estado |
|---|---|---|
| `/` | página principal. Hoje provisória ("em construção"), com hub e agendar | provisória |
| `/hub/` | links da bio do Instagram: consulta, Café Exponencial, MovMente Cast, fundo do baú (Reconec.Estado) | no ar |
| `/404.html` | página não encontrada, leva ao hub (caminhos absolutos de propósito) | pronta |
| `assets/css/base.css` | vocabulário visual "rota" (fontes, cores, título, botões, links) | base |
| `assets/img/` | foto de perfil (a mesma do Instagram) e favicon | base |

## Como cresce

- **Página nova** vira pasta com `index.html` (`/sobre/`, `/palestras/`...) e importa
  `../assets/css/base.css`; o estilo próprio fica no `<style>` dela.
- **O site principal** substitui o `index.html` da raiz. O `/hub/` não muda de endereço: é o link da bio.
- Caminhos relativos, exceto no `404.html`.
- A seção **04 · Convites e parcerias** está pronta e comentada no `hub/index.html`: liga quando o email existir.
- A identidade visual mora no mdw-em-rota (`producao-de-conteudo/instagram/visual/modos/rota.css`).
  Este repositório aplica, não define.

## Ver localmente

    python3 -m http.server 8788

e abrir `http://127.0.0.1:8788/` e `http://127.0.0.1:8788/hub/`.
