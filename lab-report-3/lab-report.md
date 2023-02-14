# UCSD CSE15L Lab Report 3

Week 4 and 5 Labs

## Researching the command `grep`

> Souce used: https://linuxcommand.org/lc3_man_pages/grep1.html


### 1st Option: `-r`, `--recursive`

> This option will "read all files under each directory, recursively." 

> This is useful because you can search for the string pattern in all the subdirectories and files within the current directory.

**Example A**

*Input*

```shell
$ grep -r "Lucayans"
```

*Output*

```shell
$ grep -r "Lucayans"
travel_guides/berlitz2/Bahamas-History.txt:Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. Originally from South America, they had traveled up through the Caribbean islands, surviving by cultivating modest crops and from what they caught from sea and shore. Nothing in the experience of these gentle people could have prepared them for the arrival of the Pinta, the Niña, and the Santa Maria at San Salvador on 12 October 1492. Columbus believed that he had reached the East Indies and mistakenly called these people Indians. We know them today as the Lucayans. Columbus claimed the island and others in the Bahamas for his royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed for only two weeks before sailing towards Cuba.
travel_guides/berlitz2/Bahamas-History.txt:The Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that their galleons frequently passed through the archipelago en route to and from the Caribbean, Florida, Bermuda, and their home ports. On Eleuthera the explorers dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used to replenish the supplies of water on their ships before they began the long journey back to Europe with their cargoes of South American gold. As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were removed from the Bahamas to work — and die — in Spanish gold mines and on farms and pearl fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.
```

**Example B**

*Input*

```shell
$ grep -r "Test"
```

*Output*

```shell
$ grep -r "Test"
non-fiction/OUP/Berk/ch1.txt:Educational practice followed suit, moving back toward traditionalism. As Scholastic Aptitude Test (SAT) scores of American high school graduates plummeted and concern over the academic preparation of American children and youths became widespread, a “back to basics” movement arose that, by 1980, was in full swing. Academic preschools ﬂourished, and kindergarten and primary classrooms returned to whole-class, teacher-directed instruction relying heavily on workbooks and frequent grading, a style still prevalent today.43 
non-fiction/OUP/Fletcher/ch1.txt:This view of the relationship between law and redemption finds expression in the Hebrew Bible, the Old Testament. It continues to inspire the law-based thinking of Judaism, Islam, the Catholic Church, and some Protestant theologians. The law given at Sinai, the law embedded in the covenant, is not the expression of individual aspiration but only of collective obligation. Seeking redemption or salvation through the church or through faith provides a way of cleansing ourselves of sin and, as it were, perfecting our individual creation.
non-fiction/OUP/Kauffman/ch10.txt:Loose arguments? Yes. Testable? Here and there. Wrong? Probably. Deeply wrong? Maybe not. Does this get the universe to the edge of expansion versus contraction or to a flat universe expanding forever more rapidly? I would love it to be so. Indeed, I would love a view in which matter, energy, and geometry can all interconvert. After all, if geometry, the vacuum, has energy, such interconversion does not seem impossible. Do the considerations of this chapter require detailed models and supporting calculations to be taken as more than the merest suggestions? Absolutely. This chapter, like much of Investigations, is protoscience. But science grows from serious protoscience, and I take Investigations to be serious protoscience.
travel_guides/berlitz1/HistoryGreek.txt:        the final book of the New Testament, the Book of Revelation. It wasn’t
travel_guides/berlitz1/HistoryLasVegas.txt:        Nellis Air Force Base and the Nevada Test Site) in the north, and Basic
travel_guides/berlitz1/WhereToFrance.txt:        deliberately elongated sculptures of Old Testament figures contrast
travel_guides/berlitz1/WhereToFrance.txt:        more than 400 scenes from the Old and New Testaments, 3,650 fig­ures
travel_guides/berlitz1/WhereToFrance.txt:        More than 200 Old and New Testament figures are sculpted
travel_guides/berlitz1/WhereToGreek.txt:        Testament.
travel_guides/berlitz1/WhereToItaly.txt:        mosaics, glittering Old Testament scenes high on the walls (don’t
travel_guides/berlitz1/WhereToItaly.txt:        Testament. Michelangelo said the latter, facing the Duomo, were good
travel_guides/berlitz1/WhereToItaly.txt:        Duomo none the less) for its dramatic frescoes of New Testament scenes
travel_guides/berlitz1/WhereToItaly.txt:        Testament and the Last Judgment.
travel_guides/berlitz1/WhereToItaly.txt:        the upper tier illustrate scenes from the Old and New Testament.
travel_guides/berlitz1/WhereToItaly.txt:        eighth being the choir and apse. The Old Testament scenes, such as
travel_guides/berlitz1/WhereToItaly.txt:        churches. It has a fine central portal with reliefs of Old Testament
travel_guides/berlitz1/WhereToItaly.txt:        the collection, the sketch of a young girl, Testa di Fanciulla, by
travel_guides/berlitz1/WhereToItaly.txt:        nave and apse depict the complete cycle of the Old Testament, replete
travel_guides/berlitz1/WhereToJerusalem.txt:        Solomon reigned and where the Old Testament prophets walked, was
travel_guides/berlitz1/WhereToJerusalem.txt:        by orchards, banana plantations, kibbutzim, and Old and New Testament
travel_guides/berlitz1/WhereToJerusalem.txt:        Galilee are some of the sites where, according to New Testament
travel_guides/berlitz1/WhereToMadrid.txt:        tiers, depicts New Testament stories in fervent detail. Just behind the
travel_guides/berlitz2/Amsterdam-WhereToGo.txt:Running parallel to Jodenbreestraat on the left-hand side is Waterlooplein, named after the famous battle and home to the famous flea market of the same name. Every day you’ll find an eclectic mix of second-hand crockery, clothes, and electrical equipment on sale, along with cotton clothes from India or Indonesia. The eastern end of the market square is dominated by the twin spires of Mozes en Aäronkerk (Moses and Aaron Church), a Catholic Church built in 1840 on the site of a secret chapel. The Old Testament figures of Moses and Aaron were found depicted on gable stones in the original building and were set into the wall of the new edifice. The fine towers are actually wood rather than stone. They were painted to match the sandstone walls in a 1990 restoration.
travel_guides/berlitz2/Boston-WhereToGo.txt:Except for quotations on the walls from the New Testament and Christian Science founder, Mary Baker Eddy, there’s no decoration. Some stained glass windows are found in the older church, which also contains founder Mary Baker Eddy’s chair. She only addressed the congregation twice, as she wished to avoid any personal idolatry. A guided tour is highly recommended (you can only visit the original church by joining a tour).
travel_guides/berlitz2/Canada-WhereToGo.txt:European Collections. Among the most important works from the 14th to the 18th centuries are Simone Martini’s St. Catherine of Alexandria, Cranach’s Venus, Hans Baldung Grien’s Eve, the Serpent and Death, Hans Memling’s Virgin, Christ and St. Anthony, Bronzino’s Portrait of a Man, Annibale Carracci’s Vision of St. Francis, Poussin’s Landscape with a Woman Washing Her Feet, Rubens’ Entombment of Christ, Rembrandt’s Heroine from the Old Testament, and Chardin’s The Governess.
travel_guides/berlitz2/Canada-WhereToGo.txt:The area around this old coalmining town is famous for the prehistoric fossils and remarkably complete remains of dinosaurs whose stamping grounds were the Badlands of the Red Deer River Valley. The 130-km (78-mile) drive northeast of Calgary on Highway 9 takes you through wheat-growing country where you may see the farming communities of Hutterites, an austere religious sect originally from Slovakia, often persecuted for their pacifism. The women wear traditional dirndl costumes with headscarf and apron, while their husbands, dressed all in black with broad-rimmed hats, cultivate the heavy beards of Old Testament prophets.
travel_guides/berlitz2/China-WhereToGo.txt:Closer to the city center is Fuboshan (“Whirlpool Hill”) another natural stone tower with a view as well as other distractions. According to legend, a General Fubo, who passed this way 2,000 years ago, tested his sword in the Sword-Testing Stone, a stalactite formation that comes down to within inches of the ground. Further on, the Thousand Buddha Cliff is carved with several hundred figures dating from the Tang and Song dynasties.
```


