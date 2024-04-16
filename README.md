# temporal-reflections-of-societal-norms-and-biases



/opt/homebrew/bin/bash /Users/bilalimamoglu/repos/temporal-reflections-of-societal-norms-and-biases/scripts/download_data.sh


/opt/homebrew/bin/bash scripts/download_data.sh


python scripts/preprocess_data.py --data_source ny_times --model_name albert-base-v2 --years_list 1900 1910 1920 1930 1940 1950 1960 1970 1980 1990 2000 2010 --reprocess

python scripts/train_models.py --data_source ny_times --model_name albert-base-v2 --years_list 1900 1910 1920 1930 1940 1950 1960 1970 1980 1990 2000 2010 --num_epochs 3 --retrain

streamlit run scripts/visualize_pipeline.py
