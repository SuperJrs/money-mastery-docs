# Políticas de Commit

Padronização dos commits no projeto. 

## 1. Introdução

Esse documento tem como objetivo padronizar a nomenclatura e uso de commits no repositório.


## 2. Semântica do Commit

### 2.1 Princípios:

#### 2.1.1 Commits atômicos

Sempre dividir em pequenos commits, para melhor manutenção e rastreamento.

#### 2.1.2 Commits em português

Foi decidido que todos os commits serão em pt-BR.

### 2.2 Formato:
```
<tipo>: assunto. <#número da issue>
```

#### 2.2.1 Tipos:

- ```feat```: nova funcionalidade
- ```docs```: referente a documentação
- ```test```: relacionado a testes 
- ```fix```: correções
- ```refact```: relacionado a refatoração de código

#### 2.2.2 Assunto:

- Deve possuir até 72 caracteres
- Deve haver apenas letras minúsculas

*Exemplo de commit:*
```
git commit -m "feat: adicao de botao no menu principal. #33"
```

## Histórico de versões

| Data       | Versão | Descrição                      | Autor(es)                                                                                                                                                  |
| :--------: | :----: | ------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 22/02/2023 |  1.0   | Criação da política de commits | [Daniel Viana](https://github.com/danielvimot), [Lameque Fernandes](https://github.com/lamequefernandes), e [Oziel Humasi](https://github.com/ozielhumasi) |
