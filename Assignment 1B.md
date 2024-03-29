# Assignment 1B:

### What are Channels and Kernels (according to EVA)?

#### Channels:
```
A channel is a collection of similar feature bags. For example: when we go to a supermarket and look for fruits section. Then we find that there are many fruits available, for example: apples, oranges, grapes, etc. So, just to understand the concept of channels, we can think of each fruits as a separate channels, apple is a channel, orange is a different channel and so on.

```

#### Kernels:
```
Kernels are nothing but feature extractors. In a CNN, they are automatically (through backpropagation) selected to extract the features from an image.

```

### Why should we only (well mostly) use 3x3 Kernels?
```
It is advised but not mandatory to use 3X3 kernels because of 2 reasons:
(i) We can construct kernels of different sizes like: 5X5, 7X7, 9X9, etc. from 3X3 kernel.
(ii) We should use kernels with odd dimensions because, they are symmetric around the origin or better we say anchor pixel. It is possible to use even dimensional kernels but then we won't be having this symmetry. We use kernels based on gaussian function, in which the top value is achieved on the axis of symmetry. This is the main reason why such kinds of kernels are preferably to be odd but we not bound to it. We may use rectangular kernels as well.

```
### How many times do we need to perform 3x3 convolution operation to reach 1x1 from 199x199 (show calculations)?
We will have to do convolution operation for 100 times.
The calculation would be like as shown below:
```
(199X199)|(3X3)|(197X197)|(3X3)|(195X195)|(3X3)|(193X193)|(3X3)|(191X191)|(3X3)|(189X189)|(3X3)|(187x187)|(3X3)|(185X185)|(3X3)|(183X183)|(3X3)|(181X181)|(3X3)|(179X179)|(3X3)|(177X177)|(3X3)|(175X175)|(3X3)|(173X173)|(3X3)|(171X171)|(3X3)|(169X169)|(3X3)|(167X167)|(3X3)|(165X165)|(3X3)|(163X163)|(3X3)|(161X161)|(3X3)|(159X159)|(3X3)|(157X157)|(3X3)|(155X155)|(3X3)|(153X153)|(3X3)|(151X151)|(3X3)|(149X149)|(3X3)|(147X147)|(3X3)|(145X145)|(3X3)|(143X143)|(3X3)|(141X141)|(3X3)|(139x139)|(3X3)|(137X137)|(3X3)|(135X135)|(3X3)|(133X133)|(3X3)|(131X131)|(3X3)|(129X129)|(3X3)|(127X127)|(3X3)|(125X125)|(3X3)|(123X123)|(3X3)|(121X121)|(3X3)|(119X119)|(3X3)|(117X117)|(3X3)|(115X115)|(3X3)|(113X113)|(3X3)|(111X111)|(3X3)|(109X109)|(3X3)|(107X107)|(3X3)|(105X105)|(3X3)|(103X103)|(3X3)|(101X101)|(3X3)|(99X99)|(3X3)|(97X97)|(3X3)|(95X95)|(3X3)|(93X93)|(3X3)|(91x91)|(3X3)|(89X89)|(3X3)|(87X87)|(3X3)|(85X85)|(3X3)|(83X83)|(3X3)|(81X81)|(3X3)|(79X79)|(3X3)|(77X77)|(3X3)|(75X75)|(3X3)|(73X73)|(3X3)|(71X71)|(3X3)|(69X69)|(3X3)|(67X67)|(3X3)|(65X65)|(3X3)|(63X63)|(3X3)|(61X61)|(3X3)|(59X59)|(3X3)|(57X57)|(3X3)|(55X55)|(3X3)|(53X53)|(3X3)|(51X51)|(3X3)|(49X49)|(3X3)|(47X47)|(3X3)|(45X45)|(3X3)|(43x43)|(3X3)|(41X41)|(3X3)|(39X39)|(3X3)|(37X37)|(3X3)|(35X35)|(3X3)|(33X33)|(3X3)|(31X31)|(3X3)|(29X29)|(3X3)|(27X27)|(3X3)(25X25)|(3X3)|(23X23)|(3X3)|(21X21)|(3X3)|(19X19)|(3X3)|(17X17)|(3X3)|(15X15)|(3X3)|(13X13)|(3X3)|(11X11)|(3X3)|(9X9)|(3X3)|(7X7)|(3X3)|(5X5)|(3X3)|(3X3)|(3X3)|(1X1)

```
