# How to 3D Print Prosethetic Ears

## Downloading Files & Presets
  Download the appropriate files in the **models** folder. I have included a couple different template versions that you can choose from, and they are all in the .3mf file, which can be directly exported to Bambu Studio. After downloading the file and opening it in Bambu Studio, download the appropriate **print preset** and **filament preset** and import it to the Bambu slicer. 
  The presets I have included in the PrintPreset folder is for the Filaflex 82a filament, which can be purchased here: 
  https://recreus.com/en-en/products/filaflex-82a?srsltid=AfmBOoqNMySuH6reLeulJEIT0YAuwA3GcN3e-P-xPYN-MZfMMSvyjS4r

  If you have a slightly different TPU or with a similar shore hardness, you could try using the presets, which should still work, but may need some fine tuning. If you are printing in PLA, normal settings should work fine since it is a lot less complex.

### Creating a Custom Ear
To create your own custom ear instead of using one of my presets is simple as well, simply follow the steps below
1. Download Polycam (mobile app)
2. Use Polycam’s  LiDAR scanning to render a human ear
3. Trim the rendering to only include the ear/necessary parts
4. Export as STL file, send to Fusion 360 or MeshMixer to patch/repair holes
5. Send STL file to MeshMixer (Online Application) to add a base/ make the render a solid
6. Export as 3MF file to Bambu Studio, adjust final settings, print.


## Printing
  To print, simply slice the plate with all the presets included, then press print plate to send it to your 3D Printer.
  As for the 3D Printers, I used the Bambu Labs A1 without AMS, which works fine. Other similar printers should work great too, just remember not to use AMS and just use the external spool, since TPU tends to clog and get stuck in the AMS tubes. 

### Printing Precautions
  One of the most important things about printing in TPU is **to print slow**. This is the most important setting no matter what type of TPU you are using, and I recommend trying to print at around 15-25 mm/s, just to get a high quality print. 
If you have any questions while printing, feel free to contact me at aurius.king@gmail.com
  
