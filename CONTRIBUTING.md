# Como contribuir

A branch `main` é protegida: ninguém envia commits direto para ela. Toda mudança entra por uma branch e um pull request.

## Passo a passo

1. Atualize a sua cópia da `main`:
   ```sh
   git switch main
   git pull
   ```
2. Crie uma branch com um nome que diga o que ela muda:
   ```sh
   git switch -c feat/nome-da-mudanca
   ```
   Prefixos usados: `feat/` (novidade), `fix/` (correção), `docs/` (texto), `chore/` (manutenção).
3. Faça as alterações, depois o commit e o push da branch:
   ```sh
   git add .
   git commit -m "feat: descreva a mudança"
   git push -u origin feat/nome-da-mudanca
   ```
4. No GitHub, abra um pull request da sua branch para a `main`.
5. O dono do repositório revisa. Depois da aprovação, o PR é integrado à `main`.

## Quem pode criar branches aqui

- **Colaboradores** (adicionados em Settings → Collaborators) criam branches direto neste repositório.
- **Qualquer outra pessoa** faz um fork, cria a branch no fork e abre o pull request daqui.

## Sobre o guia

Tudo fica em `wakfu-jornada.html`: os dados das quests (`GL`, `Q`, `RW`, `ITENS`, `EMOTES`) estão no início do `<script>`. As fontes estão listadas na página "Fontes e créditos" do próprio guia.
