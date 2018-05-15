CS43L22 audio example for theCore embedded C++ framework
========================================================

.. image:: https://travis-ci.org/theCore-embedded/example_cs43l22_audio.svg?branch=master
    :target: https://travis-ci.org/theCore-embedded/example_cs43l22_audio

This example is avaliable for STM32F4 Discovery board only.

Detailed description
--------------------

See `theCore documentation for CS43L22 audio example`_ for more information.

Quick start
-----------

#. Install theCore (this may take a while)::

        pip3 install tcore
        tcore bootstrap

#. Download this example::

        tcore init --remote https://github.com/theCore-embedded/example_cs43l22_audio

#. Step into the project directory::

        cd example_cs43l22_audio

#. Compile:

        tcore compile --target stm32f4_disc

#. Connect your STM32 Discovery board.

#. Connect headphones to audio jack on STM32 Discovery board.

#. Run:

   * For old STM32F407G-DISC boards, with STLINK/V2::

        tcore --sudo flash

   * For new STM32F407G-DISC1 boards, with STLINK/V2.1::

        tcore --sudo flash --debugger-config stlink-v2.1

#. Listen to cool 8-bit music in your headphones.

.. _`theCore documentation for CS43L22 audio example`: https://forgge.github.io/theCore/examples/stm32f4-discovery-cs43l22.html
