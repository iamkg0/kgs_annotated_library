### My annotated library
I am not a fan of Mendeley, though I value the tool, but I dont like to click twice to see the annotation and, generally speaking, find myself not reading articles i add to mendeley too often, i've decided to create my own one here... with some sorta dataset which i might work with somehow later on idk. </br>
feel free to read, if you found it somehow </br>
Notice that everything i write is for personal use so pay no attention if there is anything confusing or rude </br>
Readme contains citations and my descriptions of articles i've read </br>

## bio
1. ``Paper:`` Donner, K., & Yovanovich, C. A. M. (2020). A Frog’s Eye View: Foundational Revelations and future promises. Seminars in Cell &amp; Developmental Biology, 106, 72–85. https://doi.org/10.1016/j.semcdb.2020.05.011 <br/>
``Description:`` starts with some advanced info regarding pigments, then briefly about electroretinography and visually-guided behavior. A bit of pictures <br/>
``Opinion:`` i found it difficult to read. However, includes a lot of useful references, which makes this article useful itself <br/>
2. ``Paper:`` Schleidt, W., Shalter, M. D., & Moura-Neto, H. (2011). The Hawk/Goose Story: The classical ethological experiments of Lorenz and Tinbergen, revisited. Journal of Comparative Psychology, 125(2), 121–133. https://doi.org/10.1037/a0022068 <br/>
``Description:`` the story behind hawk/goose effect, well described. It appears that not the exact pattern is important after all - it is more about rarity of specific dynamic pattern, including same object moving in opposite directions. Then some psychological stuff went on so I stopped reading tbh <br/>
``Opinion:`` Quite useful to know <br/>
3. ``Paper:`` Rozenblit, F., & Gollisch, T. (2020). What the Salamander Eye has been telling the vision scientist’s brain. Seminars in Cell &amp; Developmental Biology, 106, 61–71. https://doi.org/10.1016/j.semcdb.2020.04.010 <br/>
``Description:`` a comprehensive review on salamander vision system - some historical background, retina features (including comparison of photoreceptors between species, and some properties of photoreceptors themselves), a bit of higher levels of vision. Contains a lot of useful references. Some info about dynamic patterns as well, but not too much. Might need to check the sources they refer to - authors briefly dedscribed an experiment where salamanders vision had been reversed by rotating eyes <br/>
``Opinion:`` interesting, even entertaining. An excellent paper, and very useful <br/>
4. ``Paper:`` Sperry, R. W. (1943). Effect of 180 degree rotation of the retinal field on Visuomotor Coordination. Journal of Experimental Zoology, 92(3), 263–279. https://doi.org/10.1002/jez.1400920303 <br/>
``Description:`` newts' retinas were rotated 180 degrees. There were different experimental groups, but in general such details are not that essential (control group was blind). Briefly, their optokinetics was reversed, and remained the same during 4.5 months of observation. Meanwhile, control group managed to adapt, thanks to other perceptual systems (like olfactory and shit). There's also some info about morphological changes (their skin color), but it doesnt seem relevant to me. More detes in the article. <br/>
``Opinion:`` interesting that there was lack of plasticity. I wonder if there are any similar researches <br/>
5. ``Paper:`` Sperry, R. W. (1943c). Visuomotor coordination in the newt (triturus viridescens) after regeneration of the optic nerve. Journal of Comparative Neurology, 79(1), 33–55. https://doi.org/10.1002/cne.900790104 <br/>
``Description:`` Continuation of [5], except this time optic nerve was cut. It regenerated (links to previous works in the article), but newts vision was still reversed. Contains huge discussion part <br/>
``Opinion:`` Now I wonder if there is anything like that done on primates, or any revisits of this work in terms of systems neuroscience <br/>
6. ``Paper:`` <br/>
``Description:`` <br/>
``Opinion:`` <br/>

## SNNs
1. ``Paper:`` <br/>
``Description:`` <br/>
``Opinion:`` <br/>

## Event cams
1. ``Paper:`` <br/>
``Description:`` <br/>
``Opinion:`` <br/>

## SNNs + Event cams
1. ``Paper:`` Chen, X., Su, L., Zhao, J., Qiu, K., Jiang, N., & Zhai, G. (2023). Sign language gesture recognition and classification based on event camera with spiking neural networks. Electronics, 12(4), 786. https://doi.org/10.3390/electronics12040786 <br/>
``Description:`` Authours state that using traditional CNN methods require event data to become frame-based, like RGB data, which is a significant drawback - lost of asynchronous data benefits, which is one the main reasons of event-based vision to exist. They've investigated some sign language datasets and created their own event collection with DAVIS346 camera. STBP method was used to train an SNN. The article contains a fairly simple explaination of the algorithm underlying the principle of event-camera. Dataset was created using v2e method + DAVIS346 for better validation - 64 classes (verbs and nouns). The model - LIF-based conv SNN, freq coding, trained with STBP (spatio-temporal backprobagation) algorithm. They used pool, conv, LIF and fc in the architecture (not quite biologically realistic, obviously). Literally, LIF layers serve as temporally assymetrical ReLU. Description of the whole work is quite comprehensive, including v2e explaination, so it might be easy to reproduce. The model is built with Pytorch, optimized with SGD. Somehow, v2e shows better accuracy, compared with native event recordings (77% and 68%, respectively). <br/>
``Opinion:`` 2/3-gen NNs - not the approach i'm looking for. Still, some info might come in handy <br/>
2. ``Paper:`` Zhang, Y., Lv, H., Zhao, Y., Feng, Y., Liu, H., & Bi, G. (2023). Event-based optical flow estimation with spatio-temporal backpropagation trained spiking neural network. Micromachines, 14(1), 203. https://doi.org/10.3390/mi14010203 <br/>
``Description:`` The idea of the paper is to introduce an SNN for discrete spatio-temporal stream of events (basically, slices of events), reducing the amount of computation (the also show the slicing method (their own, but from previous work - doi.org/10.3390/s22072614). As far as i've understood, the method is sensitive to amount of events, the more events - the shorter the slice. But i kinda doubt it, regarding their equation. Haven't dug the topic yet, so you better check it out yourself). For self-supervised learning they generate grayscale image with the event stream. The model is an autoencoder, implemented with Pytorch and trained with Adam optimizer. Authors also provide benchmarks for computational costs and prediction results with different slicing methods. <br/>
``Opinion:`` So far, this work seems questionable to me. Perhaps it is because i'm new to event cameras, but i see no reason to divide a single slice of data into two channels (ON/OFF) just to feed the first one-channel layer of the same size. <br/>
3. ``Paper:`` <br/>
``Description:`` <br/>
``Opinion:`` <br/>