**Version 0.3 fixes a few of the more glaring holes, especially PPC vs Intel issue that required "reverse Unicode" trick**

Here's a situation: you have a bunch of MP3s of Russian (or Cyrillic in general) songs that you decided to drag-and-drop add to your iTunes library.  No problem with that, except every once in awhile you end up with songs/artists/albums named using "birds language" instead of proper Cyrillic letters.

I have once in the past stumbled onto a small AppleScript solution that fixed that, but I was unable to trace it down again.  I have, therefore, decided to "scratch this particular itch" and build one myself.

See

  * ImplementationDetails
  * InstallingConvertRussian
  * RunningConvertRussian

for details.



---


**Версия 0.3 содержит несколько очень важных исправлений, в том числе адресующих "обратный Unicode"**

Проблема: ваша коллекция MP3 была создана на Windows или по какой–либо иной причине ID3 тэги были записаны в кодировке cp-1251 (a.k.a. win-1251 или ms-cyrillic).  Вы наконец купили Мак и только что перетащили все это "собрание сочинений" в iTunes.  О, ужас — вместо нормальных названий исполнителей и песен, вы видите кучу непонатных символов.

Вот тут–то as-convert-russian и может вам помочь.  Он транслирует extended ASCII символы из кодировки Mac Latin (поскольку именно в эту кодировку они попали) в Unicode, в котором они замечательно будут сохранены в iTunes.