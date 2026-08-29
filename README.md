# Ficha de Custos — Abertura do Salão

Painel para controlar os custos de abertura do salão de beleza: constituição da empresa, licenças, aluguel, reforma, fachada, equipamentos e materiais. Funciona 100% no navegador (sem servidor), guarda os dados automaticamente no seu próprio navegador (localStorage) e tem um botão para imprimir um relatório limpo.

## Como publicar no GitHub Pages (grátis)

1. **Crie um repositório novo** no GitHub (por exemplo `custos-salao`). Pode ser público ou privado (Pages funciona nos dois em contas com Pages habilitado; se ficar em dúvida, deixe público).
2. **Envie o arquivo `index.html`** para a raiz do repositório:
   - Pelo site do GitHub: abra o repositório → *Add file* → *Upload files* → arraste o `index.html` → *Commit changes*.
   - Ou pelo terminal:
     ```bash
     git init
     git add index.html README.md
     git commit -m "Painel de custos do salão"
     git branch -M main
     git remote add origin https://github.com/SEU-USUARIO/custos-salao.git
     git push -u origin main
     ```
3. **Ative o GitHub Pages**: no repositório, vá em *Settings* → *Pages*. Em "Build and deployment", escolha *Source: Deploy from a branch*, selecione a branch `main` e a pasta `/ (root)`. Clique em *Save*.
4. Em 1–2 minutos o site fica disponível em:
   ```
   https://SEU-USUARIO.github.io/custos-salao/
   ```

Pronto — é só abrir esse link sempre que quiser consultar ou atualizar os custos.

## Como usar

- Todos os valores são editáveis: clique em qualquer campo e digite o novo número.
- Cada item tem um tipo: **Único** (gasto de abertura, uma vez só) ou **Mensal** (gasto recorrente).
- Use **"+ Adicionar item"** dentro de qualquer categoria para incluir algo que não está na lista.
- Use **"+ Nova categoria personalizada"** no menu lateral para criar uma categoria inteiramente nova.
- A barra superior mostra sempre: total de investimento inicial, total de custos mensais e o valor total necessário para o primeiro mês de operação.
- **"Restaurar valores de referência"** devolve os valores originais de pesquisa (perde as suas edições — pede confirmação antes).
- **"Imprimir relatório"** abre a janela de impressão do navegador com um layout limpo, sem os botões de edição — ótimo para salvar como PDF ou entregar a um contador/investidor.

## Onde ficam os dados

Os dados ficam salvos **apenas no navegador** em que você os digitou (localStorage), não em nenhum servidor. Isso significa que:
- Ninguém mais vê os seus números — nem o GitHub.
- Se você limpar os dados do navegador, ou abrir o site em outro computador/navegador, ele volta a mostrar os valores de referência.
- Para levar seus dados para outro dispositivo, use o botão **Imprimir → Salvar como PDF** como backup, ou copie os valores manualmente.

## Personalizar

Todo o site é um único arquivo (`index.html`) com HTML, CSS e JavaScript juntos — dá para abrir num editor de texto e ajustar cores, categorias padrão ou textos livremente.
