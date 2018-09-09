download:
	mkdir -p data
	wget www.derekruths.com/static/reading_tweets/books_tweets100000.txt.gz -P ./data/ 
	gunzip ./data/books_tweets100000.txt.gz
	

prep:
	cat ./data/books_tweets100000.txt | jq '. | {userid: .user.id, created_at: .created_at, lang: .user.lang, text: .text}'	

analyze:


