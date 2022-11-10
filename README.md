# Workshop OpenRefine & Wikimedia Commons

[OpenRefine](https://openrefine.org/) is a well-known tool for editing, enriching and manipulating data. It is widely used within the Wikimedia community to add data to Wikidata. As from version 3.7, you can also upload images to Wikimedia Commons, enriched with [structured data](https://commons.wikimedia.org/wiki/Commons:Structured_data).

## Learning objectives
In this workshop you will learn
 * how to use OpenRefine to upload new images with regular file descriptions (Wikitext) and structured data to Wikimedia Commons, and
 * how to add structured data to existing Commons files, using OpenRefine

## Target audience
This workshop is suitable for people who have used OpenRefine before to add data to Wikidata, and who know what "reconciling against Wikidata" means, but who do not yet know how to use OpenRefine to add images and structured data to Wikimedia Commons. This workshop is therefore **not suitable for** people who have never worked with OpenRefine and/or Wikidata.

 ## Required preparation
* Please bring your own laptop to this workshop.
* Make sure you know your way around OpenRefine v 3.4, 3.5 or 3.6, and are comfortable with reconciling and uploading data to Wikidata.
* Install OpenRefine 3.7 SNAPSHOT on your machine. It can be downloaded at https://github.com/OpenRefine/OpenRefine#snapshot-releases. Please note: 
   * this is an unstable release, functionalities can change from release to release and may or may not work, depending on the exact snapshot release you have installed. Don't be suprised if some things that works yesterday and/or today will stop working tomorrow. 
   * Version 3.6.2 (or older) is **not** suitable, because you cannot upload files to Wikimedia Commons with it.
* If you have time: check out [OpenRefine 3.7+ – How to upload new files to Wikimedia Commons](https://docs.google.com/document/d/19eiMeq3XssiPrT9b04E-8XyE-desBEzYNgygLDYKP4o/edit)

## Working materials

* **OpenRefine 3.7 SNAPSHOT**: It can be downloaded at https://github.com/OpenRefine/OpenRefine#snapshot-releases. (See remarks above).

* **URLs needed by OpenRefine 3.7+**:
For OpenRefine 3.7+ to be able to upload images to Commons, we will need to add a couple of URLs to it: 
  * *Wikidata reconciliation service* - to allow OpenRefine to reconcile local data against Wikidata
    * https://wikidata.reconci.link/en/api (English) 
    * https://wikidata.reconci.link/nl/api (Dutch) 
  * *Wikimedia Commons reconciliation service* - to allow OpenRefine to reconcile local file names against Wikimedia Commons File:-names 
    * https://commonsreconcile.toolforge.org/en/api (English) 
    * https://commonsreconcile.toolforge.org/nl/api (Dutch) 
  * *Wikimedia Commons manifest* - so OpenRefine knows that Wikimedia Commons is a special Wikbase instance it can talk/upload to.
    *  https://raw.githubusercontent.com/OpenRefine/wikibase-manifests/master/wikimedia-commons-manifest.json 

* **Online images**: We are going to upload the 18 images from *[Nederlandsche havengezichten enz.](http://resolver.kb.nl/resolve?urn=urn:gvn:KONB16:533939704)* to Commons. These images can be directly requested via URLs such as http://resolver.kb.nl/resolve?urn=urn:gvn:KONB16:533939704&role=page&count=4&size=large (count=1, count=2, count=3... count=18)

* **Local images**: In total this page holds 18 individual images, which have been downloaded into the *[images](/images)* folder in this repo. 

* **Commons category**: As a preparation for this workshop, a couple these images have already been uploaded to the Commons [Category:Nederlandsche_havengezichten_enz.,_1780-1781_-_KONB16:533939704](https://commons.wikimedia.org/wiki/Category:Nederlandsche_havengezichten_enz.,_1780-1781_-_KONB16:533939704). These will be used for illustration and demo purposes. 

* **Example file**: One file within this category is [File:De Haven van Amsterdam - Nederlandsche havengezichten enz. - KONB16-533939704 - Prent 3 van 18.jpg](https://commons.wikimedia.org/wiki/File:De_Haven_van_Amsterdam_-_Nederlandsche_havengezichten_enz._-_KONB16-533939704_-_Prent_3_van_18.jpg). We will use this example file for guidance, it holds  
  * Wikitext : based upon the [{{Artwork template}}](https://commons.wikimedia.org/wiki/Template:Artwork)
  * Structured data : using [depicts (P180)](https://www.wikidata.org/wiki/Special:EntityPage/P180), [copyright status (P6216)](https://www.wikidata.org/wiki/Special:EntityPage/P6216), [source of file (P7482)](https://www.wikidata.org/wiki/Special:EntityPage/P7482) and [collection (P195)](https://www.wikidata.org/wiki/Special:EntityPage/P195) as a minimal set.  

* **Excel file**: All necessary data for our uploads to Commons is contained in [this Excel-file](Dataset_WorkshopOpenRefine_WikiconNL19112022.xlsx?raw=true). It will be used as input for creating our OpenRefine project during the workshop.

* **OpenRefine schema**: The OpenRefine schema that will be used to upload the images and data to Commons [can be found here](add URL)

* **PDF slides**: The outline, explanations, tips & tricks etc. that will be demonstrated during the workshop can be seen in [this PDF-presentation](add Commons URL PDF) 

## Workshop leader
This workshop is given by [Olaf Janssen](https://www.wikidata.org/wiki/User:OlafJanssen), the Wikimedia coordinator of the [Koninklijke Bibliotheek](https://www.kb.nl/over-ons/experts/olaf-janssen), the national library of the Netherlands. In this role he stimulates and facilitates collaboration between the collections, knowledge, open data and staff of the KB on the one hand, and the projects of the Wikimedia movement, such as Wikipedia, Wikimedia Commons, Wikidata and Wikibase, on the other. He is also active as a volunteer within the community.

## Workshop instances
This workshop was given during
* [WikiconNL 2022](https://web.archive.org/web/20221014171306/https://www.wikimedia.nl/wikiconnl/), 19 november 2022, Utrecht, The Netherlands. See the [programme](https://web.archive.org/web/20221103154543/https://www.wikimedia.nl/programma-2022/) and the [session description](https://web.archive.org/web/20221110131459/https://www.wikimedia.nl/sessies2022/)

## Licensing
All workshop materials are released into the public domain under the [Creative Commons Zero v1.0 Universal](LICENSE) and can therefore be reused freely and openly. Attribution is not required, but still appreciated.
