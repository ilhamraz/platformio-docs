..  Copyright (c) 2014-present PlatformIO <contact@platformio.org>
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
       http://www.apache.org/licenses/LICENSE-2.0
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

.. _board_atmelavr_feather328p:

Adafruit Feather 328P
=====================

.. contents::

Platform :ref:`platform_atmelavr`: Atmel AVR 8- and 32-bit MCUs deliver a unique combination of performance, power efficiency and design flexibility. Optimized to speed time to market-and easily adapt to new ones-they are based on the industrys most code-efficient architecture for C and assembly programming.

System
------

.. list-table::

  * - **Microcontroller**
    - ATMEGA328P
  * - **Frequency**
    - 8Mhz
  * - **Flash**
    - 31.50KB
  * - **RAM**
    - 2KB
  * - **Vendor**
    - `Adafruit <https://www.adafruit.com/product/3458?utm_source=platformio&utm_medium=docs>`__


Configuration
-------------

Please use ``feather328p`` ID for :ref:`projectconf_env_board` option in :ref:`projectconf`:

.. code-block:: ini

  [env:feather328p]
  platform = atmelavr
  board = feather328p

You can override default Adafruit Feather 328P settings per build environment using
``board_{JSON.PATH}`` option, where ``{JSON.PATH}`` is a path from
board manifest `feather328p.json <https://github.com/platformio/platform-atmelavr/blob/master/boards/feather328p.json>`_. For example,

.. code-block:: ini

  [env:feather328p]
  platform = atmelavr
  board = feather328p

  ; change microcontroller
  board_build.mcu = atmega328p

  ; change MCU frequency
  board_build.f_cpu = 8000000L

Debugging
---------
:ref:`piodebug` currently does not support Adafruit Feather 328P board.

Frameworks
----------
.. list-table::
    :header-rows:  1

    * - Name
      - Description

    * - :ref:`framework_arduino`
      - Arduino Wiring-based Framework allows writing cross-platform software to control devices attached to a wide range of Arduino boards to create all kinds of creative coding, interactive objects, spaces or physical experiences.