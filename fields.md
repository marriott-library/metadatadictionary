# Marriott Library Metadata Dictionary

General metadata fields present in our [digital library](https://collections.lib.utah.edu/). Indivdual collections may have more specialized collection templates with additional fields.

Note: This is currently a draft, some examples and specifications are still being added.



| Local Field Name      	| **Title**                                                                                                                                                                                                                	|
|-----------------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Dublin Core Mapping   	| dcterms:title
| Solr field            	| title_t    | 
| Explanation           	| Some objects, such as scanned text documents, have their own titles we can use, but if not, we think up a simple, descriptive title that conveys what,the work is about. Omit initial articles. Be succinct where possible, depending on the format of the item. Complex items might require longer titles. If you have multiple items in the same collection with the same title, distinguish by numbering them.                      	|
| Examples              	| **(Oral history)** Virginia P. Frobes, Salt Lake City, Utah: an interview by Everett L. Cooley.<br />    **(Letter,in a manuscript collection)** Correspondence between Aziz Atiya,and E. A. Lowe regarding an Arabic Sinai manuscript. <br /> **(Photograph)**	Horse drawn wagon on a barren plain. <br /> **(From Wayne Russell McConkie Photograph Collection)** Unidentified geological feature 04 <br /> **(Video)** Baden-Baden, Garmisch 1968: Joseph S. Peery, Home movie 30. <br /> **(Compound object in a manuscript collection)** Letters from American missionaries in China, April 1927 |
|  Controlled Vocabulary 	| No     |                                                                                            |  Required               | Yes     	|
|  Data Type             	| Text       |      



| Local Field Name      	| **Description**                                                                                                                                                                                                              	|
|-----------------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Dublin Core Mapping   	| dcterms:description                                                                         
| Solr field             	| description_t    |                                                                                                                            	
| Explanation           	| We can provide more details here that tell a user various information about the resource, from contents to the nature of the original work that was digitized. We attempt to be succinct, with 2-3 sentences used depending on the nature of the item being described.                      	|
| Examples              	| **(Oral history)** Transcript (59 pages) of interview by Winnifred Margetts with Wanda Clayton Thomas, retired Communications and Theater professor at the University of Utah, on March 6, 1985. This interview is no. 64 in the Everett L. Cooley Oral History Project, and tape nos. 255 and 256. <br>  **(Letter in a manuscript collection)** Letter dated 8 November 1996 from Alf M. Engen to the Board of Directors of the Alf Engen Ski Museum Foundation, regarding the progress toward choosing a site for the museum and thanking them for the decision to name it in his honor. <br>  **(Photograph)** Photo shows Chimney Rock, located north of Utah Highway 24 on the west side Capitol Reef National Park, Utah. <br /> **(Video)** Home movie (16mm film, no sound) showing clips of scenic views, the forest service employees building a bridge, and two men including Orange A. Olsen Ice fishing and making fire; location not identified. Length: 1 minute, 28 seconds. <br /> **(Compound object in a manuscript collection)** A set of letters to Earl Douglass dated 1904, 1905, 1906, and 1907 from niece Gretta Battin at Faribault, Minn.; sister Ida Battin at Medford, Minn.; Aunt Felitia Rockwood in Limerick, New York; niece Viola Battin at Maple Plains, Minn.; and an Aunt Jennie. | 
| Controlled Vocabulary 	| No    |                                                                              	
| Required              	| Yes      	|
| Data Type             	| Text             |

| Local Field Name      	| **Creator**                                                                                                                                                                                                               	|
|-----------------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Dublin Core Mapping   	| dcterms:creator |
| Solr Field               | creator_t                                                                                     |
| Explanation           	| Who is responsible for the creation of the original work?  If a manuscript document, who wrote it? If a photograph, who took the picture?  If an oral history, who is the subject (the interviewee)?  And so on.  We enter this in the manner traditionally used in cataloging records: last name first, and we check the Library of Congress name authority file, a controlled vocabulary of names of people, and use the form found there, if available.  One difference from MARC cataloging is that multiple authors of a work can be recorded in this field.                      	|
| Examples              	| **(Author of a letter)** Morgan, John (John Hamilton), 1842-1894 <br> **(Both authors in a set of letters exchanged between two people)** Whitaker, John Mills, 1863-1960; Taylor, Ida Taylor Whitaker, 1887-1980 <br> **(Person interviewed)** Engen, Alan K.<br> **(Photographer)** Kelly, Charles, 1889-1971 </br> **(Producers of a video)**  Juarez, Maricruz; Fuwell, Judy	|
| Controlled Vocabulary 	| Use [LCNAF when appropriate.](http://id.loc.gov/authorities/names.html) Can also use the [Western Name Authority File](https://exhibits.lib.utah.edu/s/wnaf/page/welcome) 	|
| Required              	| Mandatory when applicable    |                                                                     
| Data Type             	| Text    |

| Local Field Name      	| **Collection Name and Number**                                                                                                                                                                                                               	|
|-----------------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Dublin Core Mapping   	| None     
|Solr Field               | collection_name_and_number_t      	|
| Explanation           	| Used for collection name and number to reflect the physical location of a digitized resource. This is especially useful to identify distinct sections of a larger collection, such as individual collections in the Multimedia Photo Archives.                     	|
| Examples              	| P0100 Charles Kelly Photograph Collection <br> P0413 Alan K. Engen Photograph Collection	|
| Controlled Vocabulary 	| No 	|
| Required              	| No    |                                                                                           
| Data Type             	| Text   |    


| Local Field Name      	| **Contributor**                                                                                                                                                                                                                	|
|-----------------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Dublin Core Mapping   	| dcterms:contributor   
| Solr field          	| contributor_t    | 
| Explanation           	| Other people or corporate bodies that play some important role in the resource's creation.  Again, we use the officially established form of the name, if available, or enter the name according to the same standards used in the LC authority file.                      	|
| Examples              	| **(Interviewer for an oral history)** Thompson, Gregory C. (Gregory Coyne), 1943- ; <br>**(Head coach for a University of Utah football training video)** Meek, Bill (William M.), 1922-1988 	|
| Controlled Vocabulary 	| Use LCNAF when applicable                                                                                                                                                                                            	|
| Required              	| No                                                                                                                                                                                                                  	|
| Data Type             	| Text       |      

| Local Field Name      	| **Date**                                                                                                                                                                                                                	|
|-----------------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Dublin Core Mapping   	| dcterms:date   
| Solr field          	| date_t    | 
| Explanation           	| When was the original resource created? Some resources are quite clear, such as a dated letter or a photo with the date stamped on it. (Exact dates take a prescribed format: yyyy-mm-dd.) Others resources require us to make an educated guess, and we enter a range of years to cover the likely time period during which it was created. For circa dates, we use a 5 year range.          	|
| Examples              	| **(When exact date is given e.g., January 31, 1975)** 1975-01-31 <br> **(When an estimated range of years is given e.g., 1960s or 1970s)** 1960; 1961; 1962; 1963; 1964; 1965; 1966; 1967; 1968; 1969; 1970; 1971; 1972; 1973; 1974; 1975; 1976; 1977; 1978; 1979 <br> **(When a single estimated year is given, e.g., circa 1960)** Enter a range of dates on either side of that date. For example: 1957; 1958; 1959; 1960; 1961; 1962; 1963 <br> **(A range of months)** 1940-02; 1940-03; 1940-04 |
| Controlled Vocabulary 	| W3C Date Time Format profile of ISO 8601    	|
| Required              	| Yes       	|
| Data Type             	| Date       |      

| Local Field Name      	| **Format**                                                                                                                                                                                                                	|
|-----------------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Dublin Core Mapping   	| dcterms:format   
| Solr field          	| format_t    | 
| Explanation           	| File format for the digital item. In the SIMP tool, this field is automatically extracted.  |
| Examples              	| application/pdf <br> image/jp2 <br> audio/mp4 <br>	|
| Controlled Vocabulary 	|  [Internet Media Type, IMT Scheme](http://www.iana.org/assignments/media-types/)          	|
| Required              	| Yes         |                                                                                       
| Data Type             	| Text       |      



| Local Field Name      	| **Genre**                                                                                                                                                                                                                	|
|-----------------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Dublin Core Mapping   	| dcterms:medium   
| Solr field          	| genre_t    | 
| Explanation           	| Use this field to describe the nature of the original object (what it is and not what it is about), not the digital copy. When using the Getty Art & Architecture Thesaurus terms, leave all in lower case at it appears in the resource.                     	|
| Examples              	| black-and-white negatives <br> color negatives<br> matchbooks<br> oral histories (literary works)<br> correspondence<br> 35mm (photographic film size)<br> tintypes (prints) 	|
| Controlled Vocabulary 	| Use [Getty Art & Architecture Thesaurus](http://www.getty.edu/research/tools/vocabularies/aat/)          	|
| Required              	| No         |                                                                                       
| Data Type             	| Text       |      


| Local Field Name      	| **File Name**                                                                                                                                                                                                                	|
|-----------------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Dublin Core Mapping   	| none   
| Solr field          	| file_name_t    | 
| Explanation           	| File name of digitized resource, a unique identifier whose form varies between resources;  Sometimes it is constructed to be based on a numbering scheme in the original collection                     	|
| Examples              	| **(Scan of John Mills Whitaker papers, section 2, box 10, folder 33)**  0002_10_33.pdf 	|
| Controlled Vocabulary 	| No          	|
| Required              	| Yes       	|
| Data Type             	| Text       |      


| Local Field Name      	| **Is Part Of**                                                                                                                                                                                                                	|
|-----------------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Dublin Core Mapping   	| dcterms:ispartof  
| Solr field            	| is_part_of_t    | 
| Explanation           	|  Used for faceting and discovery for identified items that are part of a larger collection in Marriott Library Special Collections, especially the large Multimedia Photo Archive              	|
| Examples              	| Ski Archive <br> Utah River Running Archives 	|
| Controlled Vocabulary 	| No               |                                                   	
| Required              	| No                |                                                                    
| Data Type             	| Text       |      



| Local Field Name      	| **Keywords**                                                                                                                                                                                                                	|
|-----------------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Dublin Core Mapping   	| none 
| Solr field            	| keywords_t    | 
| Explanation           	|  A useful field for synonyms of the subject headings or other specific phrases not in the LC subject headings. We put significant words that apply to the contents of the resource.             	|
| Examples              	| **(Photo of a natural sandstone arch in Kane County, Utah)**  Landforms; Sandstone; Natural arches 	|
| Controlled Vocabulary 	| No           	|
| Required              	| No              	|
| Data Type             	| Text       |   


| Local Field Name      	| **Relation**                                                                                                                                                                                                                	|
|-----------------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Dublin Core Mapping   	| dcterms:relation 
| Solr field            	| relation_t    | 
| Explanation           	| Used to provide larger context about a collection. For Marriott Library Special Collections, we place the URL for the Finding Aid in this field for harvesting by Archives West             	|
| Examples              	| http://archiveswest.orbiscascade.org/ark:/80444/xv43640  	|
| Controlled Vocabulary 	| No               	|
| Required              	| No        	|
| Data Type             	| Text       |      


| Local Field Name      	| **Rights**                                                                                                                                                                                                                	|
|-----------------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Dublin Core Mapping   	| dcterms:rights 
| Solr field            	| rights_t    | 
| Explanation           	| For new collections, we use the URIs from rightsstatements.org             	|
| Examples              	| http://rightsstatements.org/vocab/InC-EDU/1.0/ <br>Note that the practice of claiming copyright on a digital image, e.g."Digital image copyright 2007, Marriott Library" reflects outdated understanding of rights for digital surrogates, and is being remediated in Marriott Library Collections.	|
| Controlled Vocabulary 	| https://rightsstatements.org/en/                                                        
| Required              	| Yes                                                                                                                                                                                                              	|
| Data Type             	| Text       |   


| Local Field Name      	| **Rights Holder**                                                                                                                                                                                                               
|-----------------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Dublin Core Mapping   	| dcterms:rightsholder 
| Solr field            	| rights_holder_t    | 
| Explanation           	| Information about the holder of copyright for an item             	|
| Examples              	| Copyright Trent Harris, 1984	|
| Controlled Vocabulary 	| no                                                      
| Required              	| Yes, when applicable                                                                             |
| Data Type             	| Text       |   

| Local Field Name      	| **Accesss Rights or Rights Management**                                                                                                                                                                                                                	|
|-----------------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Dublin Core Mapping   	| none
| Solr field            	| access_rights_t    | 
| Explanation           	| Additional textual rights information about an item. Can contain contact information about contact information for reproduction requests.           	|
| Examples              	| Copyright 2010. For further information regarding the rights to this collection, please visit: https://NOVEL.utah.edu/about/copyright <br> Image files courtesy National Park Service. Converted to jpg2000 delivery format and made available by the Western Soundscape Archive at Westernsoundscape.org under the Creative Commons Attribution-Noncommercial-No Derivative Works 3.0 United States License; http://creativecommons.org/licenses/by-nc-nd/3.0/us/ <br> 	|
| Controlled Vocabulary 	| No                                                      
| Required              	| No       	|
| Data Type             	| Text       |   


| Local Field Name      	| **Spatial Coverage**                                                                                                                                                                                                                	|
|-----------------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Dublin Core Mapping   	| dcterms:spatial 
| Solr field            	| spatial_coverage_t    | 
| Explanation           	|  If a resource is focused on an identifiable geographic place, we enter that here. We use a format that includes a hierarchy of broader regions: the location's county when applicable, state, and country. Multiple places may apply to the same resource. [Note: Some legacy collections, such as the Multimedia Archives Photos, still use the Library of Congress format.]              	|
| Examples              	| **(Geonames)** Alta, Salt Lake County, Utah, United States<br> Glen Canyon National Recreation Area, Utah, United States<br>**(Multimedia Archives photo from a Glen Canyon river trip, using LCSH)** Colorado River (Colo.-Mexico); Glen Canyon (Utah and Ariz.) 	|
| Controlled Vocabulary 	| [Geonames](https://www.geonames.org/)                                                                                                                                            	|
| Required              	| Strongly recommended                        |
| Data Type             	| Text       |      


| Local Field Name      	| **Source**                                                                                                                                                                                                                	|
|-----------------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Dublin Core Mapping   	| dcterms_source 
| Solr field            	| source_t    | 
| Explanation           	|  Information to help locate the original item that was the basis of the digital scan, such as a call number or local identifier.      	|
| Examples              	| **(Original call number for a scanned rare book, Thomas Paine's Common Sense)**  E211 .P124  <br> **(Photo number from the Multimedia Photo Archives)** P0013n10_115_2282 	|
| Controlled Vocabulary 	| No                                                                                                                                           	|
| Required              	| No                                                                                                                                                                                                          	|
| Data Type             	| Text       |      


| Local Field Name      	| **Type**                                                                                                                                                                                                                	|
|-----------------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Dublin Core Mapping   	| dcterms_type 
| Solr field            	| type_t    | 
| Explanation           	|  Assign a value based on the DCMI type vocabulary to describe the resource      	|
| Examples              	| Text <br> Image <br> Image/MovingImage	|
| Controlled Vocabulary 	| [DCMI Type Vocabulary](http://www.dublincore.org/specifications/dublin-core/dcmi-type-vocabulary/2010-10-11/)                                                                                                                                           	|
| Required              	| Yes                                                                                                                                                                                                          	|
| Data Type             	| Text       |      






