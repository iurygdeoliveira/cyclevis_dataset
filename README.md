# Cyclevis Master Project Dataset ![GitHub repo size](https://img.shields.io/github/repo-size/iurygdeoliveira/cyclevis_dataset?style=flat-square) [![HitCount](https://hits.dwyl.com/iurygdeoliveira/cyclevis_dataset.svg?style=flat-square)](http://hits.dwyl.com/iurygdeoliveira/cyclevis_dataset)

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

## Directory and File Structure

Each pedal has several trackpoints\
.\
├── Cyclist (Contains the cyclist's data)\
│ ├── all_distances.json (Contains the distances of each pedal)\
│   ├── pedal (Contains the pedal data)\
│   │   ├── distance_history.json (Distance recorded at each trackpoint)\
│   │   ├── elevation_bing.json (Elevation provided by bing for the coordinate latitude,longitude)\
│   │   ├── elevation_google.json (Elevation provided by google for the coordinate latitude,longitude)\
│   │   ├── elevation_gps.json (Elevation recorded at each trackpoint)\
│   │   ├── heartrate_history.json (heartrate recorded at each trackpoint)\
│   │   ├── latitudes.json (latitude recorded at each trackpoint)\
│   │   ├── longitudes.json (longitude recorded at each trackpoint)\
│   │   ├── overview.json (Contains general data, e.g., average speed, average heart rate, total trackpoints, etc.)\
│   │   ├── speed_history.json (speed recorded at each trackpoint)\
│   │   └── time_history.json (time recorded at each trackpoint)\

Additional information about the overview.json file

-   pedal: ID used in mysql database
-   path: gpx file path,
-   creator: Device or platform generating the data
-   coordinateInicial: Latitude Initial | Longitude Initial
-   coordinateFinal: Latitude Final | Longitude Final
-   country: pedal country,
-   locality: pedal locality,
-   centroid: pedal centroid
-   bbox: pedal bounding box,
-   datetime: pedal datetime,
-   duration: pedal duration (HH:MM:SS),
-   distance: pedal distance in kilometers,
-   elevation_gps: pedal elevation recorded in gps in meters,
-   elevation_google: pedal elevation obtained from google API in meters,
-   elevation_bing: pedal elevation obtained from bing API in meters,
-   speed_avg: Average pedal speed in KM/H,
-   heartrate_avg: Average pedal heartrate in bpm,
-   temperature_avg: Average pedal temperature in celsius,
-   trackpoints: total pedal trackpoints

## Reference

The original data was obtained from:

-   RAUTER, S.; FISTER, I. A collection of sport activity files for data analysis and data mining. University of Ljubljana, 2015

Additional information on data preprocessing

-   RAUTER, S.; FISTER, I.; JR, I. F. How to deal with sports activity datasets for data mining and analysis:. International Journal of Advanced Pervasive and Ubiquitous Computing, v. 7, p. 27–37, 04 2015

## API (Coming Soon)

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
