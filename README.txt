SITE DE ESTUDOS — HSK2 / Mandarim Básico 2 (Lições 1–8)
========================================================

CONTEÚDO DA PASTA
-----------------
  index.html            → Guia de estudos (gramática, vocabulário,
                          simulado interativo, redação, oral, dicas)
  treino-audicao.html   → Treino de audição (áudio em mandarim + questões)
  README.txt            → este arquivo

As duas páginas se conectam por links (o menu do guia tem "🎧 Treino de
audição"; o treino tem "← Voltar ao guia"). São arquivos 100% estáticos:
todo o CSS e o JavaScript estão embutidos, sem dependências externas.
Nada de servidor de aplicação, banco de dados ou build — é só HTML.


COMO SUBIR EM UM SERVIDOR WEB
-----------------------------
Basta enviar os dois arquivos .html para a pasta pública do servidor.
O arquivo "index.html" abre automaticamente ao acessar o endereço.

Opções fáceis (todas gratuitas):

  • GitHub Pages
      1. Crie um repositório e envie index.html e treino-audicao.html.
      2. Settings → Pages → Branch: main → Save.
      3. O site fica em https://SEU-USUARIO.github.io/NOME-DO-REPO/

  • Netlify  (netlify.com)  ou  Cloudflare Pages
      1. Arraste a pasta "site-hsk2" inteira para a área de deploy.
      2. Pronto — ele gera um endereço público na hora.

  • Hospedagem tradicional (cPanel / FTP)
      1. Envie os dois .html para a pasta "public_html" (ou "www").

  • Testar no seu PC sem internet
      Só abrir o index.html com duplo clique no navegador já funciona.
      (Opcional, via terminal na pasta:  python -m http.server 8000
       e acessar http://localhost:8000 )


OBSERVAÇÃO SOBRE O ÁUDIO
------------------------
O treino de audição usa a voz em chinês do próprio navegador (Web Speech
API). Funciona offline, mas depende de ter uma voz "Chinês (China)"
instalada no sistema:
  Windows 11 → Configurações → Hora e idioma → Idioma e região →
  Adicionar idioma → "中文 (中国) / Chinês (China)".
A própria página avisa no topo se encontrou a voz.
