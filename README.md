# FanControl.Liquidctl

This is a fork of [jmarucha](https://github.com/jmarucha/FanControl.Liquidctl)'s original. It stops liquidctl from starting and stopping all the time by using a custom made [fork](https://github.com/SuspiciousActivity/liquidctl) that has an interactive mode. Works for my machine (Kraken X63) but not tested for anything else at all, **use at your own risk**. This applies to the liquidctl repo as well.

This is a simple plugin that uses [liquidctl](https://github.com/liquidctl/liquidctl) to provide sensor data and pump control to variety of AIOs. So far it is tested with NZXT Kraken X63, but in principle shall work with [supported devices](https://github.com/liquidctl/liquidctl#supported-devices)

## Installation

1. Download lasted [release](https://github.com/chaixshot/FanControl.Liquidctl/releases)
2. Fan Control > Settings > Instal Plugin... > Choose **FanControl.Liquidctl.zip**
3. Install [Python](https://www.python.org/downloads/) 3.9 or later
4. Open Windows CMD and install **liquidctl** ```pip install liquidctl```
5. Restart **Fan Control**

## Setting up the developer environment

The project, after being imported to Visual Studio needs to have it reference to `FanControl.Plugins.dll` and `Newtonsoft.Json.dll` from FanControl directory. You also need to create the executable of liquidctl, which can be automatized with script `build-liquidctl.sh`.

## Screenshots

![Fluid temperature sensor](/docs/images/FluidTemp.png)
![Pump speed and control](/docs/images/PumpControl.png)

## License
MIT license, because it's superior.
```
Copyright (c) 2022 Jan K. Marucha

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

liquidctl, which is used by this plugin is provided on [GPLv3](https://github.com/liquidctl/liquidctl/blob/main/LICENSE.txt).
