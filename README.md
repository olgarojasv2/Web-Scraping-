# How to scrape the Web using Python?
A case study of the Rijksmuseum

## Overview
This project demonstrates how to scrape data from the Rijksmuseum's online collection using Python. We focus on extracting information about six paintings from the museum's portrait collection, showcasing the power of web scraping for art historical research.

## Project Structure
1. Data Collection
2. Corpus Description
3. Tools and Libraries
4. Scraping Process
5. Data Structure
6. Ethical Considerations

## Data Collection

Pandas and BeautifulSoup were used to scrape and visualise the data.
For the Rijksmuseum different links were utilised. Initially, the collections were analysed: https://www.rijksmuseum.nl/nl/collectie
Moreover, to minimise the scope, within the collection, the portraits were employed. This link was used to decide the corpus:
https://www.rijksmuseum.nl/nl/collectie/node/Portretten--a7c5ba17a2c44f96a25b7c8e0f6fa33d?collectionSearchContext=Art&page=1&sortingType=Popularity&facets[0].id=a7c5ba17a2c44f96a25b7c8e0f6fa33d&facets[0].nodeRelationType=HasRijksTheme

From that link, the selection of 6 paintings was made. All these paintings are under the label of "public domain".
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

## Corpus Description

The Rijksmuseum corpus consists of a list of six paintings belonging to the Rijksmuseum portrait collection. Each entry contains both visual and textual data.

Both corpora are divided into two CSV files, with different categories that will be explored in the next section. All the information recollected and portrayed is in English.

## Tools and Libraries

We used the following Python libraries for web scraping and data processing:
Pandas: For data manipulation and CSV file creation
BeautifulSoup: For parsing HTML and extracting data

## Scraping Process
1. Initialize the Python project and import necessary libraries
2. Connect to the target URLs using requests
3. Parse the HTML content with BeautifulSoup
4. Extract relevant data (title, date, description, image URL)
5. Store the extracted data in a structured format (CSV)

## Data Structure

The scraped data is stored in a CSV file with the following columns:
- Title
- Date
- Description
- Image URL

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