### 2nd Option: `-c`, `--count`

> This option will "suppress normal output; instead print a count of matching lines for each input file." 

> This is useful because you can see the number of times the string pattern appears in a given file.

**Example A**

*Input*

> Combined with `-r` to search all subdirectories:

```shell
$ grep -r -c "Lucayans"
```

*Output*

```shell
$ grep -r -c "Lucayans"
non-fiction/OUP/Abernathy/ch1.txt:0
non-fiction/OUP/Abernathy/ch14.txt:0
non-fiction/OUP/Abernathy/ch15.txt:0
non-fiction/OUP/Abernathy/ch2.txt:0
non-fiction/OUP/Abernathy/ch3.txt:0
non-fiction/OUP/Abernathy/ch6.txt:0
non-fiction/OUP/Abernathy/ch7.txt:0
non-fiction/OUP/Abernathy/ch8.txt:0
non-fiction/OUP/Abernathy/ch9.txt:0
non-fiction/OUP/Berk/CH4.txt:0
non-fiction/OUP/Berk/ch1.txt:0
non-fiction/OUP/Berk/ch2.txt:0
non-fiction/OUP/Berk/ch7.txt:0
non-fiction/OUP/Castro/chA.txt:0
non-fiction/OUP/Castro/chB.txt:0
non-fiction/OUP/Castro/chC.txt:0
non-fiction/OUP/Castro/chL.txt:0
non-fiction/OUP/Castro/chM.txt:0
non-fiction/OUP/Castro/chN.txt:0
non-fiction/OUP/Castro/chO.txt:0
non-fiction/OUP/Castro/chP.txt:0
non-fiction/OUP/Castro/chQ.txt:0
non-fiction/OUP/Castro/chR.txt:0
non-fiction/OUP/Castro/chV.txt:0
non-fiction/OUP/Castro/chW.txt:0
non-fiction/OUP/Castro/chY.txt:0
non-fiction/OUP/Castro/chZ.txt:0
non-fiction/OUP/Fletcher/ch1.txt:0
non-fiction/OUP/Fletcher/ch10.txt:0
non-fiction/OUP/Fletcher/ch2.txt:0
non-fiction/OUP/Fletcher/ch5.txt:0
non-fiction/OUP/Fletcher/ch6.txt:0
non-fiction/OUP/Fletcher/ch9.txt:0
non-fiction/OUP/Kauffman/ch1.txt:0
non-fiction/OUP/Kauffman/ch10.txt:0
non-fiction/OUP/Kauffman/ch3.txt:0
non-fiction/OUP/Kauffman/ch4.txt:0
non-fiction/OUP/Kauffman/ch5.txt:0
non-fiction/OUP/Kauffman/ch6.txt:0
non-fiction/OUP/Kauffman/ch7.txt:0
non-fiction/OUP/Kauffman/ch8.txt:0
non-fiction/OUP/Kauffman/ch9.txt:0
non-fiction/OUP/Rybczynski/ch1.txt:0
non-fiction/OUP/Rybczynski/ch2.txt:0
non-fiction/OUP/Rybczynski/ch3.txt:0
travel_guides/berlitz1/HandRHawaii.txt:0
travel_guides/berlitz1/HandRHongKong.txt:0
travel_guides/berlitz1/HandRIbiza.txt:0
travel_guides/berlitz1/HandRIsrael.txt:0
travel_guides/berlitz1/HandRIstanbul.txt:0
travel_guides/berlitz1/HandRJamaica.txt:0
travel_guides/berlitz1/HandRJerusalem.txt:0
travel_guides/berlitz1/HandRLakeDistrict.txt:0
travel_guides/berlitz1/HandRLasVegas.txt:0
travel_guides/berlitz1/HandRLisbon.txt:0
travel_guides/berlitz1/HandRLosAngeles.txt:0
travel_guides/berlitz1/HandRMadeira.txt:0
travel_guides/berlitz1/HandRMadrid.txt:0
travel_guides/berlitz1/HandRMallorca.txt:0
travel_guides/berlitz1/HistoryDublin.txt:0
travel_guides/berlitz1/HistoryEdinburgh.txt:0
travel_guides/berlitz1/HistoryEgypt.txt:0
travel_guides/berlitz1/HistoryFWI.txt:0
travel_guides/berlitz1/HistoryFrance.txt:0
travel_guides/berlitz1/HistoryGreek.txt:0
travel_guides/berlitz1/HistoryHawaii.txt:0
travel_guides/berlitz1/HistoryHongKong.txt:0
travel_guides/berlitz1/HistoryIbiza.txt:0
travel_guides/berlitz1/HistoryIndia.txt:0
travel_guides/berlitz1/HistoryIsrael.txt:0
travel_guides/berlitz1/HistoryIstanbul.txt:0
travel_guides/berlitz1/HistoryItaly.txt:0
travel_guides/berlitz1/HistoryJamaica.txt:0
travel_guides/berlitz1/HistoryJapan.txt:0
travel_guides/berlitz1/HistoryJerusalem.txt:0
travel_guides/berlitz1/HistoryLakeDistrict.txt:0
travel_guides/berlitz1/HistoryLasVegas.txt:0
travel_guides/berlitz1/HistoryMadeira.txt:0
travel_guides/berlitz1/HistoryMadrid.txt:0
travel_guides/berlitz1/HistoryMalaysia.txt:0
travel_guides/berlitz1/HistoryMallorca.txt:0
travel_guides/berlitz1/IntroDublin.txt:0
travel_guides/berlitz1/IntroEdinburgh.txt:0
travel_guides/berlitz1/IntroEgypt.txt:0
travel_guides/berlitz1/IntroFWI.txt:0
travel_guides/berlitz1/IntroFrance.txt:0
travel_guides/berlitz1/IntroGreek.txt:0
travel_guides/berlitz1/IntroHongKong.txt:0
travel_guides/berlitz1/IntroIbiza.txt:0
travel_guides/berlitz1/IntroIndia.txt:0
travel_guides/berlitz1/IntroIsrael.txt:0
travel_guides/berlitz1/IntroIstanbul.txt:0
travel_guides/berlitz1/IntroItaly.txt:0
travel_guides/berlitz1/IntroJamaica.txt:0
travel_guides/berlitz1/IntroJapan.txt:0
travel_guides/berlitz1/IntroJerusalem.txt:0
travel_guides/berlitz1/IntroLakeDistrict.txt:0
travel_guides/berlitz1/IntroLasVegas.txt:0
travel_guides/berlitz1/IntroLosAngeles.txt:0
travel_guides/berlitz1/IntroMadeira.txt:0
travel_guides/berlitz1/IntroMadrid.txt:0
travel_guides/berlitz1/IntroMalaysia.txt:0
travel_guides/berlitz1/IntroMallorca.txt:0
travel_guides/berlitz1/JungleMalaysia.txt:0
travel_guides/berlitz1/WhatToDublin.txt:0
travel_guides/berlitz1/WhatToEdinburgh.txt:0
travel_guides/berlitz1/WhatToEgypt.txt:0
travel_guides/berlitz1/WhatToFWI.txt:0
travel_guides/berlitz1/WhatToFrance.txt:0
travel_guides/berlitz1/WhatToGreek.txt:0
travel_guides/berlitz1/WhatToHawaii.txt:0
travel_guides/berlitz1/WhatToHongKong.txt:0
travel_guides/berlitz1/WhatToIbiza.txt:0
travel_guides/berlitz1/WhatToIndia.txt:0
travel_guides/berlitz1/WhatToIsrael.txt:0
travel_guides/berlitz1/WhatToIstanbul.txt:0
travel_guides/berlitz1/WhatToItaly.txt:0
travel_guides/berlitz1/WhatToJamaica.txt:0
travel_guides/berlitz1/WhatToJapan.txt:0
travel_guides/berlitz1/WhatToLakeDistrict.txt:0
travel_guides/berlitz1/WhatToLasVegas.txt:0
travel_guides/berlitz1/WhatToLosAngeles.txt:0
travel_guides/berlitz1/WhatToMadeira.txt:0
travel_guides/berlitz1/WhatToMalaysia.txt:0
travel_guides/berlitz1/WhatToMallorca.txt:0
travel_guides/berlitz1/WhereToDublin.txt:0
travel_guides/berlitz1/WhereToEdinburgh.txt:0
travel_guides/berlitz1/WhereToEgypt.txt:0
travel_guides/berlitz1/WhereToFWI.txt:0
travel_guides/berlitz1/WhereToFrance.txt:0
travel_guides/berlitz1/WhereToGreek.txt:0
travel_guides/berlitz1/WhereToHawaii.txt:0
travel_guides/berlitz1/WhereToHongKong.txt:0
travel_guides/berlitz1/WhereToIbiza.txt:0
travel_guides/berlitz1/WhereToIndia.txt:0
travel_guides/berlitz1/WhereToIsrael.txt:0
travel_guides/berlitz1/WhereToIstanbul.txt:0
travel_guides/berlitz1/WhereToItaly.txt:0
travel_guides/berlitz1/WhereToJapan.txt:0
travel_guides/berlitz1/WhereToJerusalem.txt:0
travel_guides/berlitz1/WhereToLakeDistrict.txt:0
travel_guides/berlitz1/WhereToLosAngeles.txt:0
travel_guides/berlitz1/WhereToMadeira.txt:0
travel_guides/berlitz1/WhereToMadrid.txt:0
travel_guides/berlitz1/WhereToMalaysia.txt:0
travel_guides/berlitz1/WhereToMallorca.txt:0
travel_guides/berlitz2/Algarve-History.txt:0
travel_guides/berlitz2/Algarve-Intro.txt:0
travel_guides/berlitz2/Algarve-WhatToDo.txt:0
travel_guides/berlitz2/Algarve-WhereToGo.txt:0
travel_guides/berlitz2/Amsterdam-History.txt:0
travel_guides/berlitz2/Amsterdam-Intro.txt:0
travel_guides/berlitz2/Amsterdam-WhatToDo.txt:0
travel_guides/berlitz2/Amsterdam-WhereToGo.txt:0
travel_guides/berlitz2/Athens-History.txt:0
travel_guides/berlitz2/Athens-Intro.txt:0
travel_guides/berlitz2/Athens-WhatToDo.txt:0
travel_guides/berlitz2/Athens-WhereToGo.txt:0
travel_guides/berlitz2/Bahamas-History.txt:2
travel_guides/berlitz2/Bahamas-Intro.txt:0
travel_guides/berlitz2/Bahamas-WhatToDo.txt:0
travel_guides/berlitz2/Bahamas-WhereToGo.txt:0
travel_guides/berlitz2/Bali-History.txt:0
travel_guides/berlitz2/Bali-WhatToDo.txt:0
travel_guides/berlitz2/Bali-WhereToGo.txt:0
travel_guides/berlitz2/Barcelona-History.txt:0
travel_guides/berlitz2/Barcelona-WhatToDo.txt:0
travel_guides/berlitz2/Barcelona-WhereToGo.txt:0
travel_guides/berlitz2/Beijing-History.txt:0
travel_guides/berlitz2/Beijing-WhatToDo.txt:0
travel_guides/berlitz2/Beijing-WhereToGo.txt:0
travel_guides/berlitz2/Berlin-History.txt:0
travel_guides/berlitz2/Berlin-WhatToDo.txt:0
travel_guides/berlitz2/Berlin-WhereToGo.txt:0
travel_guides/berlitz2/Bermuda-WhatToDo.txt:0
travel_guides/berlitz2/Bermuda-WhereToGo.txt:0
travel_guides/berlitz2/Bermuda-history.txt:0
travel_guides/berlitz2/Boston-WhereToGo.txt:0
travel_guides/berlitz2/Budapest-History.txt:0
travel_guides/berlitz2/Budapest-WhatToDo.txt:0
travel_guides/berlitz2/Budapest-WhereoGo.txt:0
travel_guides/berlitz2/California-History.txt:0
travel_guides/berlitz2/California-WhatToDo.txt:0
travel_guides/berlitz2/California-WhereToGo.txt:0
travel_guides/berlitz2/Canada-History.txt:0
travel_guides/berlitz2/Canada-WhereToGo.txt:0
travel_guides/berlitz2/CanaryIslands-History.txt:0
travel_guides/berlitz2/CanaryIslands-WhatToDo.txt:0
travel_guides/berlitz2/CanaryIslands-WhereToGo.txt:0
travel_guides/berlitz2/Cancun-History.txt:0
travel_guides/berlitz2/Cancun-WhatToDo.txt:0
travel_guides/berlitz2/Cancun-WhereToGo.txt:0
travel_guides/berlitz2/China-History.txt:0
travel_guides/berlitz2/China-WhatToDo.txt:0
travel_guides/berlitz2/China-WhereToGo.txt:0
travel_guides/berlitz2/Costa-History.txt:0
travel_guides/berlitz2/Costa-WhatToDo.txt:0
travel_guides/berlitz2/Costa-WhereToGo.txt:0
travel_guides/berlitz2/CostaBlanca-History.txt:0
travel_guides/berlitz2/CostaBlanca-WhatToDo.txt:0
travel_guides/berlitz2/Crete-History.txt:0
travel_guides/berlitz2/Crete-WhatToDo.txt:0
travel_guides/berlitz2/Crete-WhereToGo.txt:0
travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:0
travel_guides/berlitz2/Cuba-History.txt:0
travel_guides/berlitz2/Cuba-WhatToDo.txt:0
travel_guides/berlitz2/Cuba-WhereToGo.txt:0
travel_guides/berlitz2/Nepal-History.txt:0
travel_guides/berlitz2/Nepal-WhatToDo.txt:0
travel_guides/berlitz2/Nepal-WhereToGo.txt:0
travel_guides/berlitz2/NewOrleans-History.txt:0
travel_guides/berlitz2/Paris-WhatToDo.txt:0
travel_guides/berlitz2/Paris-WhereToGo.txt:0
travel_guides/berlitz2/Poland-History.txt:0
travel_guides/berlitz2/Poland-WhatToDo.txt:0
travel_guides/berlitz2/Portugal-History.txt:0
travel_guides/berlitz2/Portugal-WhatToDo.txt:0
travel_guides/berlitz2/Portugal-WhereToGo.txt:0
travel_guides/berlitz2/PuertoRico-History.txt:0
travel_guides/berlitz2/PuertoRico-WhatToDo.txt:0
travel_guides/berlitz2/PuertoRico-WhereToGo.txt:0
travel_guides/berlitz2/Vallarta-History.txt:0
travel_guides/berlitz2/Vallarta-WhatToDo.txt:0
travel_guides/berlitz2/Vallarta-WhereToGo.txt:0
```

