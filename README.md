# theCore _CS43L22 audio_ example

## Quick start

1. Install theCore:

   ```
   pip install tcore
   tcore bootstrap
   ```

1. Download this example:

   ```
   tcore init --remote https://github.com/theCore-embedded/example_cs43l22_audio
   ```

1. Compile:

   ```
   cd example_cs43l22_audio
   tcore compile --target stm32f4_disc
   ```

1. Run:

   1. On old STM32F407G-DISC boards, with STLINK/V2: 

      * With `sudo`:

        ```
            tcore --sudo flash
        ```

      * Without `sudo`:

        ```
            tcore flash
        ```

   1. On new STM32F407G-DISC1 boards, with STLINK/V2.1:

      * With `sudo`:

        ```
            tcore --sudo flash --debuger-config stlink-v2.1
        ```

      * Without `sudo`:

        ```
            tcore flash --debuger-config stlink-v2.1
        ```


This full example description and documentation is located in [theCore website](https://forgge.github.io/theCore/examples.html#stm32f4-discovery-audio-example-with-cs43l22-audio-dac)

