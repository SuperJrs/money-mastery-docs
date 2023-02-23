# Políticas de Branchs

Padronização das branches no projeto. 

## 1. Introdução

Esse documento tem como objetivo padronizar a nomenclatura e uso de branchs no repositório. Como base foi utilizado o modelo de branchs do gitflow como mostrado na imagem a seguir.


## 2. Formato das Branchs

### 2.1. Prefixos

- ```main```
- ```test```
- ```refact```
- ```bugfix```
- ```develop```
- ```feature```

### 2.2. Nomeclatura

```
<prefixo>/#numero_da_issue
```

Exemplo: 
```
feature/#22
```

## 3. Branches

Esse repositório trabalhará com quatro tipos de branchs: main, bugfix, develop e feature.

- **Branch main:** É a branch que contém código em nível de produção, ou seja, o código mais maduro existente na aplicação. Todo o código novo produzido eventualmente é juntado com a branch main, em algum momento do desenvolvimento;
- **Branches bugfix:** São branches no qual são realizadas correções de bugs críticos encontrados em ambiente de produção, e que por isso são criadas a partir da branch main, e são juntadas diretamente com a branch main e com a branch develop, se estiver alguma ativa (pois os próximos deploys também devem receber correções de bugs críticos). Por convenção, essas branches tem o nome começando com bugfix/ e terminando com o próximo sub-número de versão (exemplo: bugfix/2.31.1);
- **Branch develop:** É a branch que contém código em nível preparatório para o próximo deploy. Ou seja, quando features são terminadas, elas são juntadas com a branch develop, testadas (em conjunto, no caso de mais de uma feature), e somente depois as atualizações da branch develop passam pela fase de homologação e, se aprovadas, são juntadas com a branch main para produção. Sempre que uma correção for feita (bugfix) essa branch deverá ser atualizada;
- **Branches feature:** São branches no qual são desenvolvidos recursos novos para o projeto em questão. Essas branches tem por convenção nome começando com feature/issue-description (exemplo: feature/#54) e são criadas a partir da branch develop (pois um recurso pode depender diretamente de outro recurso em algumas situações), e, ao final, são juntadas com a branch develop.
- **Branch test:** É a branch utilizada para realizar os testes (exemplo: test/#50).
- **Branch refact:** Branch destinada para realizar refatorações em um determinado código (exemplo: refact/#11).


## 4. Princípios:

- As branches de bugfix e feature devem possuir uma issue.


## 5. Histórico de versões

| Data       | Versão | Descrição                      | Autor(es)                                                                                                                                                  |
| :--------: | :----: | ------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 22/02/2023 |  1.0   | Criação da política de branch  | [Daniel Viana](https://github.com/danielvimot), [Lameque Fernandes](https://github.com/lamequefernandes), e [Oziel Humasi](https://github.com/ozielhumasi) |
