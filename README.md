# code origin

files have been added to this repo:

	https://github.com/c4software/python-sitemap.git

# original files

	README_ORIGINAL.md renamed from README.md
	
	config.json

	config.py

	crawler.py

	main.py

# data files (so you don't need to run below tasks yourself)

	www.epa.gov.xml
 
	www.epa.gov.csv

	cleaned_nofiles.txt (for astrid by request)


# steps to reproduce

1) clone this repo

`git clone http://github.com/openciti/epa`

2) enter repo directory
`cd  epa`

3) run main.py specifying a website and output file of your choice. example:

`python3 main.py --domain https://www.epa.gov --output www.epa.gov.xml`

3a) TODO pass above file values to scripts instead of hard coding them. Its assumed by other scripts that you're running exactly text in step 3) 

4) the above output has been saved here for your convenience:

[link to raw view of xml](https://raw.githubusercontent.com/openciti/epa/master/www.epa.gov.xml)

4) convert to csv:

`python3 tocsv.py`

5) the above output has been saved here for your convenience:

[link to raw view of csv](https://raw.githubusercontent.com/openciti/epa/master/www.epa.gov.csv)

6) optional. strip out links to files

`./nofiles.sh`

7) the above output has been save here for your convenience:

[link to raw txt](https://raw.githubusercontent.com/openciti/epa/master/cleaned_nofiles.txt)

8) TODO: the above script is runing on an aws server check its public web site for some UI (coming soon)

9) TODO: commit to git when script is done

10) TODO: generalize for any website / discover list of sites online

11) TODO: ontario gov

here: http://52.60.90.44/~ubuntu/

or

here: http://52.60.90.44
