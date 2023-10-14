# Sentiment Analysis
Data Extraction and Natural Language Processing

## Introduction 
Natural Language Processing (NLP) involves the use of Artificial Intelligence to analyze, interpret, and generate human language data. It enables computers to comprehend and manipulate language, facilitating tasks like translation, sentiment analysis, and chatbot interaction for improved human-computer communication and understanding. This comprehensive report elucidates the intricate processes of sentiment analysis, data extraction, and natural language processing (NLP), focusing mainly on extracting data from related URLs, performing text preprocessing and deriving various linguistic and readability features.

## Methodology

o	Data Extraction and Preprocessing
The initial step involved employing web scraping techniques to extract data from specific URLs. The data collected was stored in an Excel file titled 'Input.xlsx'. Subsequently, the extracted text underwent rigorous preprocessing to ensure data quality and uniformity. This preprocessing included the removal of HTML tags and punctuations, as well as conversion to lowercase, resulting in a clean and standardized text for further analysis.

o	Sentiment Analysis
Sentiment analysis played a pivotal role in this analysis. It was conducted using predefined positive and negative word dictionaries. Each word in the text was evaluated against these dictionaries to determine its sentiment. The following formulas were utilized to compute sentiment scores:
- Positive Score (PS): Number of positive words in the text;
- Negative Score (NS): Number of negative words in the text;
- Polarity Score: (PS−NS )/PS+NS+0.000001                          
- Subjectivity Score: (PS + NS)/Cleaned Words+0.000001 
['Cleaned Words' represents the total number of words after preprocessing];

o	Cleaning Using Stop Words Lists
To enhance the accuracy of subsequent analyses, a list of stop words was employed to filter out common and less meaningful words from the text. These stop words underwent preprocessing, involving the removal of punctuations, to ensure consistency in their format and effectiveness in subsequent analysis.

o	Analysis of Readability and Derived Variables
A comprehensive analysis of the text involved the computation of various derived variables that shed light on readability and linguistic intricacies. The formulas used to calculate these variables are as follows:
- Average Sentence Length: Average Sentence Length = Cleaned Words/Number of Sentences
- Percentage of Complex Words: Percentage of Complex Words = Complex Words/Cleaned Words
- Fog Index: Fog Index = 0.4×(Average Sentence Length + Percentage of Complex Words)
- Average Number of Words Per Sentence: Average Number of Words Per Sentence = Cleaned Words/Number of Sentences
- Complex Word Count: Number of words with more than 2 syllables
- Word Count: Total number of cleaned words
- Syllable Count Per Word: Syllable Count Per Word = Total Syllables/1042
- Average Word Length: Average Word Length = Total Word Characters/Cleaned Words

## Conclusion 
The rigorous application of sentiment analysis and the derivation of linguistic features offer profound insights into the underlying characteristics of the given text data. Understanding sentiment patterns and linguistic structures is imperative for a myriad of applications, including content analysis, sentiment tracking, and deriving meaningful insights from textual data.
For an in-depth and granular analysis, the final DataFrame can be referred which encapsulates the computed scores and derived variables, providing a holistic view of the text's sentiment and linguistic nuances. The integration of NLP techniques in this analysis underscores its significance in modern data analysis. Understanding sentiment patterns and linguistic structures is vital for making informed decisions and deriving valuable insights in an increasingly data-driven world.
