Roman de la Rose
=================

A benchmark corpus for testing Rolling Stylometry methodology. It contains Roman de la Rose, a 13th-century French allegorical poem.

The corpus is aimed at stylometric benchmarks. See:
[https://computationalstylistics.github.io/](https://computationalstylistics.github.io/)
for further details.

To test the Rolling Stylometry method in no time using this corpus, download the files, open up your R shell, and type the following code:

``` R
library(stylo) 
setwd("path-to-the-locally-downloaded-repository-RdlR") 
```

Now, run the function `rolling.classify()`, use as many arguments as needed:

``` R
rolling.classify(write.png.file = TRUE, classification.method = "svm", mfw=100, training.set.sampling = "normal.sampling", slice.size = 5000, slice.overlap = 4500) 
```

Here’s the final results you should be getting:

![Roman de la Rose, analyzed by Rolling Stylometry with SVM as its kernel, and 100MFWs as stylistic features.](https://computationalstylistics.github.io/assets/img/rolling-svm_100-features_5000-per-slice.png)

