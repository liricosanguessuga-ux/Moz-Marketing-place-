# Moz Marketing Place

Site de compra e venda de produtos e serviços em Moçambique.

## Como publicar este site (passo a passo)

### 1. Enviar para o GitHub
1. Crie uma conta gratuita em https://github.com (se ainda não tiver)
2. Clique em **"New repository"**, dê o nome `moz-marketing-place` e crie (pode deixar como "Public")
3. Na página do repositório vazio, clique em **"uploading an existing file"**
4. Arraste **toda esta pasta** (`moz-marketing-place`) para a janela do navegador
5. Clique em **"Commit changes"** para enviar

### 2. Publicar na Vercel
1. Crie uma conta gratuita em https://vercel.com, entrando com **"Continue with GitHub"**
2. Clique em **"Add New" → "Project"**
3. Escolha o repositório `moz-marketing-place` e clique em **"Import"**
4. Deixe as configurações como estão e clique em **"Deploy"**
5. Em cerca de 1 minuto, a Vercel entrega um link, algo como:
   `https://moz-marketing-place.vercel.app`

O site já estará no ar e acessível a qualquer pessoa com esse link.

## Limitação atual (Fase 1)

Os anúncios, comentários e avaliações ficam guardados **apenas no navegador de cada visitante** (localStorage). Ou seja, se você publicar um anúncio no seu telemóvel, outra pessoa que abra o link no computador dela não vai ver esse anúncio.

Isto é temporário — serve para já ter o site real, no ar, com o design e a funcionalidade completos para testar.

## Próximo passo (Fase 2): dados partilhados de verdade

Para que todos os utilizadores vejam os mesmos anúncios, comentários e avaliações, é preciso ligar uma base de dados real. A opção mais simples e gratuita para começar é o **Supabase** (supabase.com), que fornece:
- Base de dados partilhada
- Autenticação de utilizadores real (com confirmação por email)
- Armazenamento de imagens (para fotos dos produtos)

Quando estiver pronto para essa fase, é só pedir — o código já está estruturado para essa troca ser direta (só a parte de `storage` no ficheiro `components/MozMarketPlace.jsx` precisa de ser trocada por chamadas ao Supabase).

## Rodar localmente (opcional, para quem tiver Node.js instalado)

```bash
npm install
npm run dev
```

Depois abra http://localhost:3000
