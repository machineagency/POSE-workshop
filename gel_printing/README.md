# 3D printing with syringe tool

If you wish to engage with Jubilee multi-material 3D printing while taking advantage of slicing software, here is a guide to using the Duet interface and PrusaSlicer to do so!

## Generate GCode using PrusaSlicer

Many slicers can be configured to work with Jubilee. Here, we use PrusaSlicer. The laptops provided in this workshop should have PrusaSlicer installed and configured. If you wish to have it on your own computer, you need to install the latest PrusaSlicer and import the config bundle `Jubilee_PrusaSlicer_config_bundle.ini`.

### Importing the Config Bundle
To import the config bundle into PrusaSlicer, follow these steps:

1. Open PrusaSlicer.
2. Go to `File > Import > Import Config Bundle ...`.
3. Navigate to the location of the `Jubilee_PrusaSlicer_config_bundle.ini` file and select it.

This will load the configuration settings for the Jubilee printer into PrusaSlicer.

![Import Config](import_config_bundle.png)

### Load and Slice the Model
After installing and configuring PrusaSlicer, you can load your 3D model into the software. To do this, click on the 'Add' button on the top and select your model file in `.stl`. Once the model is loaded, you can adjust its orientation and scale if necessary.

#### Printing and slicing parameters

We are printing with Pluronic F127 hydrogel (25 wt%). It is a gel at room temperature but liquifies at cooler temperature. The slicer bundle is set up to let you print with a 18 gauge nozzle (green). You can experiment with printing parameters to yield different results. The parameters and settings can be access by clicking on the gear icons on the right when you're inside of the `Plater` tab or by clicking on the corresponding tabs on top. When you are on any of the `Settings` tab, you can use `cmd + F` or `ctrl + F` to quickly locate a parameter.

**Nozzle diameter** allows you to use different size of nozzles to achieve different resolution. It is under `Printer Settings`. We provide a range of nozzle sizes and you can look at their `Needle Nominal ID` from [this chart](https://www.hamiltoncompany.com/laboratory-products/needles-knowledge/needle-gauge-chart).
If you change the nozzle diameter, you may also want to change your **Extrusion width** under `Print Settings > Advanced`. Again, you can quickly locate this setting by using the search hot key.

**Speed** under `Print Settings` is tied to the viscosity of the material. The default setting for F127 is 10 mm/s. If you chose to use a smaller nozzle, you may want to decrease the speed for print moves.

**Layer height/First layer height** under `Print Settings` affects your print quality and time. They should scale up and down with the nozzle size.

The rest is for you to explore!

### Slice & Export
Once you are happy with all the settings, click `Slice now` on the bottom right corner to generate a preview. The preview displays visual information such as infill pattern and tool path if you wish to examine them. Remember to `Export G-code` to generate the GCode file.

![Slice now](slice_now.png)

## Send the GCode to the Printer
Once you have your GCode, you can send it to the Jubilee printer. To do this, connect your computer to the printer and use the Duet Web Control interface to upload the GCode. A full manual about Duet Web Control can be found [here](https://docs.duet3d.com/User_manual/Reference/Duet_Web_Control_Manual).

With a tuned Jubilee, all you need to do is to upload the GCode file.

You can monitor the print to ensure that everything is going smoothly. If you notice any issues, you can pause or stop the print through the Duet interface.