# Guia para agentes: site da Impacto Digital

Este repositório **é o site no ar**: https://impactodigitalmga.github.io/ (GitHub Pages, publica a
branch `main` em 1 a 2 minutos). Tudo que entra na `main` vai direto para o público.

- `index.html`: o site inteiro (HTML + CSS + JS). `assets/`: imagens e vídeos.
- Existe uma **cópia** em `giobonifacio-lcach/Midias_carol` (pasta `site/`). Toda mudança feita aqui
  é repetida lá, junto com o registro de origem (`portfolio/<asset>.origem.json`) e o `textos/RESUMO.md`.
  As regras completas de conformidade estão no `CLAUDE.md` daquele repositório e valem aqui.

## Quem decide
- **Carol** (dona da Impacto Digital e do conteúdo) decide o que entra e aprova.
- **Giovane** cuida da coordenação técnica; uma vigia automática avisa ele sobre merges com risco.
  Por isso todo PR diz **o que muda** e **o que pode dar errado**.

## Como falar com a Carol
- Português do Brasil, linguagem simples, respostas curtas (ela usa o celular), uma pergunta por vez,
  com opções numeradas. Mostre prints (largura 390px) em vez de explicar.
- Sem jargão técnico. Diga "coloquei no site", "deixei pronto para você aprovar".
- **Nunca peça para a Carol abrir o GitHub**, a não ser que seja absolutamente inevitável
  (pedido dela, 23/11/2026). Ela aprova **na conversa** e o agente faz o resto: abre o PR e,
  com a aprovação dela por escrito na conversa, faz o merge por ela (registre no PR que o merge
  foi a pedido da Carol). Para mostrar o resultado, mande print do site no ar, não link do GitHub.
- **Falta acesso a algum repositório?** Peça pela ferramenta da sessão (`add_repo`, com `push`
  quando precisar gravar) antes de recorrer à Carol. Só fale com ela se o acesso for negado, e
  diga em palavras simples o que ela (ou o Giovane) precisa liberar.

## Regras do site
1. **Honestidade:** trabalho de exemplo leva o selo "exemplo ilustrativo"; marca inventada é avisada
   como fictícia. Nunca inventar cliente, depoimento ou número de resultado.
2. **Só material próprio ou licenciado e registrado** (origem e licença no `.origem.json` do
   Midias_carol antes do merge). Créditos de CC BY aparecem junto da peça.
3. **Sem pessoas reais reconhecíveis, marcas ou personagens de terceiros.** Imagem de cliente real só
   com autorização do cliente registrada.
4. **Leve no celular:** imagens JPG/WebP até ~200 KB com `loading="lazy"`; vídeos 720x1280 (ou
   540x960), `muted`, `playsinline`, com capa (`poster`) e `preload="none"` ou `"metadata"`.
   Nada de bibliotecas pesadas. Nunca arquivo acima de 50 MB.
5. **Visual:** fonte Inter; cores `--roxo-escuro #2B0B5E`, `--roxo #7A1FA2`, `--rosa #E8336F`,
   `--amarelo #FFC23D`, `--verde #1FAF55`, `--fundo #FFF9F4`; cantos arredondados; botões verdes
   levam para `https://wa.me/5544988069045?text=...` com mensagem pronta. Só esse WhatsApp comercial
   pode aparecer; nada de dados de clientes, tokens ou senhas.

## Como entregar
1. Branch `claude/<tema-curto>` a partir da `main`.
2. Confira no celular (print em 390px) antes de pedir aprovação.
3. PR com **O que muda**, **Origem e licença** e **Riscos** (o que pode dar errado e como desfazer:
   reverter o PR tira do ar em 1 a 2 minutos).
4. A Carol aprova na conversa; o agente faz o merge, espera publicar e manda print do site no ar.
5. Repita a mudança na cópia `site/` do Midias_carol, com o registro de origem e o RESUMO.

QA independente: vale o padrão descrito no `CLAUDE.md` do Midias_carol.
