---
hide:
- navigation
---

# Labs & Projects

## Radar Platform

The labs and projects will be principally based on the [TI AWR1843AOPEVM](https://www.ti.com/tool/AWR1843AOPEVM) mmWave radar evaluation module and the [RadarML](https://radarml.github.io/) / [xwr](https://radarml.github.io/xwr/) software stack.

Students will receive a lab kit with the following:

- Radar & capture card assembly, with the TI AWR1843AOPEVM and DCA1000EVM within a 3D-printed enclosure
- 5v power supply for the capture card
- Micro USB cable and ethernet cable

??? quote "Radar Assembly BOM"

    | Part | Qty | Description |
    | --- | --- | --- |
    | `shell.STL`; PLA, standard print quality | 1 | Top shell of the enclosure, with mounting points for each component |
    | `bottom.STL`; PLA, standard print quality | 1 | Bottom plate with 1/4-20 inserts for tripod attachment |
    | [TI AWR1843AOPEVM](https://www.ti.com/tool/AWR1843AOPEVM) | 1 | Radar sensor |
    | [TI DCA1000EVM](https://www.ti.com/tool/DCA1000EVM) | 1 | Radar capture card |
    | [Samtec HQCD-030-06.00-TEU-SEU-1 Coaxial Ribbon Cable](https://www.digikey.com/en/products/detail/samtec-inc/hqcd-030-06-00-teu-seu-1/6691516) | 1 | Longer version of the cable included with the DCA1000EVM |
    | [5.5x2.1mm DC Jack Panel Mount, 12mm diameter](https://www.amazon.com/Tugermoola-Threaded-Female-Connector-Adapter/dp/B0DP6MNQQB) | 1 | Power input for the DCA1000EVM | 
    | [5.5x2.1mm DC Jack 90 degree](https://www.amazon.com/10-Pack-Connectors-Monitors-Surveillance-Security/dp/B0G4R6M31D) | 1 | Power input for the DCA1000EVM |
    | M2x5mm screw | 2 | Mounting the AWR1843AOPEVM to the shell |
    | M2.5x5mm screw | 2 | Mounting the AWR1843AOPEVM to the shell |
    | M3x5mm screw | 4 | Mounting the DCA1000EVM to the shell |
    | M3x8mm screw | 4 | Attaching the bottom plate |
    | M3x5x4 heat set insert | 4 | Installed in the top shell |
    | 1/4-20 heat set insert | 3 | Installed in the bottom plate |

## Course Project

In groups of up to 4, students will complete an open-ended project applying machine learning techniques to the AWR1843AOP radar platform or another RF system of their choice. The project must have the following elements:

- A machine learning component (i.e., a data-driven algorithm) must be used to perform some task; training and fine-tuning is encouraged, but not required.
- The project must involve the team working with a real RF system, either for data collection and/or deployment. In other words, projects must either collect some data, demonstrate their model running on a real system, or ideally, both!
