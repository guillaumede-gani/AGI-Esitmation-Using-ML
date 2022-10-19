# Pulse Wave Analysis Using Machine Learning

This repositorie is a resume of the work I did on Photophletismography (PPG) waves during my month and a half position in a health tech compagnie. The idea of this project was to measure the Age Index[^1] (AGI).

To be more precise PPG waves in this application are measured my a finger Oximiter with a sampling rate of 50HZ. The AGI is measured using the second derivative of the original PPG wave this wave is commonly noted SDPTG. Using this wave we isolated on a single pulse 5 fiducial points as show in the graph bellow :



![](https://user-images.githubusercontent.com/46630171/196576717-ce670947-901c-4565-8eb4-7f37c955e527.jpg) |
:-------------------------:|
Fig 1[^2]

The method described above was done on pressure waveforms digitized at the sample acquisition frequency of 500Hz[^2]. This higher frequency of sampling has a cascading effect reducing drastically the ammount of noise on the second derivative since derivating signals increases the noise at each step.


### Machin Learning Approach

The methodology used to estimate the AGI on low sampling frequency signals is quite simple. The first step was to find a large ammount of high quality data with a high sampling frequency. The dataset was found on Peter H Charlton website[^3] where a collection of various PPG waves datasets are available.





## References
[^1]: Takazawa K, Tanaka N, Fujita M, et al. Assessment of vasoactive agents and vascular aging by the second derivative of photoplethysmogram waveform. Hypertension. 1998
[^2]: Bortolotto LA, Blacher J, Kondo T, Takazawa K, Safar ME. Assessment of vascular aging and atherosclerosis in hypertensive subjects: second derivative of photoplethysmogram versus pulse wave velocity. Am J Hypertens. 2000
[^3]: https://peterhcharlton.github.io/
