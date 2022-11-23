# Mahabharata-IR
The Related Presentation can be viewed at: 
https://docs.google.com/presentation/d/1TenrpWsWxaGo2ON3zitf8jYmjbOhnyPoiGU7KA8EcK4/edit#slide=id.g4dfce81f19_0_45

# Description of the Project:
This is a Mahabhartha IR System which provides one word answer to questions related to Mahabhartha Epic.The system was build in following steps:<br >
 1- We Divided the entire Mahabhartha story in smaller paragraphs also called chunks.<br >
 2- We created a query set which was set of questions to be asked<br >
 3-Now,these chunks were passed to BM25 Model along with the query set to get top-5 most relevant passages for the particular query.<br >
 4-We used variety of models mainly DistilRoberta-Bert and pyserini to find the most relevant passage out of 5 passages selected by BM25 for particular question.<br >
 5-This relevant passage along with question was passed to Question-Answering Bert which was trained over squad2.0 dataset.We Manually built test-dataset
which was in accordance with the squad2.0 over which BERT was fine-tuned.<br >
 6- Upon giving relevant passage for particular question,the QnA BERT was able to extract one word or one-liner asnwer for the question.
