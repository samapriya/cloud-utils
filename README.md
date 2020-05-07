## **[cloud-utils: Cloud Utility for Planet's UMD-2](https://samapriya.github.io/cloud-utils/)** &nbsp; [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Try%20cloud-utils%20in%20#GoogleEarthEngine%20@planetlabs%20&url=https://github.com/samapriya/cloud-utils)

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)


**Please note: This tool is in no way an official tool or Planet offering, but is a personal project created and maintained by Samapriya Roy**

 Cloud utils are tools to work with [Planet's UDM-2 dataset](https://developers.planet.com/docs/data/udm-2/). The Usable Data Mask v2 are an 8 bit 8 band image with the following bands. These tools are designed as modules that can be imported directly into any Google Earth Engine script and can then be used in a plug and play manner.



 | Band   | Description     | Pixel Value Range | Interpretation                                                                         |
 |--------|-----------------|-------------------|----------------------------------------------------------------------------------------|
 | Band 1 | Clear map       | [0, 1]            | 0: not clear, 1: clear                                                                 |
 | Band 2 | Snow map        | [0, 1]            | 0: no snow or ice, 1: snow or ice                                                      |
 | Band 3 | Shadow map      | [0, 1]            | 0: no shadow, 1: shadow                                                                |
 | Band 4 | Light haze map  | [0, 1]            | 0: no light haze, 1: light haze                                                        |
 | Band 5 | Heavy haze map  | [0, 1]            | 0: no heavy haze, 1: heavy haze                                                        |
 | Band 6 | Cloud map       | [0, 1]            | 0: no cloud, 1: cloud                                                                  |
 | Band 7 | Confidence map  | [0-100]           | percentage value: per-pixel algorithmic confidence in classification                   |
 | Band 8 | Unusable pixels | --                | Equivalent to the UDM asset: see Planet's Imagery Specification for   complete details |
|   |   |   |   |   |

UDM-2 classification stems from a supervised machine learning technique and is designed to seperate the the above classes. Things to note:

* All classes are mutually exclusive meaning you can be either of the classes in Band-1 to Band -6
* The clases (Band-1 to Band-6) are binary as mentioned in the band list.
* The Confidence map value therefore refers to a single class and has a 1:1 correlation to the underlying imagery.

To read more about the [UDM-2 Classification Methodology you can go here at our Developers Center](https://developers.planet.com/docs/data/udm-2/#udm2-classification-methodology).

Eventually this will allow you to apply cloud masking to PlanetScope Scenes and their related UDM-2 masks to create cloud free composites.

![cloud_masking](https://user-images.githubusercontent.com/6677629/81248757-16c02880-8feb-11ea-9c0a-8cd174748d82.gif)

If you use this module, and find this tool useful, star and cite it as below

<b>
```

```
</b>

