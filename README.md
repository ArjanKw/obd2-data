# OBD2 data
Need OBD2 data for big data analysis? This repository shares OBD2 datasets. The data is collected with the app "CarScanner".

## Use cases
- Analyze driving behavior (clutch usage, driving style)
- Determine fuel consumption based on the speed
   - Record the fuel consumption and speed when the car isn't accelerating
- Determine when tyres need to be inflated
   - Improper inflated tyres cause an increase in fuel usage
- Determine how good you are with rev matching when down shifting
- Determine the roll factor of your car.
- ...

## Participate
Everyone is welcome to add data to the set.

## About the data
The data is seperated by driver/car combination. Each driver has it's own folder. Each folder contains a readme, containing information about the car.

### File name
The file name is in the following format:

> `YYYY-MM-DD hh-MM-ss_[mode]-[from]-[to]-[description].csv`

The date/time is the starting point of the recording. The part behind the time is optional. It provides the driving mode, and an identifier of the starting point and the end point.

| Parameters | Values |
| --- | --- |
| **Mode** | Eco / Normal / Rush |
| **From** | Unique identifier of the starting point of the recording |
| **To** | Unique identifier of the end point of the recording |
| **Description** | Description, if necessary |

_From_ and _To_ can be used to group (semi) identical routes to each other, without the need to process GPS data. 
