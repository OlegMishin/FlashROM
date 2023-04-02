# FlashROM
Different Flash memory adapters for Commodore/Amiga or other classic computers/devices.

For now there are following types of the FlashROM: 
1. 40pin to be used in Amiga 500.
2. 42 pin designed for my Amiga 1200 but also can be used in A500 rev 8 mainboard.
3. 24 pin for Commodore 64 computers. Replacement for 2316/2332/2364 ROM chips.
4. 28 pin for other devices. Replaces 2764..27512. Supports long and short Flash memory package.

Schematics/BOM and Gerbers located in each ones folder.

# 3D render

![image](https://user-images.githubusercontent.com/81614352/164697567-8bb8a18c-abe1-49d6-b01f-3e5f90ce9067.png)

# Actual photos

40 pin in A500

![image](https://user-images.githubusercontent.com/81614352/164701710-d0ddf5fc-10ba-4de5-815e-14ce9a62f760.png)

42 pin x2 in A1200

![image](https://user-images.githubusercontent.com/81614352/164702038-e1004d7c-96cb-4587-a1e6-9f371c470d13.png)

24 pin, KERNAL, CHAR, BASIC ROMs replacement in Commodore C64

![image](https://user-images.githubusercontent.com/81614352/170873651-b827d464-fac2-4697-8e85-1b298f188321.png)

28 pin

![image](https://user-images.githubusercontent.com/81614352/229347155-5faee86f-7641-4c63-8e72-032dd1b81a13.png)

To flash 28 pin FlashROM a simple adapter is needed as the pcb has four test points for flash control signals.
![image](https://user-images.githubusercontent.com/81614352/229347387-d288125d-6bfa-4db1-94ac-310a003501fa.png)




# FlashAdapter
An adapter for TL866 to program the 16 bit flash memory(40, 42 pin). It based on the circuit:
https://proghq.org/wiki/index.php/TL866_TSOP48_adapter
Circuit diagram, gerbers and ATtiny firmware are in "FlashAdapter" folder.

Four wires required to be connected between the adapter and 40pin FlashROM(as shown below):
A18, #BSY, #RST and #WE. 
For 42pin FlashROM, only needed #BSY, #RST and #WE as A18 and A19 already connected via socket's pins 1 and 2.

![image](https://user-images.githubusercontent.com/81614352/170577765-ba97ef12-a939-4824-9e7f-c49a6ee713c4.png)
