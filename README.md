# Semana 11 — Laboratório Prático

## Objetivo da atividade

Até aqui, vimos como diferentes modelos de Machine Learning se comportam de forma isolada. Agora, vamos colocá-los à prova no mesmo cenário, comparando seus resultados.

O cenário proposto é o seguinte:

> Fomos contratados por um hospital referência em oncologia. O objetivo é criar uma Inteligência Artificial que irá auxiliar os médicos no diagnóstico de tumores de mama.

Durante o laboratório, cada grupo deverá desenvolver e comparar dois modelos de classificação:

* K-Nearest Neighbors (KNN)
* Árvore de Decisão

A análise deverá considerar não apenas a acurácia dos modelos, mas também outras métricas relevantes para o problema, com atenção especial aos erros de classificação de tumores malignos.

---

## Dataset

Será utilizado o dataset **Breast Cancer Wisconsin**, disponível nativamente no `scikit-learn`.

O conjunto de dados possui:

* 569 pacientes;
* 30 características celulares extraídas de exames de biópsia;
* Variáveis relacionadas a raio, textura, perímetro, área, suavidade, entre outras.

### Variável-alvo

| Valor | Classificação |
| ----- | ------------- |
| `0`   | Tumor Maligno |
| `1`   | Tumor Benigno |

---

## Configuração e acesso ao repositório

Cada grupo possui um repositório próprio para realizar a atividade.

Antes de começar, certifique-se de que você está trabalhando no **repositório correto do seu grupo**.

### 1. Acesse o repositório do seu grupo

Entre no GitHub e acesse o repositório correspondente ao seu grupo.

Na página do repositório, clique no repositório do seu grupo e copie a URL do repositório.

Exemplo:

```text
https://github.com/Machine-Learning-Visao-Computacional-T3/SEMANA_11/tree/main/GRUPO_1
```

> Utilize a URL do seu grupo. O endereço acima é apenas um exemplo.

### 2. Clone o repositório

Abra o terminal e navegue até a pasta onde deseja salvar o projeto:

```bash
cd caminho/para/sua/pasta
```

Em seguida, clone o repositório:

```bash
git clone URL_DO_REPOSITORIO
```

Por exemplo:

```bash
git clone https://github.com/Machine-Learning-Visao-Computacional-T3/SEMANA_11/tree/main/GRUPO_1
```

Depois, entre na pasta criada:

```bash
cd SEMANA_11_GRUPO_1
```

### 3. Verifique o repositório

Confira se o notebook do laboratório está presente:

```bash
ls
```

ou, no Windows:

```bash
dir
```

Você deverá encontrar o arquivo:

```text
laboratorio_pratico.ipynb
```

### 4. Abra o notebook

Abra o notebook utilizando o ambiente utilizado durante as aulas, como Jupyter Notebook, JupyterLab, VS Code ou Google Colab, conforme orientação da aula.

Realize toda a atividade **dentro do notebook do seu grupo**.

### 5. Salve e envie suas alterações

Após concluir a atividade, verifique as alterações realizadas:

```bash
git status
```

Adicione os arquivos modificados:

```bash
git add .
```

Crie um commit:

```bash
git commit -m "Finaliza laboratorio pratico da Semana 11"
```

Envie as alterações para o GitHub:

```bash
git push
```

Após o `push`, confirme no GitHub se o notebook atualizado está disponível no repositório do grupo.

---

## Estrutura do laboratório

O notebook está dividido nas seguintes etapas:

| Parte   | Conteúdo                                  |
| ------- | ----------------------------------------- |
| Parte 0 | Setup do ambiente                         |
| Parte 1 | Exploração dos dados                      |
| Parte 2 | Pré-processamento                         |
| Parte 3 | Modelo 1: KNN                             |
| Parte 4 | Modelo 2: Árvore de Decisão               |
| Parte 5 | Comparação final entre os modelos         |
| Parte 6 | Relatório de recomendação para o hospital |

O laboratório foi planejado para aproximadamente **2h30min**.

---

## Organização dos grupos

O repositório principal da atividade é o **SEMANA_11**.

Dentro dele, existem quatro repositórios, um para cada grupo. Cada grupo deverá trabalhar exclusivamente no seu respectivo repositório.

A estrutura geral é:

```text
SEMANA_11/
│
├── laboratorio_pratico_original.ipynb
│
├── SEMANA_11_GRUPO_1/
│   └── laboratorio_pratico_grupo1.ipynb
│
├── SEMANA_11_GRUPO_2/
│   └── laboratorio_pratico_grupo2.ipynb
│
├── SEMANA_11_GRUPO_3/
│   └── laboratorio_pratico_grupo3.ipynb
│
└── SEMANA_11_GRUPO_4/
    └── laboratorio_pratico_grupo4.ipynb
```

Os nomes exatos dos repositórios dos grupos podem variar de acordo com a organização da turma.

### Importante

Cada aluno deve:

1. Identificar o repositório correto do seu grupo;
2. Clonar **apenas o repositório do seu grupo**;
3. Trabalhar no `laboratorio_pratico.ipynb` disponibilizado nesse repositório;
4. Fazer `commit` das alterações;
5. Fazer `push` para o GitHub ao finalizar.

---

## Arquivo original

O arquivo [`laboratorio_pratico_original.ipynb`](https://github.com/Machine-Learning-Visao-Computacional-T3/SEMANA_11/blob/main/laboratorio_pratico_original.ipynb) está disponível na pasta principal do repositório **SEMANA_11** como **backup da versão original do laboratório**.

Cada grupo possui uma cópia do laboratório em seu próprio repositório.

**Não editem diretamente o arquivo original.**

Caso seja necessário recuperar o notebook original, utilize o arquivo disponível na pasta principal como referência.

---

## Checklist de entrega

Ao final da atividade, o notebook do grupo deverá conter:

* [ ] Todas as células de código executadas sem erro;
* [ ] Exploração inicial do dataset;
* [ ] Verificação do balanceamento das classes;
* [ ] Separação dos dados entre treino e teste;
* [ ] Pré-processamento e padronização dos dados;
* [ ] Modelo KNN treinado e avaliado;
* [ ] Teste de diferentes valores de `k`;
* [ ] Escolha e justificativa do melhor `k`;
* [ ] Árvore de Decisão treinada e avaliada;
* [ ] Teste de diferentes valores de `max_depth`;
* [ ] Comparação entre desempenho de treino e teste;
* [ ] Escolha e justificativa da melhor profundidade;
* [ ] Matrizes de confusão dos dois modelos;
* [ ] Tabela comparativa das principais métricas;
* [ ] Análise dos falsos negativos;
* [ ] Respostas das perguntas propostas ao longo do laboratório;
* [ ] Relatório final de recomendação para o hospital preenchido.
