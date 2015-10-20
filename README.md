![](https://github.com/marcoalopez/GrainSizeTools/blob/05837e74bb371c34c5257e869bfd363c069b9c4d/FIGURES/header_fig.png?raw=true)

[GrainSizeTools](https://sourceforge.net/projects/grainsizetools/) is a free open-source cross-platform script written in [Python][1] that provides a number of tools with the aim of characterizing the grain size and the population of grain sizes in dynamically recrystallized mylonites. The script is suitable to use in paleopiezometry studies, using different 1D grain size measures, as well as to derive the actual 3D population of grain sizes from 2D data (*i.e.* thin sections). The script only requires the previous measurement of the grain sectional areas from a thin section. There is **no need** of previous knowledge of Python language to use the script and get the results (see [documentation][2]). For advanced users, the script is organized in a modular way using Python functions, which facilitates to modify, reuse or extend the code if needed.

Features
-------------

- It allows to load and automatically extract data of interest from txt and csv files generated by the ImageJ or similar applications.
- It allows to calculate the apparent diameters of the grain profiles from their sectional areas via the equivalent circular diameter. Also, it allows to correct the diameters calculated by adding the perimeter of the grains.
- It allows to easily estimate different 1D grain sizes for paleopiezometry studies, including the mean, the median, the area-weighted mean and the frequency peak grain sizes of the apparent population of grain sizes.
- It implements several algorithms to estimate the optimal bin size of histograms and the optimal bandwidth of the Gaussian KDE based on the population features.
- It allows to estimate the actual 3D populations of grains from the population of apparent (2D) grain sizes using a variant of the Scheil-Schwartz-Saltykov method to unfold the apparent grain size population. Similar to what the *StripStar* script does. It also returns an estimation of the volume of a particular grain fraction defined by the user.
- In the case of completely dynamically recrystallized samples, it also allows to estimate the best-fit log-normal probability density function to the 3D population of grain sizes by estimating the best-fit optimal shape and scale parameters using the two-step method (Lopez-Sanchez and Llana-Fúnez, submitted).
- It produces a number of different ready-to-publish plots, allowing to save the graphical output as a bitmap or vector images. The script include the following plots: i) the number- and area-weighted population of apparent grain sizes, ii) the frequency and volume-weighted cumulative frequency population of the derived 3D grain size population, and iii) the best-fit log-normal probability density function to the derived 3D grain size population with errors.

Screenshots
-------------
*(available soon)*

Download
-------------

You can download the script in the following sites:  
https://github.com/marcoalopez/GrainSizeTools/releases 
http://figshare.com/articles/GrainSizeTools_script/1383130

Documentation
-------------
Take a look at the [table of contents](https://github.com/marcoalopez/GrainSizeTools/blob/master/DOCS/tableOfContents.md). You can also get a manual in pdf format [here](http://figshare.com/articles/GrainSizeTools_script_manual/1371025), which makes it readily available for offline reading.


Citation guidelines
-------------

####Software reference
Lopez-Sanchez, Marco A. (2015): GrainSizeTools script. figshare. http://dx.doi.org/10.6084/m9.figshare.1383130

####Technique reference:
***Frequency peak grain size based on Gaussian KDE***
Lopez-Sanchez MA and Llana-Fúnez S (2015) An evaluation of different measures of dynamically recrystallized grain size for paleopiezometry or paleowattometry studies. *Solid Earth* 6, 475-495. doi:[10.5194/se-6-475-2015](http://dx.doi.org/10.5194/se-6-475-2015)

***Saltykov and the two-step method***
Lopez-Sanchez MA and Llana-Fúnez (2015) Deriving 3D grain size distributions from thin sections in mylonites: strategy, presentation format and error considerations. To submit soon.

License
-------------
see [GNU Library or Lesser General Public License version 3.0 (LGPLv3)](https://github.com/marcoalopez/GrainSizeTools/blob/master/license.txt)



 [1]: https://www.python.org/
 [2]: https://github.com/marcoalopez/GrainSizeTools/blob/master/DOCS/tableOfContents.md
