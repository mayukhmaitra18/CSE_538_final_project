# A Contextual Recommendation Reporting System for Local Businesses
combined named entity recognition with sentiment analysis on Yelp reviews to recommend the best dishes for each restaunt

## Project environment
1. Used Google colab as implementation environment
2. To connect to google drive from colab:

```bash
from google.colab import drive
drive.mount("/content/drive",force_remount=True)
```


## Project folder setup
1. Create a folder named CSE_538 on google drive
2. Upload the all files and folders in directory CSE_538 or change the path variables in the code accordingly.
3. directory path for google colab will be:

```bash
/content/drive/My Drive/CSE_538
```
4. To navigate to above directory in google colab:

```bash
cd /content/drive/My Drive/CSE_538
```
5. The project folder will contain the below files:

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
