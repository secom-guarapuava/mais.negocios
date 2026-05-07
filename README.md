# Guarapuava Mais Negócios — Landing Page

Página informativa e estática sobre o programa **Guarapuava Mais Negócios**, de credenciamento da Prefeitura de Guarapuava, criada para organizar e apresentar as informações do programa ao público.

> Esta é uma página **informativa, não oficial e não vinculada à Prefeitura de Guarapuava**. Foi feita como apoio à comunicação do programa. Todo o conteúdo é baseado em informações públicas oficiais.

---

## Sobre o projeto

- **Tipo:** Site estático single-file (apenas `index.html`)
- **Stack:** HTML + Tailwind CSS (via CDN) + AOS (animações) + Lucide Icons
- **Sem backend.** Todos os botões de ação levam ao WhatsApp do Escritório de Compras com mensagem pré-preenchida.
- **Responsivo / mobile-first**, otimizado para acessos via celular.

## Estrutura da página

1. Header fixo com navegação
2. Hero com logo (cata-vento) animado
3. Tagline em marquee
4. Estatísticas do programa
5. Bloco "O Programa"
6. Como funciona (4 passos)
7. Editais abertos (cards com prazos)
8. Áreas de manutenção (accordion expansível)
9. Quem pode participar (MEI / ME / EPP)
10. FAQ (accordion)
11. CTA final
12. Footer
13. Botão flutuante de WhatsApp

## Como visualizar localmente

Basta abrir o `index.html` no navegador — não precisa de build, servidor ou instalação de nada.

```bash
# opcional, se quiser servir local com Python
python3 -m http.server 8000
# depois acesse http://localhost:8000
```

## Como publicar no GitHub Pages

1. Crie um repositório novo no GitHub (público ou privado, seu critério).
2. Faça commit do `index.html` (e deste `README.md`) na raiz do repo.
3. No repositório, vá em **Settings → Pages**.
4. Em **Source**, selecione a branch (`main`) e a pasta (`/root`).
5. Salve. O GitHub vai gerar a URL `https://SEU-USUARIO.github.io/NOME-DO-REPO/`.

Pronto. Sem build, sem CI, sem dor de cabeça.

## Como editar conteúdo

Tudo está num único arquivo (`index.html`). Para alterações comuns:

- **Textos:** edite direto no HTML — cada seção está marcada com comentários `<!-- ================= NOME ================= -->`.
- **Editais:** procure por `<!-- ================= EDITAIS ABERTOS =================` e duplique/edite os blocos `<article class="gradient-card …">`.
- **FAQ:** procure por `<!-- ================= FAQ =================` e edite os blocos `<details>`.
- **Cores da marca:** estão definidas no `tailwind.config` no `<head>` e nas variáveis CSS `:root`.
- **Número do WhatsApp:** todos os links seguem o formato `https://wa.me/554231421846?text=...`. Para trocar, faça find/replace de `554231421846` no arquivo.

## Identidade visual

- **Navy:** `#0E1F4A` — base institucional
- **Coral:** `#E94E2B` — destaque principal, CTAs
- **Royal:** `#2154B5` — apoio
- **Lime:** `#DCE43E` — energia, highlights
- **Tipografia:** Sora (display) + Plus Jakarta Sans (corpo) — Google Fonts

## Contato do programa (atendimento real)

- **Telefone / WhatsApp:** (42) 3142-1846
- **Local:** Escritório de Compras — Paço Municipal de Guarapuava

## Licença / uso

Página informativa de apoio. Os textos e a identidade visual referentes ao programa pertencem aos seus respectivos titulares (Prefeitura de Guarapuava e o programa Guarapuava Mais Negócios).
