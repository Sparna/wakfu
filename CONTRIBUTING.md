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
5. O dono do repositório (Sparna) revisa. **Só ele pode fazer o merge na `main`**: a regra em `.github/rulesets/proteger-main.json` bloqueia qualquer outra atualização dela, inclusive de colaboradores.

## Quem pode criar branches aqui

- **Colaboradores** (adicionados em Settings → Collaborators) criam branches direto neste repositório.
- **Qualquer outra pessoa** contribui por fork:
  1. Faça o fork em https://github.com/Sparna/wakfu/fork.
  2. Crie a branch e faça as alterações no seu fork.
  3. Abra o pull request para a `main` deste repositório em https://github.com/Sparna/wakfu/compare (marque "compare across forks").
  4. Acompanhe a revisão em https://github.com/Sparna/wakfu/pulls.

## Sobre o guia

Tudo fica em `wakfu-jornada.html`: os dados das quests (`GL`, `Q`, `RW`, `ITENS`, `EMOTES`) estão no início do `<script>`. As fontes estão listadas na página "Fontes e créditos" do próprio guia.
