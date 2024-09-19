# GO Weather CLI

This is a CLI tool written in go to fetch weather forecast details from [weatherapi.com](https://www.weatherapi.com/).

## Setup

1. Clone the repository:
    ```sh
    git clone https://github.com/rishikesh-suvarna/weather-cli.git
    cd weather-cli
    ```

2. Create a `.env` file in the root directory and set the `WEATHER_API_KEY`:
    ```sh
    echo "WEATHER_API_KEY=your_api_key_here" > .env
    ```

3. Install dependencies:
    ```sh
    go mod tidy
    ```

## Usage

To use this application, run the following command with one of the supported arguments: US Zipcode, UK Postcode, Canada Postalcode, IP address, Latitude/Longitude (decimal degree), or city name.

```sh
go run main.go <argument>
```

### Examples

- By US Zipcode:
    ```sh
    go run main.go 90210
    ```

- By UK Postcode:
    ```sh
    go run main.go SW1A1AA
    ```

- By Canada Postalcode:
    ```sh
    go run main.go M5V3L9
    ```

- By IP address:
    ```sh
    go run main.go 8.8.8.8
    ```

- By Latitude/Longitude:
    ```sh
    go run main.go "40.7128,-74.0060"
    ```

- By City Name:
    ```sh
    go run main.go "New York"
    ```

## License

This project is licensed under the MIT License. See the [LICENSE](https://github.com/rishikesh-suvarna/weather-cli/blob/main/LICENSE) file for details.