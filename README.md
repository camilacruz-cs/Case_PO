# Case - Nível de Prontidão dos POs

## Contexto & Problema:

- O banco está em processo de transformação digital e com isso vem a necessidade de trabalharmos em um novo modelo para garantir mais agilidade nas entregas de valor.
O modelo proposto é o modelo de comunidade, onde agrupamos os colaboradores, com diferentes especialidades, em squads e com mesmo objetivo
A squad é formada por: 1 PO, 1 TechLead, 1 TeamLead e alguns TeamMembers

- Para cada um dos papeis e especialidades, existem skills que são:
Gerais, ou seja, independem da especialidade - [Problem solving], [Atitude de dono], [Poder de influência], [Mindset lean e ágil], [Product discovery]
Específicas, ou seja, o nível de necessidade muda conforme a especialidade - [Contexto estratégico], [Produto como plataforma], [Negócio e indústria], [P&L], [Dados]

## Sobre os dados:

- A aba BaseAvaliacao contém as notas para cada uma das skills, e é importante observar que muitos colaboradores possuem duas avaliações: [Funcional] e [Matricial].

- Sendo a avaliação funcional, referente a avaliação que o gestor direto do colaborador realizou. Ele tem mais insumos históricos, tanto de entrega quanto comportamental e é obrigatório ter realizado o mapeamento.

- A avaliação matricial é referente a avaliação que o gestor que acompanha a atividade e é opcional.

- Na tabela NivelNecessidadePo temos uma nota de nível esperado para considerar o PO apto para aquela skill.

## Precisamos entender: 
  1. Nossos POs estão aptos a exercer seus papeis?

  2. Quais são as skills que deveríamos propor treinamentos para nossos POs? Qual seria o primeiro treinamento?


## Passos na Análise de Dados:
<img width="573" alt="image" src="https://github.com/user-attachments/assets/3ac76035-bc83-4115-837e-128a4a89c38c">

## Ferramentas utilizadas:
As ferramentas utilizadas neste projeto são:

* <b>Excel: ferramenta utilizada para toda a limpeza da base.<br>
1. Limpeza da base.
![image](https://github.com/user-attachments/assets/9c977f0f-7a92-44f3-b9c6-09633280321a)
 - Considerando que nós só precisamos dos POs, os outros cargos foram desconsiderados nesta análise;
 - Na análise, estou considerando tanto as avaliações matricial e também funcional. 

2. Análise por Skills necessária
![image](https://github.com/user-attachments/assets/0881bb10-6e25-43d7-88a1-47a6377b9bc4)

 - Sabendo que cada skill necessária possui uma nota, fiz uma formula que traz se aquele PO está ou não está apto para aquele cargo considerando aquela skill necessária.

Exemplo do que foi feito para todos os colaboradores avaliados:

| Nome do colaborador avaliado | Tipo de gestão | ESPECIALIDADE_avaliado | [Contexto estratégico] | [Problem solving] | [Atitude de dono] | [Poder de influência] | [Produto como plataforma] | [Mindset lean e ágil] | [Product discovery] | [Negócio e indústria] | [P&L] | [Dados] | [Contexto estratégico_necessidade] | [Problem solving_necessidade] | [Atitude de dono_necessidade] | [Poder de influência_necessidade] | [Produto como plataforma_necessidade] | [Mindset lean e ágil_necessidade] | [Product discovery_necessidade] | [Negócio e indústria_necessidade] | [P&L_necessidade] | [Dados_necessidade] |
| ----------------------------- | -------------- | ---------------------- | ----------------------- | ------------------ | ----------------- | ---------------------- | -------------------------- | --------------------- | -------------------- | --------------------- | ------- | ------ | ------------------------------- | -------------------------- | -------------------------- | -------------------------- | -------------------------------- | ----------------------------- | -------------------------- | ---------------------------- | -------------------- | ------------------- |
| COLABORADOR061               | Funcional       | PRODUTO                 | 3                        | 4                   | 2                  | 3                        | 3                           | 3                      | 3                     | 3                      | 2       |        | Está apto                        | Está apto                  | TREINAMENTO                  | Está apto                    | Está apto                          | Está apto                       | Está apto                    | Está apto                      | Está apto             | TREINAMENTO            |

Fórmula utilizada para chegar neste resultado:

> =SE(C3="PRODUTO"; SE(H3<2; "TREINAMENTO"; "Está apto"); SE(C3="OPERAÇÕES"; SE(H3<2; "TREINAMENTO"; "Está apto"); SE(C3="AQ DIGITAL"; SE(H3<2; "TREINAMENTO"; "Está apto"); SE(C3="CRÉDITO"; SE(H3<3; "TREINAMENTO"; "Está apto"); "Atividade não reconhecida"))))

## Resultados:

![image](https://github.com/user-attachments/assets/1f9bde00-f1c0-42f7-bf31-8cc9d6b0fb47)

- Considerando os 79 colaboradores avaliados, para o critério de "Contexto estratégico", apenas 45 colaboradores estão aptos e não irão necessitar de um treinamento.

  > Fiz essa comparação para todos os colaboradores, chegando a conclusão de que para o critério de "Contexto Estratégico", por exemplo, do universo de pessoas avaliadas 56,96% está apto, em contraponto com 43% não apto e que precisará de treinamento nesta frente.

![image](https://github.com/user-attachments/assets/f76a8857-3ffb-46df-afb2-74171abf5b49)

- Considerando todos que precisam de treinamento nos critérios avaliados, cheguei a conclusão que:
  - Dados (64%) possui um grande número de pessoas com dificuldade neste tema. E será o primeiro treinamento proposto.
  - Seguido por, Mindset (53%)
  - Contexto Estratégico (43%)
 

## Disponibilização dos materiais:

1. (Canvas)[https://www.canva.com/design/DAGMU7hoHns/28loiSCSaxLBBLSDU1LvTw/edit?utm_content=DAGMU7hoHns&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton]
2. (Google Sheets)[https://docs.google.com/spreadsheets/d/1RcVX3vdvbVI1iXQ7zGU6D2EUf131wTXZ/edit?usp=sharing&ouid=117066714637851671968&rtpof=true&sd=true]
