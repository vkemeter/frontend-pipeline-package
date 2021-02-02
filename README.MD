# frontend pipeline package 

1. clone this repository
2. remove git folder
3. yarn install
4. modify config.js paths for your need
    1. build: is the path where your package.json is located
    2. theme is the path, where your TYPO3 package is located
    3. webRoot is you public WebRoot path
5. modify config.yaml breakpoints and possible file exports for your need.
    1. possible exports are:
        1. scss
        2. constantsts
        3. yaml

the yaml file for the aspect ratio is mainly used for the CropVariantsBuilder Extension
from Josef Glatz (https://github.com/josefglatz/cropvariantsbuilder/). this file can be imported
in the crop variants yaml config file.

e.g.: 

```
imports:
     -
       resource: 'EXT:your_ext/Configuration/ImageManipulation/Imports/aspect-ratios.yaml'
```        

you are ready to go.

Includes the FE-Pipeline Main Package with following Features:

* bootstrap: 4.5.3
* family.scss: 1.0.8
* gulp: 4.0.2
* jquery: 3.5.1
* backstopjs

and a few more.