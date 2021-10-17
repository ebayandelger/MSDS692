<h1>Sentiment Analysis on Reddit's posts about Dogecoin</h1>

<h3>SUMMARY</h3>
Financial experts are highly skeptical of dogecoin, as well as other cryptocurrencies. Their extreme volatility is one reason experts say that crypto is a risky, speculative investment. That's why only the younger generation is investing in dogecoin but I am not sure if they even understand how dogecoin actually works or they care to know. Me and my colleagues had a big debate about dogecoin recently arguing whether it’s a good investment or not. And we couldn't reach an agreement because simply we did not understand how cryptocurrency worked. So, I decided to pick Dogecoin as my project for MSDS 692 Practicum I and learn about it at the same time.
<p> I performed a sentiment analysis on Reddit posts to see if people are posting positive information or negative information. Then, I based my outlook on that descriptive analysis I performed about Dogecoin.</p>
<h3>TOOLS & LIBRARIES USED</h3>
Jupyter Notebook</br>
The Jupyter Notebook is an open-source web application that allows to create and share documents that contain live code, equations, visualizations and narrative text. Uses include: data cleaning and transformation, numerical simulation, statistical modeling, data visualization, machine learning, and much more.</br></br>
The Jupyter Notebook file that contains my python script: Sentiment.ipynb</br></br>
The Python Reddit API Wrapper (PRAW)</br>
PRAW is a python module provides a simple access to Reddit's API that is easy to use and follows all of Reddit's API rules. Beneficial specially for someone who is new to python programming language and no need to learn about API which has a steep learning curve.</br></br>
Valence Aware Dictionary and sEntiment Reasoner (VADER)</br>
<p>VADER is a lexicon and rule-based sentiment analysis tool that is specifically designed and trained for social media posts. VADER uses a combination of A sentiment lexicon is a list of lexical features which are generally labeled according to their semantic orientation as either positive or negative. VADER not only tells about the Positivity and Negativity score but also tells us about how positive or negative a sentiment is.</p>
<h3>STEP 1</h3>
<p>Created a Reddit instance using PRAW, then got all the data and formatted them using panda's data frame function. Saved 1000 post files to dump.csv file type due to Reddit's policy. Later, I combined them manually before performing sentiment analysis on the data.</p> 
<h3>STEP 2</h3>
<p>VADER module was easy to use and within couple of expressions, I was able to visualize the data already. Performed a sentiment analysis using Vader's powerful package by typing few commands like ".polarity_scores".</p>
<h3>STEP 3</h3>
<p>Printed results to do a quick visualizationn:</br>
</br>
print(df.label.value_counts())</br>
print(df.label.value_counts(normalize=True) * 100)</br></br>
 1    1679</br>
 0     506</br>
-1     222</br>
Name: label, dtype: int64</br>
 1    69.754882</br>
 0    21.022019</br>
-1     9.223099</br>
Name: label, dtype: float64</br></br>
At last, I plotted the data on a graph to provide a better visualization.</p>