**Example B**

> Combined with `-r` to search all subdirectories:

*Input*

```shell
$ grep -r -c "Test"
```

*Output*

```shell
$ grep -r -c "Test"
non-fiction/OUP/Abernathy/ch1.txt:0
non-fiction/OUP/Abernathy/ch14.txt:0
non-fiction/OUP/Abernathy/ch15.txt:0
non-fiction/OUP/Abernathy/ch2.txt:0
non-fiction/OUP/Abernathy/ch3.txt:0
non-fiction/OUP/Abernathy/ch6.txt:0
non-fiction/OUP/Abernathy/ch7.txt:0
non-fiction/OUP/Abernathy/ch8.txt:0
non-fiction/OUP/Abernathy/ch9.txt:0
non-fiction/OUP/Berk/CH4.txt:0
non-fiction/OUP/Berk/ch1.txt:1
non-fiction/OUP/Berk/ch2.txt:0
non-fiction/OUP/Berk/ch7.txt:0
non-fiction/OUP/Castro/chA.txt:0
non-fiction/OUP/Castro/chB.txt:0
non-fiction/OUP/Castro/chC.txt:0
non-fiction/OUP/Castro/chL.txt:0
non-fiction/OUP/Castro/chM.txt:0
non-fiction/OUP/Castro/chN.txt:0
non-fiction/OUP/Castro/chO.txt:0
non-fiction/OUP/Castro/chP.txt:0
non-fiction/OUP/Castro/chQ.txt:0
non-fiction/OUP/Castro/chR.txt:0
non-fiction/OUP/Castro/chV.txt:0
non-fiction/OUP/Castro/chW.txt:0
non-fiction/OUP/Castro/chY.txt:0
non-fiction/OUP/Castro/chZ.txt:0
non-fiction/OUP/Fletcher/ch1.txt:1
non-fiction/OUP/Fletcher/ch10.txt:0
non-fiction/OUP/Fletcher/ch2.txt:0
non-fiction/OUP/Fletcher/ch5.txt:0
non-fiction/OUP/Fletcher/ch6.txt:0
non-fiction/OUP/Fletcher/ch9.txt:0
non-fiction/OUP/Kauffman/ch1.txt:0
non-fiction/OUP/Kauffman/ch10.txt:1
non-fiction/OUP/Kauffman/ch3.txt:0
non-fiction/OUP/Kauffman/ch4.txt:0
non-fiction/OUP/Kauffman/ch5.txt:0
non-fiction/OUP/Kauffman/ch6.txt:0
non-fiction/OUP/Kauffman/ch7.txt:0
non-fiction/OUP/Kauffman/ch8.txt:0
non-fiction/OUP/Kauffman/ch9.txt:0
non-fiction/OUP/Rybczynski/ch1.txt:0
non-fiction/OUP/Rybczynski/ch2.txt:0
non-fiction/OUP/Rybczynski/ch3.txt:0
travel_guides/berlitz1/HandRHawaii.txt:0
travel_guides/berlitz1/HandRHongKong.txt:0
travel_guides/berlitz1/HandRIbiza.txt:0
travel_guides/berlitz1/HandRIsrael.txt:0
travel_guides/berlitz1/HandRIstanbul.txt:0
travel_guides/berlitz1/HandRJamaica.txt:0
travel_guides/berlitz1/HandRJerusalem.txt:0
travel_guides/berlitz1/HandRLakeDistrict.txt:0
travel_guides/berlitz1/HandRLasVegas.txt:0
travel_guides/berlitz1/HandRLisbon.txt:0
travel_guides/berlitz1/HandRLosAngeles.txt:0
travel_guides/berlitz1/HandRMadeira.txt:0
travel_guides/berlitz1/HandRMadrid.txt:0
travel_guides/berlitz1/HandRMallorca.txt:0
travel_guides/berlitz1/HistoryDublin.txt:0
travel_guides/berlitz1/HistoryEdinburgh.txt:0
travel_guides/berlitz1/HistoryEgypt.txt:0
travel_guides/berlitz1/HistoryFWI.txt:0
travel_guides/berlitz1/HistoryFrance.txt:0
travel_guides/berlitz1/HistoryGreek.txt:1
travel_guides/berlitz1/HistoryHawaii.txt:0
travel_guides/berlitz1/HistoryHongKong.txt:0
travel_guides/berlitz1/HistoryIbiza.txt:0
travel_guides/berlitz1/HistoryIndia.txt:0
travel_guides/berlitz1/HistoryIsrael.txt:0
travel_guides/berlitz1/HistoryIstanbul.txt:0
travel_guides/berlitz1/HistoryItaly.txt:0
travel_guides/berlitz1/HistoryJamaica.txt:0
travel_guides/berlitz1/HistoryJapan.txt:0
travel_guides/berlitz1/HistoryJerusalem.txt:0
travel_guides/berlitz1/HistoryLakeDistrict.txt:0
travel_guides/berlitz1/HistoryLasVegas.txt:1
travel_guides/berlitz1/HistoryMadeira.txt:0
travel_guides/berlitz1/HistoryMadrid.txt:0
travel_guides/berlitz1/HistoryMalaysia.txt:0
travel_guides/berlitz1/HistoryMallorca.txt:0
travel_guides/berlitz1/IntroDublin.txt:0
travel_guides/berlitz1/IntroEdinburgh.txt:0
travel_guides/berlitz1/IntroEgypt.txt:0
travel_guides/berlitz1/IntroFWI.txt:0
travel_guides/berlitz1/IntroFrance.txt:0
travel_guides/berlitz1/IntroGreek.txt:0
travel_guides/berlitz1/IntroHongKong.txt:0
travel_guides/berlitz1/IntroIbiza.txt:0
travel_guides/berlitz1/IntroIndia.txt:0
travel_guides/berlitz1/IntroIsrael.txt:0
travel_guides/berlitz1/IntroIstanbul.txt:0
travel_guides/berlitz1/IntroItaly.txt:0
travel_guides/berlitz1/IntroJamaica.txt:0
travel_guides/berlitz1/IntroJapan.txt:0
travel_guides/berlitz1/IntroJerusalem.txt:0
travel_guides/berlitz1/IntroLakeDistrict.txt:0
travel_guides/berlitz1/IntroLasVegas.txt:0
travel_guides/berlitz1/IntroLosAngeles.txt:0
travel_guides/berlitz1/IntroMadeira.txt:0
travel_guides/berlitz1/IntroMadrid.txt:0
travel_guides/berlitz1/IntroMalaysia.txt:0
travel_guides/berlitz1/IntroMallorca.txt:0
travel_guides/berlitz1/JungleMalaysia.txt:0
travel_guides/berlitz1/WhatToDublin.txt:0
travel_guides/berlitz1/WhatToEdinburgh.txt:0
travel_guides/berlitz1/WhatToEgypt.txt:0
travel_guides/berlitz1/WhatToFWI.txt:0
travel_guides/berlitz1/WhatToFrance.txt:0
travel_guides/berlitz1/WhatToGreek.txt:0
travel_guides/berlitz1/WhatToHawaii.txt:0
travel_guides/berlitz1/WhatToHongKong.txt:0
travel_guides/berlitz1/WhatToIbiza.txt:0
travel_guides/berlitz1/WhatToIndia.txt:0
travel_guides/berlitz1/WhatToIsrael.txt:0
travel_guides/berlitz1/WhatToIstanbul.txt:0
travel_guides/berlitz1/WhatToItaly.txt:0
travel_guides/berlitz1/WhatToJamaica.txt:0
travel_guides/berlitz1/WhatToJapan.txt:0
travel_guides/berlitz1/WhatToLakeDistrict.txt:0
travel_guides/berlitz1/WhatToLasVegas.txt:0
travel_guides/berlitz1/WhatToLosAngeles.txt:0
travel_guides/berlitz1/WhatToMadeira.txt:0
travel_guides/berlitz1/WhatToMalaysia.txt:0
travel_guides/berlitz1/WhatToMallorca.txt:0
travel_guides/berlitz1/WhereToDublin.txt:0
travel_guides/berlitz1/WhereToEdinburgh.txt:0
travel_guides/berlitz1/WhereToEgypt.txt:0
travel_guides/berlitz1/WhereToFWI.txt:0
travel_guides/berlitz1/WhereToFrance.txt:3
travel_guides/berlitz1/WhereToGreek.txt:1
travel_guides/berlitz1/WhereToHawaii.txt:0
travel_guides/berlitz1/WhereToHongKong.txt:0
travel_guides/berlitz1/WhereToIbiza.txt:0
travel_guides/berlitz1/WhereToIndia.txt:0
travel_guides/berlitz1/WhereToIsrael.txt:0
travel_guides/berlitz1/WhereToIstanbul.txt:0
travel_guides/berlitz1/WhereToItaly.txt:9
travel_guides/berlitz1/WhereToJapan.txt:0
travel_guides/berlitz1/WhereToJerusalem.txt:3
travel_guides/berlitz1/WhereToLakeDistrict.txt:0
travel_guides/berlitz1/WhereToLosAngeles.txt:0
travel_guides/berlitz1/WhereToMadeira.txt:0
travel_guides/berlitz1/WhereToMadrid.txt:1
travel_guides/berlitz1/WhereToMalaysia.txt:0
travel_guides/berlitz1/WhereToMallorca.txt:0
travel_guides/berlitz2/Algarve-History.txt:0
travel_guides/berlitz2/Algarve-Intro.txt:0
travel_guides/berlitz2/Algarve-WhatToDo.txt:0
travel_guides/berlitz2/Algarve-WhereToGo.txt:0
travel_guides/berlitz2/Amsterdam-History.txt:0
travel_guides/berlitz2/Amsterdam-Intro.txt:0
travel_guides/berlitz2/Amsterdam-WhatToDo.txt:0
travel_guides/berlitz2/Amsterdam-WhereToGo.txt:1
travel_guides/berlitz2/Athens-History.txt:0
travel_guides/berlitz2/Athens-Intro.txt:0
travel_guides/berlitz2/Athens-WhatToDo.txt:0
travel_guides/berlitz2/Athens-WhereToGo.txt:0
travel_guides/berlitz2/Bahamas-History.txt:0
travel_guides/berlitz2/Bahamas-Intro.txt:0
travel_guides/berlitz2/Bahamas-WhatToDo.txt:0
travel_guides/berlitz2/Bahamas-WhereToGo.txt:0
travel_guides/berlitz2/Bali-History.txt:0
travel_guides/berlitz2/Bali-WhatToDo.txt:0
travel_guides/berlitz2/Bali-WhereToGo.txt:0
travel_guides/berlitz2/Barcelona-History.txt:0
travel_guides/berlitz2/Barcelona-WhatToDo.txt:0
travel_guides/berlitz2/Barcelona-WhereToGo.txt:0
travel_guides/berlitz2/Beijing-History.txt:0
travel_guides/berlitz2/Beijing-WhatToDo.txt:0
travel_guides/berlitz2/Beijing-WhereToGo.txt:0
travel_guides/berlitz2/Berlin-History.txt:0
travel_guides/berlitz2/Berlin-WhatToDo.txt:0
travel_guides/berlitz2/Berlin-WhereToGo.txt:0
travel_guides/berlitz2/Bermuda-WhatToDo.txt:0
travel_guides/berlitz2/Bermuda-WhereToGo.txt:0
travel_guides/berlitz2/Bermuda-history.txt:0
travel_guides/berlitz2/Boston-WhereToGo.txt:1
travel_guides/berlitz2/Budapest-History.txt:0
travel_guides/berlitz2/Budapest-WhatToDo.txt:0
travel_guides/berlitz2/Budapest-WhereoGo.txt:0
travel_guides/berlitz2/California-History.txt:0
travel_guides/berlitz2/California-WhatToDo.txt:0
travel_guides/berlitz2/California-WhereToGo.txt:0
travel_guides/berlitz2/Canada-History.txt:0
travel_guides/berlitz2/Canada-WhereToGo.txt:2
travel_guides/berlitz2/CanaryIslands-History.txt:0
travel_guides/berlitz2/CanaryIslands-WhatToDo.txt:0
travel_guides/berlitz2/CanaryIslands-WhereToGo.txt:0
travel_guides/berlitz2/Cancun-History.txt:0
travel_guides/berlitz2/Cancun-WhatToDo.txt:0
travel_guides/berlitz2/Cancun-WhereToGo.txt:0
travel_guides/berlitz2/China-History.txt:0
travel_guides/berlitz2/China-WhatToDo.txt:0
travel_guides/berlitz2/China-WhereToGo.txt:1
travel_guides/berlitz2/Costa-History.txt:0
travel_guides/berlitz2/Costa-WhatToDo.txt:0
travel_guides/berlitz2/Costa-WhereToGo.txt:0
travel_guides/berlitz2/CostaBlanca-History.txt:0
travel_guides/berlitz2/CostaBlanca-WhatToDo.txt:0
travel_guides/berlitz2/Crete-History.txt:0
travel_guides/berlitz2/Crete-WhatToDo.txt:0
travel_guides/berlitz2/Crete-WhereToGo.txt:0
travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:0
travel_guides/berlitz2/Cuba-History.txt:0
travel_guides/berlitz2/Cuba-WhatToDo.txt:0
travel_guides/berlitz2/Cuba-WhereToGo.txt:0
travel_guides/berlitz2/Nepal-History.txt:0
travel_guides/berlitz2/Nepal-WhatToDo.txt:0
travel_guides/berlitz2/Nepal-WhereToGo.txt:0
travel_guides/berlitz2/NewOrleans-History.txt:0
travel_guides/berlitz2/Paris-WhatToDo.txt:0
travel_guides/berlitz2/Paris-WhereToGo.txt:0
travel_guides/berlitz2/Poland-History.txt:0
travel_guides/berlitz2/Poland-WhatToDo.txt:0
travel_guides/berlitz2/Portugal-History.txt:0
travel_guides/berlitz2/Portugal-WhatToDo.txt:0
travel_guides/berlitz2/Portugal-WhereToGo.txt:0
travel_guides/berlitz2/PuertoRico-History.txt:0
travel_guides/berlitz2/PuertoRico-WhatToDo.txt:0
travel_guides/berlitz2/PuertoRico-WhereToGo.txt:0
travel_guides/berlitz2/Vallarta-History.txt:0
travel_guides/berlitz2/Vallarta-WhatToDo.txt:0
travel_guides/berlitz2/Vallarta-WhereToGo.txt:0
```


