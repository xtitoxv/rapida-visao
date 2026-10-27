# Rápida Visão — Vistoria Cautelar

Site estático para a empresa Rápida Visão - Vistoria Cautelar, com foco em gerar contatos pelo WhatsApp.

## Pré-visualização

**Link da prévia (GitHub Pages):** https://xtitoxv.github.io/rapida-visao/

## Tecnologias

- HTML5 semântico
- CSS3 (responsivo, mobile-first)
- JavaScript vanilla
- Sem backend, sem dependências externas

## Estrutura do projeto

```
site/
├── index.html      # Página principal
├── style.css       # Estilos
├── app.js          # JavaScript para menu mobile e interações
├── logotipo.jpeg   # Logotipo da empresa
├── ref1.jpeg       # Imagens de referência
├── ref2.jpeg
├── ref3.jpeg
└── README.md
```

## Funcionalidades

- **Responsivo**: Adaptado para celular, tablet e desktop
- **Foco em conversão**: Múltiplos botões para WhatsApp com mensagens pré-definidas
- **Botão flutuante**: WhatsApp sempre visível no celular
- **Navegação suave**: Menu com links âncora
- **SEO básico**: Meta tags e título otimizados
- **Acessibilidade**: Navegação por teclado e semântica HTML

## Editando o site

### Alterar informações

1. **Contato**: Edite o número em `index.html` (procure por `5553997122093`)
2. **Preços**: Altere os valores na seção "Preços e Opções"
3. **Textos**: Modifique diretamente no `index.html`
4. **Cores**: Ajuste as variáveis CSS em `style.css`

### Adicionar imagens

1. Coloque as novas imagens na pasta `site/`
2. Atualize as referências no `index.html`

## Publicação no GitHub Pages

### Opção 1: Usando GitHub CLI (recomendado)

```bash
cd site
git init
git add .
git commit -m "Initial commit - Rápida Visão site"
gh repo create rapida-visao --public --source=. --remote=origin --push
```

Depois, ative o GitHub Pages:
```bash
gh api repos/xtitoxv/rapida-visao/pages -X POST -f source[branch]=main -f source[path]=/
```

### Opção 2: Manualmente

1. Crie o repositório `rapida-visao` na conta `xtitoxv` no GitHub
2. Faça upload de todos os arquivos da pasta `site/` para a raiz do repositório
3. Vá em Settings > Pages
4. Em "Source", selecione "Deploy from a branch"
5. Selecione branch `main` (ou `master`) e pasta `/ (root)`
6. Salve e aguarde o deploy

## Configurar domínio próprio (após aprovação)

Após a aprovação do cliente, para associar `www.rapidavisao.com.br`:

1. **No GitHub Pages:**
   - Settings > Pages > Custom domain
   - Digite: `www.rapidavisao.com.br`
   - Marque "Enforce HTTPS" após verificação

2. **No provedor DNS:**
   - Crie um registro CNAME: `www` apontando para `xtitoxv.github.io`
   - Ou registre A para os IPs do GitHub Pages

3. **Criar arquivo CNAME:**
   - Adicione um arquivo `CNAME` na raiz do repositório com conteúdo: `www.rapidavisao.com.br`

**Importante:** Não configure o domínio agora. Deixe preparado para esta etapa.

## Contato

**Gustavo** - WhatsApp: (53) 99712-2093
**Unidade:** Pelotas - RS
**Empresa:** Rápida Visão — Vistoria Cautelar
