# Trabalho 02 Unidade 1
Aluno: Matheus Rivaldo da Silva

Trabalho baseado no repositório https://github.com/alvarofpp/dataset-flights-brazil

A resolução do trabalho está no notebook `Trabalho 2 Unidade 1.ipynb`

## [`air_traffic.graphml`](https://drive.google.com/file/d/1Xh0Ga_AjRqv7LrpAv2KPTn3AAE7i5zNm/view?usp=sharing)
It's an undirected graph.

### Node attributes
The id of each node is the ICAO airport code.

| Column | Type | Description | Example |
| --- | --- | --- | --- |
| name | `string` | Airport name. | `"GUARULHOS"` |
| country | `string` | Country where the airport is located. | `"BRASIL"` |
| latitude | `double` | Latitude of the airport reference point. | `-23.435556` |
| longitude | `double` | Longitude of the airport reference point. | `-46.473056` |
| region | `string` | Region of Brazil where the airport is located. | `"SUDESTE"` |

### Edge attributes
| Column | Type | Description | Example |
| --- | --- | --- | --- |
| flight_count | `int` | Number of flights carried out between these airports. | `147` |

