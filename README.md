# Sentiment analysis and entity recognition
combined named entity recognition with sentiment analysis on Yelp reviews to recommend the best dishes for each restaunt

```bash
1. businesses.json: raw file containing restaurant data
2. menus.json: raw file containing menu data
3. reviews.json: raw file containing reviews data
4. quadruples.csv: file generated after performing named entity recognition
5. glove.6B.100d.txt: glove embedding
6. LSTM_project.model: LSTM trained model
7. result_file.csv: recommendations per restaurant generated using LSTM model

```
## Usage
1. Follow the colab jupyter notebook comments for execution.
2. The Recommendations generation section can be run directly by loading the already saved LSTM model. The code handles it, you can just run the section.
3. Major time consuming sections: Named entity recognition (~6 hours); BERT training and prediction (~3 hours)
4. You can load the quadruples.csv file directly as already done in code if you don't wish to perform named entity recognition.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)

## Note: 
Since the raw files are pretty large, download it from the link: https://drive.google.com/drive/folders/1nZ0seVC-VMecVUfeFXYmdcTIFGgjv2-H?usp=sharing