### 3rd Option: `-l`, `--files-with-matches`

> This option will "Suppress normal output; instead print the name of each input file from which output would normally have been printed."

>This is useful because you can see just the names of the files containing the matching string pattern and don't have to scroll through the printed file outputs.

**Example A**

*Input*

> Combined with `-r` to search all subdirectories:

```shell
$ grep -r -l "Lucayans"
```

*Output*

```shell
$ grep -r -l "Lucayans"
travel_guides/berlitz2/Bahamas-History.txt
```

**Example B**

> Combined with `-r` to search all subdirectories:

*Input*

```shell
$ grep -r -l "Test"
```

*Output*

```shell
$ grep -r -l "Test"
non-fiction/OUP/Berk/ch1.txt
non-fiction/OUP/Fletcher/ch1.txt
non-fiction/OUP/Kauffman/ch10.txt
travel_guides/berlitz1/HistoryGreek.txt
travel_guides/berlitz1/HistoryLasVegas.txt
travel_guides/berlitz1/WhereToFrance.txt
travel_guides/berlitz1/WhereToGreek.txt
travel_guides/berlitz1/WhereToItaly.txt
travel_guides/berlitz1/WhereToJerusalem.txt
travel_guides/berlitz1/WhereToMadrid.txt
travel_guides/berlitz2/Amsterdam-WhereToGo.txt
travel_guides/berlitz2/Boston-WhereToGo.txt
travel_guides/berlitz2/Canada-WhereToGo.txt
travel_guides/berlitz2/China-WhereToGo.txt
```


