# Stress-detection-using-ML

## Stress Detection using Naive Bayes

![Depression Illustration](https://s3.amazonaws.com/spectrumnews-web-assets/wp-content/uploads/2018/06/22080230/JuliaYellow-Depression_1120x550_acf_cropped_1120x550_acf_cropped.jpg)

According to the World Health Organization, depression is the leading cause of disability worldwide. Globally, more than 300 million people of all ages suffer from the disorder. And the incidence of the disorder is increasing everywhere. Depression is a complex condition, involving many systems of the body, including the immune system, either as cause or effect. It disrupts sleep and it interferes with appetite; in some cases, it causes weight loss; in others, it contributes to weight gain. Depression is also often accompanied by anxiety. Research indicates that not only do the two conditions co-occur but that they overlap in vulnerability patterns.

Because of its complexity, a full understanding of depression has been elusive. Researchers have some evidence that depression susceptibility is related to diet, both directly—through inadequate consumption of nutrients such as omega-3 fats—and indirectly, through the variety of bacteria that populate the gut. But depression involves mood and thoughts as well as the body, and it causes pain for both those living with the disorder and those who care about them.

Even in the most severe cases, depression is highly treatable. The condition is often cyclical, and early treatment may prevent or forestall recurrent episodes. Many studies show that the most effective treatment is cognitive behavioral therapy, which addresses problematic thought patterns, with or without the use of antidepressant drugs. In addition, evidence is quickly accumulating that regular mindfulness meditation, on its own or combined with cognitive therapy, can stop depression before it starts by diminishing reactivity to distressing experiences, effectively enabling disengagement of attention from the repetitive negative thoughts that often set the downward spiral of mood in motion.

---
### Project Description

Stress, tension, and misery are undermining the psychological well-being of individuals. Each individual has a justification behind having an unpleasant life. Individuals frequently discuss their thoughts via web-based entertainment stages like on Instagram as posts and stories, and on Reddit through requesting ideas about their life on subreddits. In the beyond couple of years, many substance makers have approached to make content to assist individuals with their psychological wellness. Numerous associations can utilize pressure discovery to find which virtual entertainment clients are focused on to rapidly help them. Stress discovery is a difficult undertaking, as there are so many words that can be utilized by individuals on their posts that can show regardless of whether an individual is having mental pressure. The dataset I’m utilizing for this errand contains information presented on subreddits related on emotional wellness. This dataset contains different emotional well-being issues shared by individuals about their life. People often share their feelings on social media platforms. Many organizations can use stress detection to find which social media users are stressed to help them quickly.

### Bernoulli Naive Bayes

Naive Bayes is a machine learning model that is used for large volumes of data, even if you are working with data that has millions of data records the recommended approach is Naive Bayes. It gives very good results when it comes to NLP tasks such as sentimental analysis. It is a fast and uncomplicated classification algorithm.

#### Bayes Theorem

It is a theorem that works on conditional probability. Conditional probability is the probability that something will happen, given that something else has already occurred. The conditional probability can give us the probability of an event using its prior knowledge. 

##### Conditional Probability: 
![Bayes Theorem in cool led lamp](https://upload.wikimedia.org/wikipedia/commons/1/18/Bayes%27_Theorem_MMB_01.jpg)

Where, <br>
P(A): The probability of hypothesis H being true. This is known as the prior probability. <br>
P(B): The probability of the evidence. <br>
P(A|B): The probability of the evidence given that hypothesis is true. <br>
P(B|A): The probability of the hypothesis given that the evidence is true. <br>

#### Naive Bayes Classifier
- It is a kind of classifier that works on Bayes theorem.
- Prediction of membership probabilities is made for every class such as the probability of data points associated to a particular class.
- The class having maximum probability is appraised as the most suitable class.
- This is also referred as Maximum A Posteriori (MAP). 
- The MAP for a hypothesis is: 
  - 𝑀𝐴𝑃 (𝐻) = max 𝑃((𝐻|𝐸))  
  - 𝑀𝐴𝑃 (𝐻) = max 𝑃((𝐻|𝐸)  ∗ (𝑃(𝐻)) /𝑃(𝐸))  
  - 𝑀𝐴𝑃 (𝐻) = max(𝑃(𝐸|𝐻) ∗ 𝑃(𝐻))
  - 𝑃 (𝐸) is evidence probability, and it is used to normalize the result. The result will not be affected by removing 𝑃(𝐸).
- NB classifiers conclude that all the variables or features are not related to each other.
- The Existence or absence of a variable does not impact the existence or absence of any other variable.
- Example:  
  - Fruit may be observed to be an apple if it is red, round, and about 4″ in diameter.
  - In this case also even if all the features are interrelated to each other, and NB classifier will observe all of these independently contributing to the probability that       the fruit is an apple.  
- We experiment with the hypothesis in real datasets, given multiple features. 
- So, computation becomes complex.

#### Types Of Naive Bayes Algorithms
1. Gaussian Naïve Bayes:  When characteristic values are continuous in nature then an assumption is made that the values linked with each class are dispersed according to          Gaussian that is Normal Distribution.

2. Multinomial Naïve Bayes: Multinomial Naive Bayes is favored to use on data that is multinomial distributed. It is widely used in text classification in NLP.  Each event in      text classification constitutes the presence of a word in a document.

 3. Bernoulli Naïve Bayes:  When data is dispensed according to the multivariate Bernoulli distributions then Bernoulli Naive Bayes is used. That means there exist multiple        features but each one is assumed to contain a binary value. So, it requires features to be binary-valued.
---
### Objectives
Aim for this project is to build a machine learning model that can classify a text to two category: STRESS(0) or NO STRESS(1) using bernoulli naive bayes formula by calculating the sentiment of the frequency words in the training data.This model uses a 70:30 train to test ratio to detect the stress in an individual.
