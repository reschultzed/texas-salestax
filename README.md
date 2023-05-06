# texas-salestax
This dataset consists of all Texas-based businesses and entities registered as sales taxpayers with the Texas Comptroller of Public Accounts, from the establishment of the state's sales tax in September 1961 up to April 19, 2023. Businesses and entities based outside of Texas that have been registered as sales taxpayers in Texas are not included in the dataset. There are over 6,168,000 entries, each of which represents a single taxpayer entity.

At the time this dataset was compiled in April-May 2023, all of the data could be publicly retrieved through the website of the Texas Comptroller of Public Accounts (https://mycpa.cpa.state.tx.us/staxpayersearch/). This dataset was compiled because only those taxpayer records which were active within the past four years could be downloaded as a single file, despite the fact that several decades' worth of additional data was visible through a manual search. To create the dataset, the website was searched for all ZIP codes between 75000 and 79999, and the results for each search were extracted and processed to remove extraneous text. In rare cases, records will list the wrong ZIP code and thus will be sorted incorrectly. In much rarer cases, a record for a Texas-based taxpayer may list a ZIP code outside the 75000-79999 range; the quantity of such errors is unknown and most such records were not compiled into this dataset.

Each file is a tab-separated .tsv document consisting of eight data columns. First is the name of the location represented in the record; second is its street address; third is the city or postal town designation of the location; fourth is the location's ZIP code. Fifth is the taxpayer ID of the business or entity responsible for the location, and this designation can be used to search for other locations belonging to the same entity through the "Taxpayer ID" field on the TCPA website (https://mycpa.cpa.state.tx.us/staxpayersearch/). Sixth is a sequential number distinguishing different locations operated by the same entity from one another. Seventh is the date on which the entity began paying sales taxes at the location; eighth is the date on which it stopped doing so. In most cases, these dates match up with the opening and closing dates of the business.

Because there are millions of records in this dataset, the data has been split into 51 .tsv files, each one representing a ZIP-3 region of the state of Texas. To find a particular location, download the file named for the first three digits of the location's ZIP code. Below is a table explaining the contents of each file.

| File | Largest city | Other major cities | Population | Entries |
| --- | --- | --- | --- | --- |
| 750 | Plano | Allen, Carrollton, Frisco, Garland, Grand Prairie, Irving, Lewisville, McKinney, Richardson | 2,561,000 | 510,737 |
| 751 | Mesquite | Corsicana, Duncanville, Forney, Waxahachie | 883,030 | 177,768 |
| 752 | Dallas |  | 1,375,223 | 420,067 |
| 753 | none |  | 0 | 482 |
| 754 | Greenville | Anna, Mount Pleasant, Paris, Princeton, Sulphur Springs | 380,385 | 79,174 |
| 755 | Texarkana | Atlanta, New Boston | 125,649 | 26,152 |
| 756 | Longview | Gilmer, Henderson, Kilgore, Marshall | 338,432 | 89,441 |
| 757 | Tyler | Athens, Jacksonville, Lindale | 372,375 | 94,080 |
| 758 | Palestine | Crockett, Trinity | 121,795 | 25,917 |
| 759 | Lufkin | Center, Jasper, Nacogdoches, Woodville | 254,506 | 59,890 |
| 760 | Arlington | Bedford, Burleson, Cleburne, Euless, Granbury, Grapevine, Hurst, Mansfield, Weatherford | 1,319,801 | 291,911 |
| 761 | Fort Worth | Haltom City, North Richland Hills | 1,061,369 | 218,874 |
| 762 | Denton | Argyle, Aubrey, Gainesville, Keller, Roanoke | 553,826 | 92,817 |
| 763 | Wichita Falls | Burkburnett, Iowa Park, Vernon | 170,239 | 46,011 |
| 764 | Stephenville | Bridgeport, Graham | 148,604 | 37,824 |
| 765 | Killeen | Belton, Copperas Cove, Fort Hood, Gatesville, Harker Heights, Temple | 546,068 | 90,059 |
| 766 | Hewitt | Hillsboro, McGregor, Mexia | 166,866 | 38,810 |
| 767 | Waco | Woodway | 187,617 | 53,704 |
| 768 | Brownwood | Brady, Early | 84,086 | 26,177 |
| 769 | San Angelo | Big Lake, Sonora | 136,690 | 38,161 |
| 770 | Houston |  | 3,201,957 | 812,354 |
| 771 | none |  | 0 | 62 |
| 772 | Houston |  | 4,459 | 1,586 |
| 773 | Spring | Conroe, Humble, Huntsville, Tomball | 1,386,067 | 229,474 |
| 774 | Katy | Bay City, Cypress, Missouri City, Richmond, Rosenberg, Stafford, Sugar Land | 1,377,578 | 196,233 |
| 775 | Pasadena | Alvin, Baytown, Friendswood, Galveston, League City, Pearland, Texas City | 1,305,833 | 244,028 |
| 776 | Port Arthur | Groves, Lumberton, Nederland, Orange, Vidor | 276,298 | 66,890 |
| 777 | Beaumont |  | 143,838 | 38,832 |
| 778 | College Station | Brenham, Bryan, Navasota | 340,765 | 65,921 |
| 779 | Victoria | Cuero, Port Lavaca, Yoakum | 169,218 | 45,339 |
| 780 | Laredo | Boerne, Helotes, Kerrville | 596,914 | 127,479 |
| 781 | New Braunfels | Beeville, Cibolo, Converse, Floresville, Schertz, Seguin, Universal City | 494,391 | 83,040 |
| 782 | San Antonio |  | 1,831,298 | 351,517 |
| 783 | Kingsville | Alice, Aransas Pass, Portland, Robstown, Rockport | 231,000 | 55,471 |
| 784 | Corpus Christi |  | 319,286 | 82,779 |
| 785 | Brownsville | Edinburg, Harlingen, McAllen, Mission, Pharr, Weslaco | 1,372,256 | 238,833 |
| 786 | Round Rock | Cedar Park, Georgetown, Leander, Pflugerville, San Marcos | 1,185,054 | 202,553 |
| 787 | Austin |  | 1,131,178 | 277,737 |
| 788 | Eagle Pass | Del Rio, Uvalde | 172,303 | 33,787 |
| 789 | La Grange | Columbus, Giddings, Smithville | 69,725 | 20,264 |
| 790 | Plainview | Borger, Canyon, Dalhart, Dumas, Hereford, Pampa, Perryton | 215,952 | 55,309 |
| 791 | Amarillo |  | 234,775 | 61,894 |
| 792 | Childress | Clarendon, Floydada, Quanah | 29,267 | 9,343 |
| 793 | Seminole | Brownfield, Lamesa, Levelland | 144,252 | 34,217 |
| 794 | Lubbock |  | 280,751 | 69,770 |
| 795 | Snyder | Clyde, Colorado City, Sweetwater | 94,160 | 27,437 |
| 796 | Abilene |  | 137,352 | 37,466 |
| 797 | Odessa | Andrews, Big Spring, Midland, Pecos | 445,848 | 116,546 |
| 798 | San Elizario | Alpine, Anthony, Canutillo, Clint, Fabens, Marfa, Presidio, Tornillo | 70,252 | 15,484 |
| 799 | El Paso | Fort Bliss, Horizon City, Socorro | 812,205 | 148,279 |
| 999 | Texhoma | data errors | 33 | 86 |