### 4th Option: `-L`, `--files-without-match`

> This option will "suppress normal output; instead print the name of each input file from which no output would normally have been printed."

> This is useful because you can see the names of the files that don't conatin the matching string pattern.

**Example A**

> Combined with `-r` to search all subdirectories:

*Input*

```shell
$ grep -r -L "Lucayans"
```

*Output*

```shell
$ grep -r -L "Lucayans"
non-fiction/OUP/Abernathy/ch1.txt
non-fiction/OUP/Abernathy/ch14.txt
non-fiction/OUP/Abernathy/ch15.txt
non-fiction/OUP/Abernathy/ch2.txt
non-fiction/OUP/Abernathy/ch3.txt
non-fiction/OUP/Abernathy/ch6.txt
non-fiction/OUP/Abernathy/ch7.txt
non-fiction/OUP/Abernathy/ch8.txt
non-fiction/OUP/Abernathy/ch9.txt
non-fiction/OUP/Berk/CH4.txt
non-fiction/OUP/Berk/ch1.txt
non-fiction/OUP/Berk/ch2.txt
non-fiction/OUP/Berk/ch7.txt
non-fiction/OUP/Castro/chA.txt
non-fiction/OUP/Castro/chB.txt
non-fiction/OUP/Castro/chC.txt
non-fiction/OUP/Castro/chL.txt
non-fiction/OUP/Castro/chM.txt
non-fiction/OUP/Castro/chN.txt
non-fiction/OUP/Castro/chO.txt
non-fiction/OUP/Castro/chP.txt
non-fiction/OUP/Castro/chQ.txt
non-fiction/OUP/Castro/chR.txt
non-fiction/OUP/Castro/chV.txt
non-fiction/OUP/Castro/chW.txt
non-fiction/OUP/Castro/chY.txt
non-fiction/OUP/Castro/chZ.txt
non-fiction/OUP/Fletcher/ch1.txt
non-fiction/OUP/Fletcher/ch10.txt
non-fiction/OUP/Fletcher/ch2.txt
non-fiction/OUP/Fletcher/ch5.txt
non-fiction/OUP/Fletcher/ch6.txt
non-fiction/OUP/Fletcher/ch9.txt
non-fiction/OUP/Kauffman/ch1.txt
non-fiction/OUP/Kauffman/ch10.txt
non-fiction/OUP/Kauffman/ch3.txt
non-fiction/OUP/Kauffman/ch4.txt
non-fiction/OUP/Kauffman/ch5.txt
non-fiction/OUP/Kauffman/ch6.txt
non-fiction/OUP/Kauffman/ch7.txt
non-fiction/OUP/Kauffman/ch8.txt
non-fiction/OUP/Kauffman/ch9.txt
non-fiction/OUP/Rybczynski/ch1.txt
non-fiction/OUP/Rybczynski/ch2.txt
non-fiction/OUP/Rybczynski/ch3.txt
travel_guides/berlitz1/HandRHawaii.txt
travel_guides/berlitz1/HandRHongKong.txt
travel_guides/berlitz1/HandRIbiza.txt
travel_guides/berlitz1/HandRIsrael.txt
travel_guides/berlitz1/HandRIstanbul.txt
travel_guides/berlitz1/HandRJamaica.txt
travel_guides/berlitz1/HandRJerusalem.txt
travel_guides/berlitz1/HandRLakeDistrict.txt
travel_guides/berlitz1/HandRLasVegas.txt
travel_guides/berlitz1/HandRLisbon.txt
travel_guides/berlitz1/HandRLosAngeles.txt
travel_guides/berlitz1/HandRMadeira.txt
travel_guides/berlitz1/HandRMadrid.txt
travel_guides/berlitz1/HandRMallorca.txt
travel_guides/berlitz1/HistoryDublin.txt
travel_guides/berlitz1/HistoryEdinburgh.txt
travel_guides/berlitz1/HistoryEgypt.txt
travel_guides/berlitz1/HistoryFWI.txt
travel_guides/berlitz1/HistoryFrance.txt
travel_guides/berlitz1/HistoryGreek.txt
travel_guides/berlitz1/HistoryHawaii.txt
travel_guides/berlitz1/HistoryHongKong.txt
travel_guides/berlitz1/HistoryIbiza.txt
travel_guides/berlitz1/HistoryIndia.txt
travel_guides/berlitz1/HistoryIsrael.txt
travel_guides/berlitz1/HistoryIstanbul.txt
travel_guides/berlitz1/HistoryItaly.txt
travel_guides/berlitz1/HistoryJamaica.txt
travel_guides/berlitz1/HistoryJapan.txt
travel_guides/berlitz1/HistoryJerusalem.txt
travel_guides/berlitz1/HistoryLakeDistrict.txt
travel_guides/berlitz1/HistoryLasVegas.txt
travel_guides/berlitz1/HistoryMadeira.txt
travel_guides/berlitz1/HistoryMadrid.txt
travel_guides/berlitz1/HistoryMalaysia.txt
travel_guides/berlitz1/HistoryMallorca.txt
travel_guides/berlitz1/IntroDublin.txt
travel_guides/berlitz1/IntroEdinburgh.txt
travel_guides/berlitz1/IntroEgypt.txt
travel_guides/berlitz1/IntroFWI.txt
travel_guides/berlitz1/IntroFrance.txt
travel_guides/berlitz1/IntroGreek.txt
travel_guides/berlitz1/IntroHongKong.txt
travel_guides/berlitz1/IntroIbiza.txt
travel_guides/berlitz1/IntroIndia.txt
travel_guides/berlitz1/IntroIsrael.txt
travel_guides/berlitz1/IntroIstanbul.txt
travel_guides/berlitz1/IntroItaly.txt
travel_guides/berlitz1/IntroJamaica.txt
travel_guides/berlitz1/IntroJapan.txt
travel_guides/berlitz1/IntroJerusalem.txt
travel_guides/berlitz1/IntroLakeDistrict.txt
travel_guides/berlitz1/IntroLasVegas.txt
travel_guides/berlitz1/IntroLosAngeles.txt
travel_guides/berlitz1/IntroMadeira.txt
travel_guides/berlitz1/IntroMadrid.txt
travel_guides/berlitz1/IntroMalaysia.txt
travel_guides/berlitz1/IntroMallorca.txt
travel_guides/berlitz1/JungleMalaysia.txt
travel_guides/berlitz1/WhatToDublin.txt
travel_guides/berlitz1/WhatToEdinburgh.txt
travel_guides/berlitz1/WhatToEgypt.txt
travel_guides/berlitz1/WhatToFWI.txt
travel_guides/berlitz1/WhatToFrance.txt
travel_guides/berlitz1/WhatToGreek.txt
travel_guides/berlitz1/WhatToHawaii.txt
travel_guides/berlitz1/WhatToHongKong.txt
travel_guides/berlitz1/WhatToIbiza.txt
travel_guides/berlitz1/WhatToIndia.txt
travel_guides/berlitz1/WhatToIsrael.txt
travel_guides/berlitz1/WhatToIstanbul.txt
travel_guides/berlitz1/WhatToItaly.txt
travel_guides/berlitz1/WhatToJamaica.txt
travel_guides/berlitz1/WhatToJapan.txt
travel_guides/berlitz1/WhatToLakeDistrict.txt
travel_guides/berlitz1/WhatToLasVegas.txt
travel_guides/berlitz1/WhatToLosAngeles.txt
travel_guides/berlitz1/WhatToMadeira.txt
travel_guides/berlitz1/WhatToMalaysia.txt
travel_guides/berlitz1/WhatToMallorca.txt
travel_guides/berlitz1/WhereToDublin.txt
travel_guides/berlitz1/WhereToEdinburgh.txt
travel_guides/berlitz1/WhereToEgypt.txt
travel_guides/berlitz1/WhereToFWI.txt
travel_guides/berlitz1/WhereToFrance.txt
travel_guides/berlitz1/WhereToGreek.txt
travel_guides/berlitz1/WhereToHawaii.txt
travel_guides/berlitz1/WhereToHongKong.txt
travel_guides/berlitz1/WhereToIbiza.txt
travel_guides/berlitz1/WhereToIndia.txt
travel_guides/berlitz1/WhereToIsrael.txt
travel_guides/berlitz1/WhereToIstanbul.txt
travel_guides/berlitz1/WhereToItaly.txt
travel_guides/berlitz1/WhereToJapan.txt
travel_guides/berlitz1/WhereToJerusalem.txt
travel_guides/berlitz1/WhereToLakeDistrict.txt
travel_guides/berlitz1/WhereToLosAngeles.txt
travel_guides/berlitz1/WhereToMadeira.txt
travel_guides/berlitz1/WhereToMadrid.txt
travel_guides/berlitz1/WhereToMalaysia.txt
travel_guides/berlitz1/WhereToMallorca.txt
travel_guides/berlitz2/Algarve-History.txt
travel_guides/berlitz2/Algarve-Intro.txt
travel_guides/berlitz2/Algarve-WhatToDo.txt
travel_guides/berlitz2/Algarve-WhereToGo.txt
travel_guides/berlitz2/Amsterdam-History.txt
travel_guides/berlitz2/Amsterdam-Intro.txt
travel_guides/berlitz2/Amsterdam-WhatToDo.txt
travel_guides/berlitz2/Amsterdam-WhereToGo.txt
travel_guides/berlitz2/Athens-History.txt
travel_guides/berlitz2/Athens-Intro.txt
travel_guides/berlitz2/Athens-WhatToDo.txt
travel_guides/berlitz2/Athens-WhereToGo.txt
travel_guides/berlitz2/Bahamas-Intro.txt
travel_guides/berlitz2/Bahamas-WhatToDo.txt
travel_guides/berlitz2/Bahamas-WhereToGo.txt
travel_guides/berlitz2/Bali-History.txt
travel_guides/berlitz2/Bali-WhatToDo.txt
travel_guides/berlitz2/Bali-WhereToGo.txt
travel_guides/berlitz2/Barcelona-History.txt
travel_guides/berlitz2/Barcelona-WhatToDo.txt
travel_guides/berlitz2/Barcelona-WhereToGo.txt
travel_guides/berlitz2/Beijing-History.txt
travel_guides/berlitz2/Beijing-WhatToDo.txt
travel_guides/berlitz2/Beijing-WhereToGo.txt
travel_guides/berlitz2/Berlin-History.txt
travel_guides/berlitz2/Berlin-WhatToDo.txt
travel_guides/berlitz2/Berlin-WhereToGo.txt
travel_guides/berlitz2/Bermuda-WhatToDo.txt
travel_guides/berlitz2/Bermuda-WhereToGo.txt
travel_guides/berlitz2/Bermuda-history.txt
travel_guides/berlitz2/Boston-WhereToGo.txt
travel_guides/berlitz2/Budapest-History.txt
travel_guides/berlitz2/Budapest-WhatToDo.txt
travel_guides/berlitz2/Budapest-WhereoGo.txt
travel_guides/berlitz2/California-History.txt
travel_guides/berlitz2/California-WhatToDo.txt
travel_guides/berlitz2/California-WhereToGo.txt
travel_guides/berlitz2/Canada-History.txt
travel_guides/berlitz2/Canada-WhereToGo.txt
travel_guides/berlitz2/CanaryIslands-History.txt
travel_guides/berlitz2/CanaryIslands-WhatToDo.txt
travel_guides/berlitz2/CanaryIslands-WhereToGo.txt
travel_guides/berlitz2/Cancun-History.txt
travel_guides/berlitz2/Cancun-WhatToDo.txt
travel_guides/berlitz2/Cancun-WhereToGo.txt
travel_guides/berlitz2/China-History.txt
travel_guides/berlitz2/China-WhatToDo.txt
travel_guides/berlitz2/China-WhereToGo.txt
travel_guides/berlitz2/Costa-History.txt
travel_guides/berlitz2/Costa-WhatToDo.txt
travel_guides/berlitz2/Costa-WhereToGo.txt
travel_guides/berlitz2/CostaBlanca-History.txt
travel_guides/berlitz2/CostaBlanca-WhatToDo.txt
travel_guides/berlitz2/Crete-History.txt
travel_guides/berlitz2/Crete-WhatToDo.txt
travel_guides/berlitz2/Crete-WhereToGo.txt
travel_guides/berlitz2/CstaBlanca-WhereToGo.txt
travel_guides/berlitz2/Cuba-History.txt
travel_guides/berlitz2/Cuba-WhatToDo.txt
travel_guides/berlitz2/Cuba-WhereToGo.txt
travel_guides/berlitz2/Nepal-History.txt
travel_guides/berlitz2/Nepal-WhatToDo.txt
travel_guides/berlitz2/Nepal-WhereToGo.txt
travel_guides/berlitz2/NewOrleans-History.txt
travel_guides/berlitz2/Paris-WhatToDo.txt
travel_guides/berlitz2/Paris-WhereToGo.txt
travel_guides/berlitz2/Poland-History.txt
travel_guides/berlitz2/Poland-WhatToDo.txt
travel_guides/berlitz2/Portugal-History.txt
travel_guides/berlitz2/Portugal-WhatToDo.txt
travel_guides/berlitz2/Portugal-WhereToGo.txt
travel_guides/berlitz2/PuertoRico-History.txt
travel_guides/berlitz2/PuertoRico-WhatToDo.txt
travel_guides/berlitz2/PuertoRico-WhereToGo.txt
travel_guides/berlitz2/Vallarta-History.txt
travel_guides/berlitz2/Vallarta-WhatToDo.txt
travel_guides/berlitz2/Vallarta-WhereToGo.txt
```

