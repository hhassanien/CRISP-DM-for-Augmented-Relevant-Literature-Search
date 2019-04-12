# CRISP-DM-for-Augmented-Relevant-Literature-Search
---------------------------------------------------


This is a repository with all sample executables mapping to the work done on the paper titled "Web Scraping Academic Repositories for Augmented Relevant Literature Search using CRISP-DM".

This repository works on extending the reach of applying extractive summarization for relevant literature search beyond open access repositories; if not all academic repositories especially, that many repositories do not follow open access standards? 
And, introduces a rather user-friendly advanced analytical methods using RapidMiner serving these principles of systematic reviews through a ZERO code approach?

The uploaded folders are labeled as follows:

	1-Web Scraper SiteMaps JSON	
	2-Scraping Raw Data	
	3-Worksbooks	
	4-RapidMiner Processes


-- Folder 1: 1-Web Scraper SiteMaps JSON	
-----------------------------------------
This folder contains the Web Scraper IO JSON Sitemaps metadata being used for scraping data from all the basket journals of AIS.

The same structure could be used by researchers in order to scrape data from Google Scholar. Only minor tuning would be required in these specific cases. On the other hand, the same structure could be readapted to suite any other academic repository


-- Folder 2: 2-Scraping Raw Data
---------------------------------
As sample output from the scraping tasks



-- Folder 3: 3-Worksbooks
-------------------------
These are the extarcts in Micorsoft Excel format


-- Folder 4: 4-RapidMiner Processes:
------------------------------------

The exported RapidMiner Processes being used for the purpose of applying the modelling stage of the CRISP-DM lifecycle. These are composed of two processes with readapted sub-tasks enabling researchers enhanced analysis of the outcomes:

	--- Process 1: 1-1_Similarity Process.rmp:
		This process executes a set of text mining tasks (Process Document TF-IDF, N-Grams, etc.) as well as CosineSimilarity to produce siilarity measures between all scraped literature titles

			-- Sub-Task 1: 1-2_ExampleSetID to N-Grams.rmp:
				This sub task readapts the output to present the N-Grams text making it easier for analysis

			-- Sub-Tasks 2: 1-3_ID to Titles.rmp:
			This sub task readapts the output to present the Original title making it easier for analysis

	--- Process 2: 2_Clustering & RandomForest.rmp:
		This process executes X-Means clustering algorithm with Cluster Model Visualizer for enhanced level of analyzing the scraped infromation adding a level of augmentation to the exercise of relevant literature search. It is to be noted that within this process Random Forest algorithm also gets executed in order to introduce a level of interpretation of how the key defniing words proliferate the corpora across the title keywords and corresponding outlets

		
