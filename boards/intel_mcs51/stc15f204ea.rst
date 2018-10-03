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

.. _board_intel_mcs51_stc15f204ea:

Generic STC15F204EA
===================

.. contents::

Platform :ref:`platform_intel_mcs51`: The Intel MCS-51 (commonly termed 8051) is an internally Harvard architecture, complex instruction set computer (CISC) instruction set, single chip microcontroller (uC) series developed by Intel in 1980 for use in embedded systems.

System
------

.. list-table::

  * - **Microcontroller**
    - STC15F204EA
  * - **Frequency**
    - 11Mhz
  * - **Flash**
    - 4KB
  * - **RAM**
    - 256B
  * - **Vendor**
    - `STC <https://www.stcmicro.com/STC/STC15F204EA.html?utm_source=platformio&utm_medium=docs>`__


Configuration
-------------

Please use ``stc15f204ea`` ID for :ref:`projectconf_env_board` option in :ref:`projectconf`:

.. code-block:: ini

  [env:stc15f204ea]
  platform = intel_mcs51
  board = stc15f204ea

You can override default Generic STC15F204EA settings per build environment using
``board_{JSON.PATH}`` option, where ``{JSON.PATH}`` is a path from
board manifest `stc15f204ea.json <https://github.com/platformio/platform-intel_mcs51/blob/master/boards/stc15f204ea.json>`_. For example,

.. code-block:: ini

  [env:stc15f204ea]
  platform = intel_mcs51
  board = stc15f204ea

  ; change microcontroller
  board_build.mcu = stc15f204ea

  ; change MCU frequency
  board_build.f_cpu = 11059200L

Debugging
---------
:ref:`piodebug` currently does not support Generic STC15F204EA board.