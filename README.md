<p align="center">
![GitHub repo size](https://img.shields.io/github/repo-size/iurygdeoliveira/cyclevis_dataset?style=flat-square) [![HitCount](https://hits.dwyl.com/iurygdeoliveira/cyclevis_dataset.svg?style=flat-square)](http://hits.dwyl.com/iurygdeoliveira/cyclevis_dataset)
</p>

# Cyclevis Master Project Dataset

<p align="justify"> 
Technological evolution and the growing massive production of data demand the creation of new mechanisms for
processing and analysis in the most different domains of information. The same is true for the domain of sports,
which has a great popular appeal worldwide and has increasingly gained the scientific community’s interest. Among the
different sports genres, cycling has gained special attention in the information visualization and
Visual Analytics community over the years. In general, these works focus on discovering patterns to
strategize, display statistical information, or analyze the performance of groups of cyclists. However,
there is a gap in works that focus on courses unrelated to professional competitions or considering
climate and intensity attributes in their analyses. In this context, this master’s proposal presents a
data visualization approach that understands these characteristics in specific recreational races that contain
intensity characteristics, such as heart rate, cadence, and elevation, and climatic variables, such
as temperature, in addition to the traditional variables related to the route and geolocation.
The objective is to find patterns of visual information that provide an understanding of how these variables
influence the performance of cyclists and provide a comparison between them. To assist the visual exploration
process, multidimensional, temporal, graph, and geolocation visualization techniques will be juxtaposed
and coordinated to facilitate user interaction. Additionally, this proposal presents an evaluation
methodology based on qualitative and quantitative metrics. Specifically, three types of usability
assessments will be carried out, i) the cognitive path to assess effectiveness, ii) heuristic assessment
to assess efficiency, and iii) questionnaire using the scale SUS (System Usability Scale)
to assess satisfaction. Therefore, this repository stores the dataset used in this project.
<b>Access the project at this link:</b>
</p>

## Demo

Link do youtube

## Supporting Universities

<img src="download.png"> ![Logo](https://computacao.ufba.br/sites/computacao.ufba.br/files/logo_dcc_1.png)

## Authors

Master's student - [Prof. Esp. Iury Gomes de Oliveira](https://github.com/iurygdeoliveira)\
Mentor - [Prof. Dr. Danilo Coimbra](http://lattes.cnpq.br/9590398895954821)

## Documentação da API

#### Retorna todos os itens

```http
  GET /api/items
```

| Parâmetro | Tipo     | Descrição                           |
| :-------- | :------- | :---------------------------------- |
| `api_key` | `string` | **Obrigatório**. A chave da sua API |

#### Retorna um item

```http
  GET /api/items/${id}
```

| Parâmetro | Tipo     | Descrição                                   |
| :-------- | :------- | :------------------------------------------ |
| `id`      | `string` | **Obrigatório**. O ID do item que você quer |

#### add(num1, num2)

Recebe dois números e retorna a sua soma.

## Support

iurygdeoliveira@gmail.com
