# EurorackEnvelopeGenerator
An envelope generator Eurorack module, based on the Electric Druid EnvGen8 chip.
The chip is available at the [ElectricDruid](https://electricdruid.net) web shop.

There is a [YouTube video](https://youtu.be/kh0m0Idso9o) available with some demonstration of this an a few other ADSR modules.

## Design and Modification
The design mainly follows the schematic provided in the Electric Druid chip documentation.

The chip output level is between 0V and +5V.
This is increased by a factor 2 in my design, as I prefer to have  max out of +10V for my envelope generators.
If you want to have the original +5V output, just replace resistor R16 (20K) with a 10K resistor.

## Module Built and PCBs
If you want to build the module yourself, I uploaded the schematics, the BOM and the Gerber files for the PCB.

There are two different versions for the control board, an "original" and a "Thonk" version.
Reason is that for my own module, I am using specific potentiometers - 16K4 series from Supertech Electronics - and 3.5mm jack sockets - MJ-355 from Marushin - available at my local electronics shop.

However, since most DIY projects for Eurorack modules out there are using potentiometers from ALPHA and so-called THONKICONN jacks, as they are provided by Thonk in the UK, I also created a version with footprints for those components.
Choose the one you need.

I created the Gerber files with the online tool EasyEDA and ordered it at JLCPCB.
I cannot guarantee, if this set of zipped Gerber files works also for other providers, like e.g. PCBWay. I have not tried that. But I saw online, that others did it.

You might have seen in the photo of the module backside below that there is a wire soldered between the gate and trigger jacks. That is the correction of an error I found after I already ordered the PCBs. That error is fixed in the Gerber files and in the schematic.

## Panel Layout
I added the information about hole coordinates for the front panel in the folder PanelLayout, referring to the component layout in the Gerber files. The layout is the same for both versions.

## Additional Information about specific Components
If you want to use the Gerber files for having PCB manufactured, please note the following information about components used.

- The module is mainly using THT components.There is only a number of SMD 0.1uF capacitors with the package size 1608.
- In order to save space, I am always using small size resistors, about 3mm length, which are about half the size of usually used resistors.

![EnvGen](https://user-images.githubusercontent.com/97026614/192098471-b669f019-572a-496e-8c8f-6947cc0d9cd8.jpeg)

![EnvGenFront](https://user-images.githubusercontent.com/97026614/192098477-b9432812-7527-4084-833a-a47fdb83da9e.jpeg)

![EnvGenBack](https://user-images.githubusercontent.com/97026614/192098488-47a251d0-43d9-4013-b616-e3a2d452e1e5.jpeg)

![EnvGenSide](https://user-images.githubusercontent.com/97026614/192098500-59872c81-8888-4879-9a10-f07366d42855.jpeg)

<img width="742" alt="PCB_Main_Back" src="https://user-images.githubusercontent.com/97026614/192097654-7a270e5f-7fad-4a6e-8093-694130036e2f.png">

<img width="742" alt="PCB_Wain_Front" src="https://user-images.githubusercontent.com/97026614/192097663-136f6a4f-e18d-44f0-873e-4165023815a7.png">

<img width="399" alt="PCB_Ctrl_Front" src="https://user-images.githubusercontent.com/97026614/192097671-76f63356-2940-4e9d-ac19-bc1404821650.png">

<img width="399" alt="PCB_Ctrl_Back" src="https://user-images.githubusercontent.com/97026614/192097677-f62215f7-2171-455d-a9e7-321993803fd1.png">
