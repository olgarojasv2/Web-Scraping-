# How to scrape the Web using Python?
A case of Goodreads &amp; the Rijksmuseum

## Goodreads & Rijksmuseum Corpus

### Goodreads
Goodreads corpus consists of my personal reading list in Goodreads. The aim of this corpus was to investigate how our own data in Goodreads was presented and how much of our data is collected. 
This corpus is essentially text.

### Rijksmuseum 
The Rijksmuseum corpus consists of a list of six paintings belonging to the Rijksmuseum portrait collection. The corpus consists of paintings and text.

Both corpora are divided into two CSV files, with different categories that will be explored in the next section. All the information recollected and portrayed is in English.

## Data Collection Process

### Goodreads
Pandas was used in order to organise and visualise the data.
Before 2020 Goodreads had an API which gave developers access to their data. Nevertheless, that changed -all information is included in the Terms and Conditions of Goodreads-. Goodreads allows users to export their data in a CSV file form. The indications of how to access your information are in this link: 
https://help.goodreads.com/s/article/Does-Goodreads-support-the-use-of-APIs

### Rijksmuseum
Pandas and BeautifulSoup were used to scrape and visualise the data.
For the Rijksmuseum different links were utilised. Initially, the collections were analysed: https://www.rijksmuseum.nl/nl/collectie
Moreover, to minimise the scope, within the collection, the portraits were employed. This link was used to decide the corpus:
https://www.rijksmuseum.nl/nl/collectie/node/Portretten--a7c5ba17a2c44f96a25b7c8e0f6fa33d?collectionSearchContext=Art&page=1&sortingType=Popularity&facets[0].id=a7c5ba17a2c44f96a25b7c8e0f6fa33d&facets[0].nodeRelationType=HasRijksTheme

From that link, the selection of 6 paintings was made. These are the ones:
1. Self-portrait as the Apostle Paul
https://www.rijksmuseum.nl/nl/collectie/object/Zelfportret-als-de-apostel-Paulus--4faa97ed774e6e3f81b76cf3aed6226d?collectionSearchContext=Art&page=1&sortingType=Popularity&facets[0].id=a7c5ba17a2c44f96a25b7c8e0f6fa33d&facets[0].nodeRelationType=HasRijksTheme
2. <u> Self-Portrait Vincent van Gogh </u>
https://www.rijksmuseum.nl/nl/collectie/object/Zelfportret--72f97ac66c33f86b161cd51d62f7d365?collectionSearchContext=Art&page=1&sortingType=Popularity&facets[0].id=a7c5ba17a2c44f96a25b7c8e0f6fa33d&facets[0].nodeRelationType=HasRijksTheme
3. Portraits of Giuliano and Francesco Giamberti da Sangallo
https://www.rijksmuseum.nl/nl/collectie/object/Portretten-van-Giuliano-en-Francesco-Giamberti-da-Sangallo--ecf669da18531a3f30b41aa715a64428?collectionSearchContext=Art&page=1&sortingType=Popularity&facets[0].id=a7c5ba17a2c44f96a25b7c8e0f6fa33d&facets[0].nodeRelationType=HasRijksTheme
4. Portrait of Lysbeth van Duvenvoirde
https://www.rijksmuseum.nl/nl/collectie/object/Portret-van-Lysbeth-van-Duvenvoirde--299ed0752625ed80c9c43b67d6fefcd5?collectionSearchContext=Art&page=1&sortingType=Popularity&facets[0].id=a7c5ba17a2c44f96a25b7c8e0f6fa33d&facets[0].nodeRelationType=HasRijksTheme
5. Portrait of Marie Jeanette de Lange
https://www.rijksmuseum.nl/nl/collectie/object/Portret-van-mevrouw-Marie-Jeannette-de-Lange--443eae859f95c387ab0ad79562c98340?collectionSearchContext=Art&page=1&sortingType=Popularity&facets[0].id=a7c5ba17a2c44f96a25b7c8e0f6fa33d&facets[0].nodeRelationType=HasRijksTheme
6. <u> Isabella </u>
https://www.rijksmuseum.nl/nl/collectie/object/Isabella--ead5f623d828c7250ce5413e809b3551?collectionSearchContext=Art&page=1&sortingType=Popularity&facets[0].id=a7c5ba17a2c44f96a25b7c8e0f6fa33d&facets[0].nodeRelationType=HasRijksTheme

## CSV File Structure

### Goodreads
The CSV is divided into book id, title, author, additional authors, ISBN, my rating, average rating, publisher, binding, number of pages, year published, original publication year, date added, exclusive shelf, read count and owned.

### Rijksmuseum
The CSV is divided into title, date, description and image_url.


## Terms and Conditions Goodreads
As part of our overall commitment to continually improve our data management, Goodreads no longer issues new developer keys for our public developer API and plans to retire the current version of these tools. While we assess the value of APIs to determine how to support them in the future, we continue to support active API users who meet our terms of service. You are welcome to give your feedback on Goodreads APIs by completing the developer API survey.

You can follow these steps if you'd like to export your data from the site:

To import or export your books, go to My Books, then click on Import and Export under Tools on the left. From there:

To Import your books from a .csv, .txt, or .xls file, click choose file under Import from a File, select the file from your computer, then click on Import Books. The batch upload may take several minutes to process, depending on how large your file is.
To Export your books to a .csv file, click on the Export Library button at the top of the screen, below the Export heading, then wait for the file to generate. This may take some time if you have a large library. If successful, you will see a Your export from (date) - (time) note below the button. Click on that text to download the csv file.

## Terms and Conditions Rijksmuseum
### Introduction Information and Data Policy
The Rijksmuseum links individuals with art and history. Information and data play a vital role in making these connections possible. The Rijksmuseum's Information and Data Policy aims to share information and data about our collections with as many people as possible. While we make our information and data as openly available as possible, we also ensure the protection of sensitive and confidential information, such as personal data.

### What does the policy cover?
The Information and Data Policy outlines:

How the Rijksmuseum handles information and data related to the collection.
What users are allowed to do with our information and data.
What information and data we share, and the circumstances under which restrictions apply, such as privacy regulations or agreements with other parties.
We adhere to (inter)national standards to facilitate collaboration and the exchange of information. We also use open software formats wherever possible to promote the use of our information and data.

### Why an Information and Data Policy?
Since 2011/12, the Rijksmuseum has been sharing information and data through an open data policy, which was expanded in 2024. With the rapid growth of digital technology and the increase in digital research, more information and data about our collection and organisation have become available. The variety of data types has also increased. Our policy explains how we manage this wealth of information and data and make it as accessible as possible. We collaborate with the national and international heritage community, where standardisation, cooperation, and knowledge sharing are increasingly important.

### What can you do with our information and data?
According to our policy, much of the information and data on the Rijksmuseum's collection website and through our open data services can be freely used, including for commercial purposes, without needing to request permission. In some cases, however, usage restrictions apply, which are indicated on our collection website.

For much of the information and data on the collection website, you will find a Public Domain or Creative Commons Zero (CC0) Public Domain Dedication under the copyright notice, meaning you can use the material freely This means that the material is either free of copyright or the Rijksmuseum has waived its rights.
In some cases, copyright does apply. If so, a Creative Commons BY 4.0 (CC BY 4.0) licence is indicated. This allows you to use the material, as long as you acknowledge the Rijksmuseum as the source.
The collection website also contains information and data that are not freely available, such as photographs of objects that are still under copyright. In these cases, the copyright holder is indicated in the copyright notice.
