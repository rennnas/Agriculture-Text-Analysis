## What we talk about when we talk about innovation in Agriculture

This work intends to create the first attempt using text analysis tools while working with a database of studies related to innovation in agriculture. The objective here is to write the coding structure and apply it to a developing database, later advancing to a larger one, replicating the procedures developed here. In this way, I wrote the code so that it is possible to apply it in other databases without the necessity of significant changes.
Considering the ERC proposal’s intentions to understand the broad impacts of innovation in the agriculture sector, this work seeks to help in the definition of innovation within the field - what is considered innovation by different studies, its effects, applications and, mainly, what type of impact is mainly being measured. The analysis tries to give tools and assist in answering questions such as:
What types of studies are being done?
Which methodologies are being used mainly? What do they assess?
Is innovation mostly considered technological or governance processes? What are these technologies or policies?
What kind of result is expected from applying these innovations: productivity gains, the reduction of GHG emissions, or possibly an advance in the social conditions of agricultural workers?
And finally, is it possible to find a way to fully measure the impacts of innovation in agriculture, an assessment that addresses both environmental, social, and economic effects?

### Methodology
This work mainly uses the `quanteda()` package within the R program for the Text Analysis procedures. The package assists in creating tokens, matrices, and visualizations of qualitative and quantitative textual analysis processes. The database used in this project results from a research query extracted using the publish or perish program. The research query was delimited between the years 2010 and 2021, within the crossref database, resulting in more than 600 studies.
I used data transformation to Corpus and DFM format o identify the most frequent words and words associated with the word “innovation” to understand what these studies talk about when they talk about innovation.
![](https://github.com/rennnas/Agriculture-Text-Analysis/blob/main/imagem%201.png)

#### Dictionary analysis
A dictionary analysis also allows us to have a more accurate observation of the objectives and interests of the different studies. It was possible to create three types of dictionaries to help us in the investigations:
Dictionary of impact analysis associating terms for “environmental impact”, “social impact”, and “economic impact”;
Dictionary of methodologies, associating terms to each type of industrial ecology methodology;
Dictionary of innovations, differentiating technological innovation from governance innovation.
The analysis from the dictionaries allows us to make observations such as which methodologies are being most used in the studies, if the innovations fall mainly on the technical or governance innovation side, and understand the type of impact prioritized by these studies.
![](https://github.com/rennnas/Agriculture-Text-Analysis/blob/main/imagem%202.png)
 
#### Text Analysis: Topic Modeling
Topic model is a textual statistical analysis used to extract “topics” within a collection of documents, creating patterns within a set of topics. With supervised human analysis, it is possible to understand the frequently associated terms with the same set. This allows us to observe, for example, the terms associated with each methodology or the terms associated with each type of innovation. Through the packages `topicmodels()`, `LDAvis()` and `servr()` we build the topics.
 
![](https://github.com/rennnas/Agriculture-Text-Analysis/blob/main/Imagem%203.png)
 
 
### Next Steps
Through topic modeling and dictionaries, it is possible to create an application that individually defines the methodology used by each paper. From this, it is possible to associate terms for each method, which has the potential to connect the terms inside each topic to each methodology. Likewise, this product can be replicated to understand each type of innovation and impact analysis, understanding what processes are mostly connected to each type of impact analysis or each type of innovation process.
 
![](https://github.com/rennnas/Agriculture-Text-Analysis/blob/main/Imagem%204.png)
