# Terena

Plataforma digital da língua e da cultura Terena, parte da
[Plataforma de Línguas Indígenas](https://plataformas.terradoc.org/). Construída com
[terradoc](https://pypi.org/project/terradoc/).

**Em preparação.** O site começa com a enciclopédia e a bibliografia, a partir de fontes
publicadas; o dicionário, a fauna e as plantas entram com os dados da pesquisa de campo. Por
enquanto ele está só em prévia, no ramo `inicio`:
<https://previews.terradoc.org/terena/inicio/>. Quando a comunidade tiver visto, vai para
`master` e fica em <https://terena.terradoc.org/>.

| O quê | Onde |
|---|---|
| configuração, cores | `terradoc.yaml` |
| textos do site | `locales/pt.yaml`, `locales/en.yaml` |
| enciclopédia | `data/encyclopedia/*.md` |
| bibliografia | `data/references.bib` |
| fotografias | `static/images/` (créditos em `CULTURA.md`) |
| faixa e textura | `config/templates/v2/motifs/terena/` |
| de onde vêm as cores e os desenhos | `CULTURA.md` |

Como mudar algo e como uma mudança chega ao site: o guia em
<https://github.com/plataformasindigenas/terradoc/tree/master/docs/guia>.

```bash
pip install -r requirements.txt
terradoc check -c terradoc.yaml
terradoc build -c terradoc.yaml --out /tmp/terena   # e abra /tmp/terena/index.html
```

O conteúdo é público. Nada restrito ou sagrado entra aqui, e qualquer conteúdo pode ser
retirado a pedido da comunidade.
