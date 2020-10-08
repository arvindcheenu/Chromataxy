# 🌈 Chromataxy

**Chromataxy** (abbreviated ***coxy***) is a perceptually intuitive **c**olor **n**aming **s**ystem based on the ***Lightness-Chroma-Hue*** *color space* that covers a sizeable spectrum of colors while boasting a negligible learning curve.
 
 ### Features

* Over **3 lakh** named colors and **2.3 million utility classes**
* **Perceptually uniform**<sup>[1]</sup> colours
* **Semantically sound** names
* **ii8n**<sup>[2]</sup> friendly 
* **Accessible** by design

### Why not other Color Spaces?

* **HSL**  While this transformation of RGB color space is more intuitive in its representation, the *lightness* in *HSL* does *not* represent *perceptual lightness* but rather *relative brightness*.
* **Munsell**  : While colors were loosely based on perception, they were mostly inconsistent and dependent on the environment. Moreover, quantitative differences could only be defined over a single color attribute<sup>[3]</sup>.
* **NCS** : Based on the psychophysics of color perception, *NCS* is better than *Munsell* as environmental lighting conditions do not impact color choices. However, this system must not be used to model perceived color differences<sup>[4]</sup>, which is necessary requirement for a naming system to be accessible.
* **LAB** : Though the *CIELAB* color space represents a broader color gamut with better perceptual accuracy than the *Munsell* System, the parameters **a*** and **b*** makes it harder to arrive at a mental model.

### Designing the Nomenclature of Color

To ensure that the naming system is semantically intuitive and accessible, simple adjectives suffixed with their positive, comparative and superlative forms were used to describe the different dimensions of color.

#### Degrees of Hue Table

