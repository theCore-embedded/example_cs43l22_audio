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

   * With `sudo`:

     ```
        tcore runenv --sudo -- openocd -f board/stm32f4discovery.cfg -c 'init; reset halt; flash write_image erase audio.bin 0x08000000; reset run; exit'
     ```

   * Without `sudo`:

     ```
        tcore runenv -- openocd -f board/stm32f4discovery.cfg -c 'init; reset halt; flash write_image erase audio.bin 0x08000000; reset run; exit'
     ```

   **TODO**

This full example description and documentation is located in [theCore website](https://forgge.github.io/theCore/examples.html#stm32f4-discovery-audio-example-with-cs43l22-audio-dac)

