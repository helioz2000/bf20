# Commands and info 
##related to Mesa interface card:

To see mesa card info:
mesaflash --device 7C81 --spi --addr /dev/spidev0.0 --readhmid

To verify a loaded file:
mesaflash --device 7C81 --spi --addr /dev/spidev0.0 --verify FPGAFILE.BIT

To write new bit file:
mesaflash --device 7C81 --spi --addr /dev/spidev0.0 --write FPGAFILE.BIT

To write fallback bit file:
mesaflash --device 7C81 --spi --addr /dev/spidev0.0 --fallback --write FALLBACK.BIT
fallback bit file is provided by Mesa and will load if the user config is corrupt or invalid. 
The Init LED will flash if the fallback config is activated and a new bitfile can be loaded.

---

# Bit files:

  * 7c81_7i85x1d.bit - supplied by Peter Wallace from Mesa on 8 April 2020

  * 7c81_7i85S.bit - compiled by helioz2000
