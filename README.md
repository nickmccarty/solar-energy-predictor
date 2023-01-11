# Predicting How Much Money Tesla Owes Us
## Using Tesla Solar Energy Data, Our Power Bill, and Historical Daylength Data for Our Local Area

<table width = "100%">
    <tr>
        <td>
            <img src="./images/tesla-app-screenshot.jpg"/> 
        </td>
        <td>
            <img src="./images/power-bill-screenshot.jpg"/>
        </td>
        <td>
            <img src="./images/daylength-data-screenshot.jpg"/>
        </td>
    </tr>
</table>

### Working Directory Structure

```
./
├── README.md
├── data
│   ├── interim
│   │   ├── combined-solar-data.csv
│   │   └── combined-sunlight-duration-data.csv
│   ├── processed
│   │   ├── resampled_merged_data.csv
│   │   ├── solar_and_daylength_data.csv
│   │   ├── solar_data.csv
│   │   └── sunlight_duration_in_decimal_hrs.csv
│   └── raw
│       ├── energy-costs.csv
│       ├── solar
│       │   ├── 1.10-1.16
│       │   ├── 1.17-1.23
│       │   ├── 1.24-1.30
│       │   ├── 1.3-1.9
│       │   ├── 1.31-2.6
│       │   ├── 10.10-10.16
│       │   ├── 10.17-10.23
│       │   ├── 10.24-10.30
│       │   ├── 10.3-10.9
│       │   ├── 10.31-11.6
│       │   ├── 11.1-11.7
│       │   ├── 11.15-11.21
│       │   ├── 11.22-11.28
│       │   ├── 11.29-12.5
│       │   ├── 11.8-11.14
│       │   ├── 12.13-12.19
│       │   ├── 12.20-12.26
│       │   ├── 12.27-1.2
│       │   ├── 12.6-12.12
│       │   ├── 2.14-2.20
│       │   ├── 2.21-2.27
│       │   ├── 2.28-3.6
│       │   ├── 2.7-2.13
│       │   ├── 3.14-3.20
│       │   ├── 3.21-3.27
│       │   ├── 3.28-4.3
│       │   ├── 3.7-3.13
│       │   ├── 4.11-4.17
│       │   ├── 4.18-4.24
│       │   ├── 4.25-5.1
│       │   ├── 4.4-4.10
│       │   ├── 5.16-5.22
│       │   ├── 5.2-5.8
│       │   ├── 5.23-5.29
│       │   ├── 5.30-6.5
│       │   ├── 5.9-5.15
│       │   ├── 6.13-6.19
│       │   ├── 6.20-6.26
│       │   ├── 6.27-7.3
│       │   ├── 6.6-6.12
│       │   ├── 7.11-7.17
│       │   ├── 7.18-7.24
│       │   ├── 7.25-7.31
│       │   ├── 7.4-7.10
│       │   ├── 8.1-8.7
│       │   ├── 8.15-8.21
│       │   ├── 8.22-8.28
│       │   ├── 8.29-9.4
│       │   ├── 8.8-8.14
│       │   ├── 9.12-9.18
│       │   ├── 9.19-9.25
│       │   ├── 9.26-10.2
│       │   └── 9.5-9.11
│       ├── sunlight-duration-2021.csv
│       └── sunlight-duration-2022.csv
├── images
│   ├── daylength-data-screenshot.jpg
│   ├── power-bill-screenshot.jpg
│   └── tesla-app-screenshot.jpg
└── notebooks
    ├── analysis
    │   ├── 1 - Solar EDA.ipynb
    │   ├── 2 - Sunlight Duration EDA.ipynb
    │   ├── 3 - Energy Cost EDA.ipynb
    │   └── 4 - Combined EDA.ipynb
    ├── modeling
    │   └── 1 - Feature Engineering.ipynb
    └── pre-processing
        ├── 1 - Solar Data Pre-Processing.ipynb
        ├── 2 - Sunlight Duration Data Pre-Processing.ipynb
        └── 3 - Merging Dataframes.ipynb
```