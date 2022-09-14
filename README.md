# Japanese-OCR
Using CNNs to recognize Hiragana, Katakana and Kanji

The goal of this project is less to build a powerful model, but more to understand how various models and methods perform the task of OCR. Since Hiragana and Kanji are always side by side in a sentence, it made the most sense to deal with these together using two different strategies. The first strategy was to train a single model to
classify both the syllabary and the logography at once. The second strategy was to create an ensemble of models, first to train a model to classify whether a character was Hiragana or Katakana, then to train two different models, one for Hiragana and one for Kanji to classify each more accurately. Finally, I will distill my learnings to achieve a single model with the highest accuracy rate.

The data source I used is the ETL Character Database, found here: http://etlcdb.db.aist.go.jp/. It records handwritten English characters, Arabic numerals, Japanese Hiragana, Katakana and Kanji.
