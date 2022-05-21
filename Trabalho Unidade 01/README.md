# Trabalho 02 Unidade 1
Projeto da disciplina de análise de redes da UFRN que tem como objetivo principal colocar em prática o conteúdo referente a Unidade 1 da matéria, focado nos princípios de visualização de dados e métricas de grafos.

Trabalho baseado no repositório: https://github.com/alvarofpp/dataset-flights-brazil

A resolução do trabalho está no notebook `Trabalho 2 Unidade 1.ipynb`.

## 📚 Requisitos

Verifique se você atende a todos os requisitos a seguir:
* Ter uma máquina com ` Windows | Linux | Mac `.
* Ter o [`Python 3.9`](https://www.python.org/downloads/) instalado na sua máquina.
* Ter os pacotes necessários do python instalados:
```
pip install -r requirements.txt
```

## Começando

Para começar a usar este projeto, basta clonar o repositório:

Opção HTTP:
```
git clone https://github.com/matheusriv/network_analysis_2021.2.git
```

Opção SSH:
```
git clone git@github.com:matheusriv/network_analysis_2021.2.git
```

## Datasets
Os datasets estão na pasta `data/`.

### `anac.csv`
Todos os voos no Brasil pela ANAC. A ANAC não disponibiliza o dicionário de dados.

#### Columns:
company_abbreviation', 'company_name', 'company_nationality', 'year', 'month', 'origin_airport_abbreviation', 'origin_airport_name', 'origin_airport_state', 'origin_airport_region', 'origin_airport_country', 'origin_airport_continent', 'destination_airport_abbreviation', 'destination_airport_name', 'destination_airport_state', 'destination_airport_region', 'destination_airport_country', 'destination_airport_continent', nature', 'flight_group', 'paid_passenger', 'free_passenger', 'charge_paid_kg', 'charge_free_kg', 'mail_kg', 'ask', 'rpk', 'atk', 'rtk', 'fuel_l', 'distance_flown_km', 'takeoffs', 'charge_paid_km', 'charge_free_km', 'mail_km', 'seats', 'payload', 'fly_hours', 'baggage_kg'.

### `airports.csv`
Todos os aeroportos nos registros de voo da ANAC.

| Column | Type | Description | Example |
| --- | --- | --- | --- |
| code | `string` | [ICAO airport code](https://en.wikipedia.org/wiki/ICAO_airport_code) | `"SNBG"` |
| name | `string` | Airport name. | `"BAIXO GUANDU"` |
| state | `string` | State where the airport is located. | `"ES"` |
| region | `string` | Region where the airport is located. | `"SUDESTE"` |
| country | `string` | Country where the airport is located. | `"BRASIL"` |
| continent | `string` | Continent where the airport is located. | `"AMÉRICA DO SUL"` |
| lat_geo_point | `double` | Latitude of the airport reference point. | `-19.498889` |
| lon_geo_point | `double` | Longitude of the airport reference point. | `-41.041944` |

### `air_traffic.graphml`
É um grafo não direcionado.

#### Atributos do nós
The id of each node is the ICAO airport code.

| Column | Type | Description | Example |
| --- | --- | --- | --- |
| name | `string` | Airport name. | `"GUARULHOS"` |
| country | `string` | Country where the airport is located. | `"BRASIL"` |
| latitude | `double` | Latitude of the airport reference point. | `-23.435556` |
| longitude | `double` | Longitude of the airport reference point. | `-46.473056` |
| region | `string` | Region of Brazil where the airport is located. | `"SUDESTE"` |

#### Atributos das arestas
| Column | Type | Description | Example |
| --- | --- | --- | --- |
| flight_count | `int` | Number of flights carried out between these airports. | `147` |
