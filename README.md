# COVID Data: An Exploration of Variants
____

Lindsey Uribe

*December 8, 2021*

Despite our tiring of COVID-19, and a desperate desire to return to "normal", it seems that COVID is not tiring of us. There is now a new COVID "variant of concern" that has been ramping up in Botswana and South Africa since early August of 2021. This new variant, *Omicron* (also known as *B.1.1.529*), has been found to have enough significant mutations as to cause the UK and United States to shut down flights incoming from South Africa$^{[\dagger]}$$^{[\star]}$. The predominant fear is that this variant has so many mutations that it will render all of our current vaccines ineffective, and a new flush of covid will spread throughout the globe once more, unimpeded by our most touted of solutions. For the majority of Americans, we've found ourselves at the sharp end of that solution, but does a vaccinated population actually have fewer covid variants? And how does the number of variants increase or decrease over time? 

According to the CDC, *“Vaccines remain the best public health measure to protect people from COVID-19, slow transmission, and reduce the likelihood of new variants emerging.”* $^{[\diamond]}$
Clearly, the CDC is arguing that vaccines do indeed have an effect on a reduction of opportunities for viral mutations, simply by a reduction in transmissibility of the virus. I can wrap my brain around that argument: the fewer people infected, the fewer hosts available in which a virus can undergo mutations, thus a reduced number of variants theoretically present in the population. But do the data support that argument? 

The two major questions that I want to explore: 
 - **Does an increasingly vaccinated population have any relationship to a reduction in the number of COVID variants present in a country?** This is a roundabout way of trying to take a crack at the question lots of people want answered: Do vaccines even matter? Would this variant have happened anyway, vaccines or no vaccines? Some might argue that vaccines have no effect on variants, but given the stance of the CDC, the official argument is that there is a reduction in the likelihood of novel variants creditable to vaccines.

 - **Does the number of variants detected in a population increase according to an exponential distribution?** In other words, is there any way I could try to predict the number of variants that might be present globally, just given some kind of timeframe? Without considering anything else, in just the simplest of terms, could I possibly figure out whether, in two years time, we will have say, 24 variants? 

<br>
_______

One very important note: The dataset `variants` is **not** the result of random sampling. The variants included here are those that have been detected via genomic sequencing across the globe and deemed to be "variants of concern" or "variants of interest". Considering that the accumulation of this dataset is the collective feat of the world, and it's just about as thorough as we humans can be on a global scale at this point in time, I have little choice but to treat this data as anything other than a census-like (albeit flawed) collection of genomic sequencing. Thus while performing my tests below, it's important to note that I am considering the *population* here to be the detectable traces of these variants themselves. In other words, the dataset *is* my population and I will be sampling randomly from that population. 
