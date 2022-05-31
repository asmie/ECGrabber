# ECGrabber

## General Description

ECGrabber is a prototype for multi-purpose device that can monitor ECG using analog sensors either 3 or 12 lead. In the first stage only 3 lead sensor will be used but during the next phase there is a plan to use 12 lead sensor to monitor full ECG.

ECGrabber can be used during move and is designed as simple and compact size with the following functionality:
- monitor ECG (using 3 or 12 lead sensor)
- transmit ECG data using Bluetooth to the phone or PC
- transmit ECG data to the defined server using GSM data transmission
- detect movement and fall
- alarm defined contacts using SMS or call with the position of the person (GPS)

Project consists of:
- STM32H743ZIT6U on the NUCLEO board
- AD8232 - analog ECG sensor
- LIS3DHTR  for acceleration and fall detection
- Waveshare 13460 with SIM868 module for GSM alert connectivity, Bluetooth 3.0 and GNSS.

## Current state
Project is still under development.
Current work is done towards:
- AD8232 handling using STM32 ADC
- GSM connectivity (SMS sending).

## Usage

### Building

There can be used STM32CubeIDE to build the whole project. It's possible to generate Makefile from the tool and use it in the command line using gcc compiler for STM32 target.

## Bug reporting

Bugs can be reported using [GitHub issue tracker](https://github.com/asmie/ECGrabber/issues).

## Further development
Project is currently under development.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## Versioning

I use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/asmie/ECGrabber). 

## Authors

* **Piotr Olszewski** - *Original work* - [asmie](https://github.com/asmie)

See also the list of [contributors](https://github.com/asmie/ECGrabber/contributors) who participated in this project.


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
