# Branches dos alunos

Este repositório tem uma branch remota por aluno. Cada branch é um espaço de trabalho separado; antes de começar, confirme que está na branch correspondente ao seu nome.

## Como acessar uma branch

No terminal, dentro do clone do repositório, atualize a lista de branches remotas:

```bash
git fetch origin
```

Na primeira vez, crie uma branch local ligada à branch remota desejada. Substitua `NOME_DA_BRANCH` pelo nome da tabela:

```bash
git switch --track origin/NOME_DA_BRANCH
```

Exemplo para Julia:

```bash
git switch --track origin/julia_christina
```

Se a branch local já existir, basta alternar para ela:

```bash
git switch NOME_DA_BRANCH
```

Confira a branch ativa antes de editar ou fazer commits:

```bash
git branch --show-current
```

Depois de trabalhar, salve e envie suas alterações para a branch correspondente:

```bash
git add .
git commit -m "Descreva suas alterações"
git push
```

Não faça o trabalho de um aluno na branch de outra pessoa. Para integrar as alterações ao `main`, abra um pull request da branch do aluno para `main` e aguarde a revisão/integração.

## Alunos e branches

| Aluno | Branch |
|---|---|
| Julia Christina Cortes Ara jo | `julia_christina` |
| Karin Garcia Aguado | `karin_garcia` |
| Kelly Fumika Hatada | `kelly_fumika` |
| Kleber Barbosa Teodoro | `kleber_barbosa` |
| Lilian Akemi Harada | `lilian_akemi` |
| Luana Francisca De Sousa Monteles | `luana_francisca` |
| Luiz Augusto Gon alves Sim es | `luiz_augusto` |
| Marcio Augusto De Souza Camara | `marcio_augusto` |
| Marcio Ricardo De Carvalho Santos | `marcio_ricardo` |
| Matias Schorr | `matias_schorr` |
| Mileidy Silva Pereira Da Rocha | `mileidy_silva` |
| Paulo Cesar Pereira Brito | `paulo_cesar` |
| Priscila Danúbia De Melo | `priscila_danubia` |
| Renata Cristina Patricio De Oliveira | `renata_cristina` |
| Silvana De Melo Perbelini | `silvana_de` |
| Soraia Moreira Vasconcelos | `soraia_moreira` |
| Vagner Santos Lour do | `vagner_santos` |
| Vanessa Maria Borges Da Silva | `vanessa_maria` |
| Walkiria Franco Lima | `walkiria_franco` |