test:
	touch README.txt
	wget https://raw.githubusercontent.com/fivethirtyeight/data/master/murder_2016/murder_2015_final.csv
	head -n 1 ./murder_2015_final.csv > murder_header.csv
	tail -n +2 ./murder_2015_final.csv > murder_data.csv
	cat murder_data.csv | grep Illinois > murder_illinois.csv
	cat murder_data.csv | grep Maryland | wc -l > murder_maryland.count
	cat murder_illinois.csv | cut -d, -f3,4 > murder_illinois_2014-15.csv

