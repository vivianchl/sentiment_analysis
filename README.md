# Sentiment Analysis
## Background
### 1.	Why is sentiment Analysis important?

Customer reviews reflect the opinions and thoughts of consumers about the products they have purchased, which can have a significant impact on marketing strategies. For example, a brand can analyze customer reviews on social media to gain insights. If negative reviews increase, the company can take prompt actions to address customer concerns and improve satisfaction.

### 2.	What is Sentiment Analysis

Sentiment Analysis is the process of determining whether the sentiment expressed in a text is positive or negative. This analysis involves five key components: entity, attribute, opinion, holder, and time. Among these, the entity and aspect are collectively referred to as the "target." The main goal of sentiment analysis is to extract these elements from unstructured textual data, such as customer reviews, to gain valuable insights.
Example of review:

	“HUAWEI mobile phone has really good camera.

	Entity: HUAWEI mobile phone

	Aspect: camera

	Opinion: good (positive) ”

### 3.	Type of Sentiment Analysis
	
The main tasks of sentiment analysis can be divided into three types: Word-level sentiment analysis, sentence/document-level sentiment analysis, and target-level sentiment analysis.
Among them, the word-level and sentence-level analyses target the positive and negative sentiment of a word and the whole sentence, respectively, without distinguishing the specific targets in the sentence, such as entities or aspects, which is equivalent to ignoring the two elements of the five elements, namely entities and aspects.
Sentence-level/chapter-level sentiment analysis studies how to give sentiment labels to whole sentences or chapters, e.g., ‘The weather is very good today’ corresponds to the sentiment label ‘positive’.
Target-level sentiment analysis, on the other hand, considers a concrete target, which could be an entity, an aspect of an entity, or even the combination of an entity and its aspect. These can be divided into three categories: Target-grounded aspect based sentiment analysis (TG-ABSA), Target no aspect based sentiment analysis (TN-ABSA), Target aspect based sentiment analysis (T-ABSA)
Example of TG-ABSA:

	“The 2.0T turbocharged engine delivers strong performance, making overtaking at high speeds, such as 120 km/h, effortless. The exterior design is a model that both my wife and I find very appealing. However, the rear seating space is somewhat limited, and the fuel consumption is relatively high.

	Entity: Car

	Aspect and Opinion: engine(positive), design(positive), space(negative), fuel consumption(negative)"

Example of TN-ABSA:

	“HUAWEI mobile phone is better than iPhone.
 
	Entity1: HUAWEI mobile phone

	Entity2: iPhone

	Opinion1: positive (Entity1)

	Opinion2: negative (Entity2)”

Example of T-ABSA:

	“HUAWEI mobile phone has good camera, but Xiaomi has better quality-price ratio.
 
	Entity1: HUAWEI mobile phone 

	Aspect1: camera

	Entity2: Xiaomi

	Aspect2: quality-price ratio

	Opinion1: positive (Entity1)

	Opinion2: positive (Entity2)”

Each category can in turn be further divided into two main types of tasks: object recognition and sentiment recognition.
* Object Recognition: This involves two sub-tasks:

1.	Extracting words of evaluative object.
2.	Classifying words of evaluative object.
   
* Sentiment Recognition: This also consists of two sub-tasks:
1.	Extracting evaluative words.
2.	Classifying sentiments of evaluative words as positive or negative.

Example of review:

	“The phone features a powerful memory, a smooth operating system, and offers excellent quality-price ratio.
 
	Object: quality-price ratio

	Category of Object: Price

	Evaluative words: excellent
	
	Sentiment: positive”