**Example B**

> Combined with `-r` to search all subdirectories:

*Input*

```shell
$ grep -r -L "Test"
```

*Output*

```shell
$ grep -r -L "Test"
non-fiction/OUP/Abernathy/ch1.txt
non-fiction/OUP/Abernathy/ch14.txt
non-fiction/OUP/Abernathy/ch15.txt
non-fiction/OUP/Abernathy/ch2.txt
non-fiction/OUP/Abernathy/ch3.txt
non-fiction/OUP/Abernathy/ch6.txt
non-fiction/OUP/Abernathy/ch7.txt
non-fiction/OUP/Abernathy/ch8.txt
non-fiction/OUP/Abernathy/ch9.txt
non-fiction/OUP/Berk/CH4.txt
non-fiction/OUP/Berk/ch2.txt
non-fiction/OUP/Berk/ch7.txt
non-fiction/OUP/Castro/chA.txt
non-fiction/OUP/Castro/chB.txt
non-fiction/OUP/Castro/chC.txt
non-fiction/OUP/Castro/chL.txt
non-fiction/OUP/Castro/chM.txt
non-fiction/OUP/Castro/chN.txt
non-fiction/OUP/Castro/chO.txt
non-fiction/OUP/Castro/chP.txt
non-fiction/OUP/Castro/chQ.txt
non-fiction/OUP/Castro/chR.txt
non-fiction/OUP/Castro/chV.txt
non-fiction/OUP/Castro/chW.txt
non-fiction/OUP/Castro/chY.txt
non-fiction/OUP/Castro/chZ.txt
non-fiction/OUP/Fletcher/ch10.txt
non-fiction/OUP/Fletcher/ch2.txt
non-fiction/OUP/Fletcher/ch5.txt
non-fiction/OUP/Fletcher/ch6.txt
non-fiction/OUP/Fletcher/ch9.txt
non-fiction/OUP/Kauffman/ch1.txt
non-fiction/OUP/Kauffman/ch3.txt
non-fiction/OUP/Kauffman/ch4.txt
non-fiction/OUP/Kauffman/ch5.txt
non-fiction/OUP/Kauffman/ch6.txt
non-fiction/OUP/Kauffman/ch7.txt
non-fiction/OUP/Kauffman/ch8.txt
non-fiction/OUP/Kauffman/ch9.txt
non-fiction/OUP/Rybczynski/ch1.txt
non-fiction/OUP/Rybczynski/ch2.txt
non-fiction/OUP/Rybczynski/ch3.txt
travel_guides/berlitz1/HandRHawaii.txt
travel_guides/berlitz1/HandRHongKong.txt
travel_guides/berlitz1/HandRIbiza.txt
travel_guides/berlitz1/HandRIsrael.txt
travel_guides/berlitz1/HandRIstanbul.txt
travel_guides/berlitz1/HandRJamaica.txt
travel_guides/berlitz1/HandRJerusalem.txt
travel_guides/berlitz1/HandRLakeDistrict.txt
travel_guides/berlitz1/HandRLasVegas.txt
travel_guides/berlitz1/HandRLisbon.txt
travel_guides/berlitz1/HandRLosAngeles.txt
travel_guides/berlitz1/HandRMadeira.txt
travel_guides/berlitz1/HandRMadrid.txt
travel_guides/berlitz1/HandRMallorca.txt
travel_guides/berlitz1/HistoryDublin.txt
travel_guides/berlitz1/HistoryEdinburgh.txt
travel_guides/berlitz1/HistoryEgypt.txt
travel_guides/berlitz1/HistoryFWI.txt
travel_guides/berlitz1/HistoryFrance.txt
travel_guides/berlitz1/HistoryHawaii.txt
travel_guides/berlitz1/HistoryHongKong.txt
travel_guides/berlitz1/HistoryIbiza.txt
travel_guides/berlitz1/HistoryIndia.txt
travel_guides/berlitz1/HistoryIsrael.txt
travel_guides/berlitz1/HistoryIstanbul.txt
travel_guides/berlitz1/HistoryItaly.txt
travel_guides/berlitz1/HistoryJamaica.txt
travel_guides/berlitz1/HistoryJapan.txt
travel_guides/berlitz1/HistoryJerusalem.txt
travel_guides/berlitz1/HistoryLakeDistrict.txt
travel_guides/berlitz1/HistoryMadeira.txt
travel_guides/berlitz1/HistoryMadrid.txt
travel_guides/berlitz1/HistoryMalaysia.txt
travel_guides/berlitz1/HistoryMallorca.txt
travel_guides/berlitz1/IntroDublin.txt
travel_guides/berlitz1/IntroEdinburgh.txt
travel_guides/berlitz1/IntroEgypt.txt
travel_guides/berlitz1/IntroFWI.txt
travel_guides/berlitz1/IntroFrance.txt
travel_guides/berlitz1/IntroGreek.txt
travel_guides/berlitz1/IntroHongKong.txt
travel_guides/berlitz1/IntroIbiza.txt
travel_guides/berlitz1/IntroIndia.txt
travel_guides/berlitz1/IntroIsrael.txt
travel_guides/berlitz1/IntroIstanbul.txt
travel_guides/berlitz1/IntroItaly.txt
travel_guides/berlitz1/IntroJamaica.txt
travel_guides/berlitz1/IntroJapan.txt
travel_guides/berlitz1/IntroJerusalem.txt
travel_guides/berlitz1/IntroLakeDistrict.txt
travel_guides/berlitz1/IntroLasVegas.txt
travel_guides/berlitz1/IntroLosAngeles.txt
travel_guides/berlitz1/IntroMadeira.txt
travel_guides/berlitz1/IntroMadrid.txt
travel_guides/berlitz1/IntroMalaysia.txt
travel_guides/berlitz1/IntroMallorca.txt
travel_guides/berlitz1/JungleMalaysia.txt
travel_guides/berlitz1/WhatToDublin.txt
travel_guides/berlitz1/WhatToEdinburgh.txt
travel_guides/berlitz1/WhatToEgypt.txt
travel_guides/berlitz1/WhatToFWI.txt
travel_guides/berlitz1/WhatToFrance.txt
travel_guides/berlitz1/WhatToGreek.txt
travel_guides/berlitz1/WhatToHawaii.txt
travel_guides/berlitz1/WhatToHongKong.txt
travel_guides/berlitz1/WhatToIbiza.txt
travel_guides/berlitz1/WhatToIndia.txt
travel_guides/berlitz1/WhatToIsrael.txt
travel_guides/berlitz1/WhatToIstanbul.txt
travel_guides/berlitz1/WhatToItaly.txt
travel_guides/berlitz1/WhatToJamaica.txt
travel_guides/berlitz1/WhatToJapan.txt
travel_guides/berlitz1/WhatToLakeDistrict.txt
travel_guides/berlitz1/WhatToLasVegas.txt
travel_guides/berlitz1/WhatToLosAngeles.txt
travel_guides/berlitz1/WhatToMadeira.txt
travel_guides/berlitz1/WhatToMalaysia.txt
travel_guides/berlitz1/WhatToMallorca.txt
travel_guides/berlitz1/WhereToDublin.txt
travel_guides/berlitz1/WhereToEdinburgh.txt
travel_guides/berlitz1/WhereToEgypt.txt
travel_guides/berlitz1/WhereToFWI.txt
travel_guides/berlitz1/WhereToHawaii.txt
travel_guides/berlitz1/WhereToHongKong.txt
travel_guides/berlitz1/WhereToIbiza.txt
travel_guides/berlitz1/WhereToIndia.txt
travel_guides/berlitz1/WhereToIsrael.txt
travel_guides/berlitz1/WhereToIstanbul.txt
travel_guides/berlitz1/WhereToJapan.txt
travel_guides/berlitz1/WhereToLakeDistrict.txt
travel_guides/berlitz1/WhereToLosAngeles.txt
travel_guides/berlitz1/WhereToMadeira.txt
travel_guides/berlitz1/WhereToMalaysia.txt
travel_guides/berlitz1/WhereToMallorca.txt
travel_guides/berlitz2/Algarve-History.txt
travel_guides/berlitz2/Algarve-Intro.txt
travel_guides/berlitz2/Algarve-WhatToDo.txt
travel_guides/berlitz2/Algarve-WhereToGo.txt
travel_guides/berlitz2/Amsterdam-History.txt
travel_guides/berlitz2/Amsterdam-Intro.txt
travel_guides/berlitz2/Amsterdam-WhatToDo.txt
travel_guides/berlitz2/Athens-History.txt
travel_guides/berlitz2/Athens-Intro.txt
travel_guides/berlitz2/Athens-WhatToDo.txt
travel_guides/berlitz2/Athens-WhereToGo.txt
travel_guides/berlitz2/Bahamas-History.txt
travel_guides/berlitz2/Bahamas-Intro.txt
travel_guides/berlitz2/Bahamas-WhatToDo.txt
travel_guides/berlitz2/Bahamas-WhereToGo.txt
travel_guides/berlitz2/Bali-History.txt
travel_guides/berlitz2/Bali-WhatToDo.txt
travel_guides/berlitz2/Bali-WhereToGo.txt
travel_guides/berlitz2/Barcelona-History.txt
travel_guides/berlitz2/Barcelona-WhatToDo.txt
travel_guides/berlitz2/Barcelona-WhereToGo.txt
travel_guides/berlitz2/Beijing-History.txt
travel_guides/berlitz2/Beijing-WhatToDo.txt
travel_guides/berlitz2/Beijing-WhereToGo.txt
travel_guides/berlitz2/Berlin-History.txt
travel_guides/berlitz2/Berlin-WhatToDo.txt
travel_guides/berlitz2/Berlin-WhereToGo.txt
travel_guides/berlitz2/Bermuda-WhatToDo.txt
travel_guides/berlitz2/Bermuda-WhereToGo.txt
travel_guides/berlitz2/Bermuda-history.txt
travel_guides/berlitz2/Budapest-History.txt
travel_guides/berlitz2/Budapest-WhatToDo.txt
travel_guides/berlitz2/Budapest-WhereoGo.txt
travel_guides/berlitz2/California-History.txt
travel_guides/berlitz2/California-WhatToDo.txt
travel_guides/berlitz2/California-WhereToGo.txt
travel_guides/berlitz2/Canada-History.txt
travel_guides/berlitz2/CanaryIslands-History.txt
travel_guides/berlitz2/CanaryIslands-WhatToDo.txt
travel_guides/berlitz2/CanaryIslands-WhereToGo.txt
travel_guides/berlitz2/Cancun-History.txt
travel_guides/berlitz2/Cancun-WhatToDo.txt
travel_guides/berlitz2/Cancun-WhereToGo.txt
travel_guides/berlitz2/China-History.txt
travel_guides/berlitz2/China-WhatToDo.txt
travel_guides/berlitz2/Costa-History.txt
travel_guides/berlitz2/Costa-WhatToDo.txt
travel_guides/berlitz2/Costa-WhereToGo.txt
travel_guides/berlitz2/CostaBlanca-History.txt
travel_guides/berlitz2/CostaBlanca-WhatToDo.txt
travel_guides/berlitz2/Crete-History.txt
travel_guides/berlitz2/Crete-WhatToDo.txt
travel_guides/berlitz2/Crete-WhereToGo.txt
travel_guides/berlitz2/CstaBlanca-WhereToGo.txt
travel_guides/berlitz2/Cuba-History.txt
travel_guides/berlitz2/Cuba-WhatToDo.txt
travel_guides/berlitz2/Cuba-WhereToGo.txt
travel_guides/berlitz2/Nepal-History.txt
travel_guides/berlitz2/Nepal-WhatToDo.txt
travel_guides/berlitz2/Nepal-WhereToGo.txt
travel_guides/berlitz2/NewOrleans-History.txt
travel_guides/berlitz2/Paris-WhatToDo.txt
travel_guides/berlitz2/Paris-WhereToGo.txt
travel_guides/berlitz2/Poland-History.txt
travel_guides/berlitz2/Poland-WhatToDo.txt
travel_guides/berlitz2/Portugal-History.txt
travel_guides/berlitz2/Portugal-WhatToDo.txt
travel_guides/berlitz2/Portugal-WhereToGo.txt
travel_guides/berlitz2/PuertoRico-History.txt
travel_guides/berlitz2/PuertoRico-WhatToDo.txt
travel_guides/berlitz2/PuertoRico-WhereToGo.txt
travel_guides/berlitz2/Vallarta-History.txt
travel_guides/berlitz2/Vallarta-WhatToDo.txt
travel_guides/berlitz2/Vallarta-WhereToGo.txt
```