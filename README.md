# Cloud Sim examples

Firmware projects to build on your computer and run on
[Cloud Sim](https://simantic.com/cloud-sim), which simulates the
microcontroller in the cloud, so you don't need a board.

Each top-level folder is an MCU, named as the API names it: the `mcu` its
projects run on. Each folder in it is a project, with a README that says
what it does, what you need, and how to build and run it.

| MCU | Project | What it does |
| --- | --- | --- |
| [STM32F401RE](STM32F401RE) | [hello-world](STM32F401RE/hello-world) | Prints "Hello, world!" over UART, then the time, once a second. An STM32CubeMX project, built with make. |

## Get started

```
git clone https://github.com/simantic-dev/cloud-sim-examples.git
cd cloud-sim-examples/STM32F401RE/hello-world
```

Then follow the project's README. To run anything on Cloud Sim, you need an
API key, from your account's [API Settings](https://simantic.com/account/api).
The [API reference](https://cloud.simantic.com/v1/docs) has every call.

## Adding an example

A new project goes in its MCU's folder, `<MCU>/<project>/`, with the folder
named as the API names the MCU (a new MCU gets a new top-level folder). Give
it a README that says what it does and how to build and run it, and add a
row for it to the table above.

## License

[MIT](LICENSE), except vendor code such as ST's HAL and Arm's CMSIS in a
project's `Drivers/` folder, which keeps the license that comes with it.
