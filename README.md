# Oh My Cookie · ohmycookie.pt

Página estática (HTML + imagens), pronta para o GitHub Pages.

## Pôr online
1. Cria um repositório no GitHub (ex.: `ohmycookie-site`) e envia todo o conteúdo desta pasta (incluindo `CNAME` e `img/`).
2. No repositório: **Settings → Pages → Source: Deploy from a branch → main / (root)**.
3. No painel onde compraste o domínio (DNS de ohmycookie.pt):
   - 4 registos **A** para `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - 1 registo **CNAME** para `www` → `O-TEU-UTILIZADOR.github.io`
4. Volta a **Settings → Pages**, confirma o domínio `ohmycookie.pt` e ativa **Enforce HTTPS** (pode demorar até algumas horas).

## Editar
Tudo está no `index.html`:
- **Preços, contactos, portes, mínimo:** bloco `CONFIG` no início do `<script>`.
- **Sabores:** lista `FLAVOURS` (um sabor com preço diferente leva `price: 2.90`). A foto é `img/<id>.webp` (452×300).
- **Textos PT/EN:** objeto `T` (`pt` e `en`). Um sabor sazonal novo precisa de `desc.<id>` nos dois idiomas.
