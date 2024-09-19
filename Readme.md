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

## Build

To build the application, run the following command:
```sh
go build -o ./build/weather-cli
```

Once the build is created, you can move it to your OS binary directory to run it directly from the terminal.

For macOS/Linux:
```sh
sudo mv ./build/weather-cli /usr/local/bin/weather-cli
```

For Windows:
```sh
move .\build\weather-cli.exe C:\Windows\System32\weather-cli.exe
```

## Usage

To use this application, run the following command with one of the supported arguments: US Zipcode, UK Postcode, Canada Postalcode, IP address, Latitude/Longitude (decimal degree), or city name.

```sh
weather-cli <argument>
```

### Examples

- By US Zipcode:
    ```sh
    weather-cli 90210
    ```

- By UK Postcode:
    ```sh
    weather-cli SW1A1AA
    ```

- By Canada Postalcode:
    ```sh
    weather-cli M5V3L9
    ```

- By IP address:
    ```sh
    weather-cli 8.8.8.8
    ```

- By Latitude/Longitude:
    ```sh
    weather-cli "40.7128,-74.0060"
    ```

- By City Name:
    ```sh
    weather-cli "New York"
    ```

## License

This project is licensed under the MIT License. See the [LICENSE](https://github.com/rishikesh-suvarna/weather-cli/blob/main/LICENSE) file for details.