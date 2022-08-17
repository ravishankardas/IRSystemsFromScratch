run:
	pip install numpy
	pip install pandas
	pip install nltk
	pip install num2words
	unzip ir-systems
	cd ir-systems && chmod +x test.sh && sh test.sh $(ARGS)
	
clean:
	rm -rf QRels_brs.csv
	rm -rf QRels_bm25.csv
	rm -rf QRels_tfidf.csv
	rm -rf ir-systems.zip
	zip -r ir-systems.zip ir-systems
	rm -rf ir-systems
