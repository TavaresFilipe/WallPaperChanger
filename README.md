

<h1 align="center">
    WallPaperChanger 🖼️
</h1>
<hr>
<p align="center">
    <img src="https://img.shields.io/badge/os-linux%2C%20windows-blue.svg"> 
    <img src="https://img.shields.io/github/stars/yangman946/WallPaperChanger?color=ccf">
    <img src="https://img.shields.io/badge/license-MIT-dfd.svg">
    <img src="https://img.shields.io/github/contributors/yangman946/WallPaperChanger?color=9ea">
    
</p>

<p align="center">
    <img src=".github/images/wallpaper.jpeg" alt="wallpaper">
</p>

<br>

## Description ⛈️
This Python script changes your desktop wallpaper based on the weather.
<br>
<br>
  
## Cloning 🌀

`$ git clone https://github.com/yangman946/WallPaperChanger`
<br>
<br>

## Running ⚡
You need:
<ul>
  <li>install requirements: <code>pip install -r requirements.txt</code> </li>
  <li>Image url for weather widget: customise your own widget here: https://www.theweather.com/</li>
  <li>Your own api key for openweather: https://openweathermap.org/api </li>
</ul>


refer to `mainScript.py` for where to insert these values. 

<br>

You can run this script two ways:

<ul>
  <li>Via the <code>run.bat</code> script</li>
    <ul>
        <li>Change the first line CD {your file location} to the file location of <code>run.bat</code> </li>
        <li>and use Windows Task scheduler to periodically run the <code>run.bat</code> file. You could make the script run once every hour. </li>
        <li>Or import the provided .xml file into task scheduler (change path to your batch file)</li>
    </ul>
  <li>or Via the command line
    <ul>
      <li>CD to your directory</li>
      <li>run <code>python -m wallpaperChanger.mainScript</code> </li>
    </ul>
  </li>
</ul>

<br>
<br>

## Customising Wallpapers ✏️

Currently, the `mainScript.py` script supports the following weather states:
<ul>
  <li>Clear </li>
  <li>Mist (cloudy)</li>
  <li>Rain </li>
  <li>and thunder </li>
</ul>

<br>
You will find separate pairs of folders for each weather condition (day and night). 
These folders contain jpeg images (3936x2624 pixels) each labeled from 1 to the number of images in the folder. 
If you wish to replace images, ensure that:
<br>
<ul>
  <li>The images are of correct size (recommended 3936x2624 pixels)</li>
  <li>The images are in the correct folders</li>
  <li>The images are properly labelled {weather state}_{day state}_{image index} </li>
  <li>The images are jpeg images </li>
</ul>
<br>
<br>

To customise the layout of the wallpaper, refer to the `configurations` dictionary at `mainScript.py`.
Here, you can add custom layouts or use existing ones. Each layout requires six parameters:

<ol>
  <li>Coordinates of your widget (x, y)</li>
  <li>Day/date text location ("x", "y")</li>
    <ul>
        <li>"x": left, center or right </li>
        <li>"y": top, center or bottom </li>
    </ul>
  <li>show water mark (true, false)</li>
  <li>show compile time (true, false)</li>
  <li>Compile time location ("x", "y")</li>
    <ul>
        <li>"x": left, center or right </li>
        <li>"y": top, center or bottom </li>
    </ul>
  <li>Font</li>
    <ul>
        <li>Bold</li>
        <li>ExtraBold</li>
        <li>ExtraLight</li>
        <li>Italic</li>
        <li>Light</li>
        <li>Medium</li>
        <li>Regular</li>
        <li>Thin</li>
        <li>See all <a href = "https://github.com/yangman946/WallPaperChanger/tree/main/assets/fonts/Montserrat">fonts</a></li>
    </ul>
</ol>

## Contributing 👍

If you wish to contribute to this project, send a pull request, and I will look at it. Here’s an easy and quick [video guide](https://youtu.be/waEb2c9NDL8) for learning how to contribute via GitHub.

<br>
<br>

## TODO List ✔️

This project is a work in progress and will expect frequent updates.
<br>
<ul>
  <li>Expand wallpaper folders.</li>
  <li><s>Add a sunrise/sunset API to change the daystate. </s></li>
  <li>Add temperature conditions and assign certain wallpapers to temperature. </li>
  <li><s>Make the program run without appearing (invisible)</s></li>
</ul>

<br>
<br>

## Possible future improvements ✅
<br>
<ul>
  <li>Find a wallpaper API, reduces need for having folders full of images</li>
  <li>Show news or other information along with the weather.</li>
  <li>Export as an executable</li>
  <li><s>Make this project compatible with non-windows systems.</s></li>
</ul>

<br>
<br>