All the numbers have units in degrees (not radians). This naming method adds an additional dimension of **temperature** to distinguish transitional colours between two hues, effectively **naming a hue for every *3° rotation***. In this table, *Base* denotes only the root colour without a describing adjective being attached to it. The base color names are generated from the nearest equivalents in [**Named HTML CSS Colors**](http://www.htmlcsscolor.com/).

| **Colour**         | **Coolest** | **Cooler** | **Cool** | **Base** | **Warm** | **Warmer** | **Warmest** |
| ------------------ | ----------- | ---------- | -------- | -------- | -------- | ---------- | ----------- |
| **CeriseRed**      | 1           | 4          | 7        | 10       | 13       | 16         | 19          |
| **CinnabarRed**    | 21          | 24         | 27       | 30       | 33       | 36         | 39          |
| **FieryOrange**    | 41          | 44         | 47       | 50       | 53       | 56         | 59          |
| **CopperOrange**   | 61          | 64         | 67       | 70       | 73       | 76         | 79          |
| **LuxorGold**      | 81          | 84         | 87       | 90       | 93       | 96         | 99          |
| **OliveGreen**     | 101         | 104        | 107      | 110      | 113      | 116        | 119         |
| **ForestGreen**    | 121         | 124        | 127      | 130      | 133      | 136        | 139         |
| **AppleGreen**     | 141         | 144        | 147      | 150      | 153      | 156        | 159         |
| **SeaGreen**       | 161         | 164        | 167      | 170      | 173      | 176        | 179         |
| **TealGreen**      | 181         | 184        | 187      | 190      | 193      | 196        | 199         |
| **PacificBlue**    | 201         | 204        | 207      | 210      | 213      | 216        | 219         |
| **CuriousBlue**    | 221         | 224        | 227      | 230      | 233      | 236        | 239         |
| **DodgerBlue**     | 241         | 244        | 247      | 250      | 253      | 256        | 259         |
| **AzureBlue**      | 261         | 264        | 267      | 270      | 273      | 276        | 279         |
| **RoyalBlue**      | 281         | 284        | 287      | 290      | 293      | 296        | 299         |
| **AmethystPurple** | 301         | 304        | 307      | 310      | 313      | 316        | 319         |
| **FuchsiaPink**    | 321         | 324        | 327      | 330      | 333      | 336        | 339         |
| **CerisePink**     | 341         | 344        | 347      | 350      | 353      | 356        | 359         |

This results in a whopping **126 hue variations per combination** of chroma and lightness. 

#### Chroma Table

The chroma range **(0 - 100)** is split into **12** (3 forms of 4 comparative adjectives each) **adjectives** with **2** extra stops for denoting *gray* and *base* colors totalling **14 segments**. In this table, *Base* denotes only the root colour without a describing adjective being attached to it.

| **Chroma** | **Names** |
| ---------- | --------- |
| 0          | Gray      |
| 9.25       | Gloomiest |
| 18.5       | Gloomier  |
| 27.75      | Gloomy    |
| 37         | Dullest   |
| 46.25      | Duller    |
| 55.5       | Dull      |
| 66         | Base      |
| 71.65      | Deep      |
| 77.3       | Deeper    |
| 82.95      | Deepest   |
| 88.6       | Vivid     |
| 94.25      | Vivider   |
| 99.9       | Vividest  |

#### Lightness Table

The lightness range **(0 - 100)** is split into **12** (3 forms of 4 comparative adjectives each) **adjectives** with **4** extra stops for denoting *white*, *black* and *base* colors totalling **15 segments**. In this table, *Base* denotes only the root colour without a describing adjective being attached to it.

**Rationale** : Among the 4 chosen adjectives, 2 adjectives (*dark* and *dim*) are used to denote the *shades* of a color while the other 2 (*pale* and *bright*) are used to denote the *tints*. Here, the adjectives describe the lighting of a windowless room  (a room without an external light source). Hence, *black* corresponds to a pitch black room  with walls painted with 100% light-absorbing paint and vice versa.

| **Lightness (in Degrees)** | **Name**  |
| -------------------------- | --------- |
| 0                          | Black     |
| 7.25                       | Darkest   |
| 14.5                       | Darker    |
| 21.75                      | Dark      |
| 29                         | Dimmest   |
| 36.25                      | Dimmer    |
| 43.5                       | Dim       |
| 50.75                      | Base      |
| 58                         | Pale      |
| 65.25                      | Paler     |
| 72.5                       | Palest    |
| 79.75                      | Bright    |
| 87.5                       | Brighter  |
| 95.25                      | Brightest |
| 100                        | White     |

#### Alpha Table

The alpha range **(0 - 100)** is split into **9** (3 forms of 3 comparative adjectives each) **adjectives** with **2** extra stops for denoting *transparent* and *base* colors totalling **11 segments**. In this table, *Base* denotes only the root colour without a describing adjective being attached to it.

**Rationale** : The adjectives chosen (*clear*, *misty* and *foggy*) indicate the appearance of a glass paned window under various weather conditions. Here, a perfectly clear window equates to a transparent color and vice versa.

| **Alpha (in Percentage)** | **Name**    |
| ------------------------- | ----------- |
| 0                         | Transparent |
| 10                        | Clearest    |
| 20                        | Clearer     |
| 30                        | Clear       |
| 40                        | Misty       |
| 50                        | Mistier     |
| 60                        | Mistiest    |
| 70                        | Foggy       |
| 80                        | Foggier     |
| 90                        | Foggiest    |
| 100                       | Base        |

Thus, each hue consists of **210 variations of Chroma and Lightness**. Given that there are **126 hues**, About  **26,460 named colors** can be derived. 

> To put that number in perspective, If you cycle through **every unique color** generated by coxy as your **daily desktop wallpaper**, it would approximately take you **72 years** to eventually run out of unique wallpapers..

If we factor in the additional dimension of **Transparency**, A staggering collection of **2,91,060 named colors** can be derived.

---

### Footnotes

[**1**]: *A system is perceptually uniform if a small perturbation to a component value is approximately equally perceptible across the range of that value*. In terms of colour spaces, a small degree of change between hues across the range (0°-360°) correspond to a similar increase in chroma and lightness that are perceptually equivalent under natural vision.

[**2**]: Abbreviation for Internationalisation, which in this context, refers to multilingual compatibility.

[**3**]: Modern Color Models - Munsell Color System. http://www.handprint.com/HP/WCL/color7.html#MUNSELL

[**4**]: Modern Color Models - Swedish Natural Color System. http://www.handprint.com/HP/WCL/color7.html#NCS 
