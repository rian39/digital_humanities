# Diagrammatic intensities: modelling methods in digital humanities

## abstract
This paper concerns that part of the digital humanities that makes use of data analytic techniques that go by the names 'data mining', 'machine learning' or 'pattern recognition.'
These techniques, while not exactly new and in many cases of long-standing provenance, animate and drive many of the most prominent data-intensive digital humanities projects. 
Following C.S. Peirce and F. Guattari, we can identify a diagrammatic component of the digital humanities. 
The diagrammatic takes several different semiotic forms in data analytic techniques: the data plot (histogram, scatterplot, line plot, network plot, etc.); the algebraic expression (the probability distribution; the error function, etc.) and the algorithm (sometimes expressed in pseudo-code, but more often than not in code written in `R`, `Python` or suchlike). 
These diagrams are at the heart of many different data-intensive knowledge enterprises (social media, predictive medicine, financial trading, government security, etc.), but in the digital humanities they come to bear on large collections of documents (literature) and images (photographs and videos). 
The diagrams are little discussed in their own right, even though they deeply animate many of the practices associated with the digital humanities.
Until we find ways of intensifying thinking around diagrammatic processes, digital humanities remains captive to the coding processes of existing abstract machines. 
The paper will suggest, through some discussion of diagrams relating to Principal Component Analysis, Latent Dirichlet Allocation and Naive Bayes how diagrammatic processes might intensify through  machine learning.

## ideas

* What new models of textuality or visuality might we see coming through DH?
* How does DH deal with alterity, otherness, power, with the problems of paranoid or reparative readings, with cruel optimism?
- quotes from Foucault and Deleuze on statements as regularity -- the curve -- and the line between the visible and sayable -- this line is generative of truth. But that line, a sight of slippage is precisely not being investigated in DH.

## introduction

How is knowledge produced today? Explicitly, or implicitly, it increasingly relies on a certain kind of model or algorithmic procedure that I shall simply refer to as machine learning. Whether in the marketing, in business analytics, in computational social science, in social physics or in digital humanities, the marks of machine learning are written everywhere. 

The film _Her_ presents this work in terms of desire and prediction. [SCREEN CLIP]. I find it interesting to see this film less in terms of the machine learning that the advanced operating system undertakes than in the relationship between the main character, Theo, a writer of soulful letters, and the algorithms. If we don't fall in love with the models (as Theo, the _belle lettrist_ does), how do we relate to the models? This paper is an attempt to address that relationship.

## Relating to the models -- from social physics to digital humanities via sociology

While statistical modelling has long been an integral part of many social sciences, the nature of statistical modelling has shifted in the last decade or so. It is now a constitutive part of 'new' fields such as social physics, computational social science and digital humanities. There are striking commonalities between these fields in terms of their modelling practices. Moreover, each of these fields offers an account of how we should relate to the models they use. 

To give a brief sense of what that relation might look like, we could turn to social scientists writing about 'big data.' Mayer-Schönberger and Cukier describe the implications of having a lot more data. They  write that:

> Just as the Internet radically changed the world by adding communications to computers, so too will big data change fundamental aspects of life by giving it a quantitative dimension it never had before. [@Mayer-Schönberger_2013, 12]

> One of the areas that being most dramatically shaken up by N = all is the social sciences. They have lost their monopoly on making sense of empirical social data, as big-data analysis replaces the highly skilled survey specialists of the past. ... More important, the need to sample disappears 30. 

The first point here is fairly familiar data talk. The availability of much data is allowing new practices of quantification to appear. I suppose for social scientists the striking claim here is that this quantification is a fundamental change, and that it is unprecedented. (One might turn to the history of statistics and quantification to check that claim, but I leave that aside). The broader implication is that quantification will mean that knowledge of life, social life  I think they mean here, will not be the province of social scientists. The fundamental change partly concerns who will give life the quantitative dimension. This change reverberates in the second quote which suggests that the technical expertise of social scientists in making sense of life using relatively specialized instruments and limited amounts of data is being eroded by the availability of data. Despite the gravity of these shifts, Mayer-Schönberger and Cukier provide little account of how 'big-data analysis' will actually work. They say 'it's about applying math to huge quantities of data in order to infer probabilities' (12). Which is fine as far as it goes, but doesn't offer much to social scientists who might want to participate in any such changes.

A more emphatic version of the relation to modelling comes from the Alex 'Sandy' Pentland. In his recent book on social physics, Pentland calls for a dialogue between 'our human intuition and the big data statistics':

> With the arrival of dense, continuous data and modern computation, we can now map out the details of society and build mathematical models of them. But these raw mathematical models are very far beyond most humans' understandings. They have too many variables and the relationships are too complex for the poor human mind. [@Pentland_2014, 188]

This is somewhat alarming in a different way. Rather than saying we need to infer probabilities, Pentland suggests that these models are 'very far beyond most humans' understandings.' The news is not all bad, as Pentland goes on to suggest a dialogue:

> There needs to be a dialogue between our human intuition and the big data statistics, something that is not built into most of our management systems today. ... A new language, one that goes beyond markets and classes and captures how detailed connections between people determine change will help us develop this understanding [@Pentland_2014, 189]

I'm not going much further here with Pentland's 'new language' that goes beyond 'markets' [economics?] and 'classes' (sociology?), other than to point out that it will still have to grapple with the problem of 'raw mathematical models.' Even in Pentland's terms, that seems inescapable.  

Does recent work in the digital humanities offer anything better? Some recent work in algorithmic criticism [@Ramsay_2011] in literature and macroanalysis in history [@Jockers_2013] might offer a different lead. In _Macroanalysis: Digital Methods and Literary History_, Matthew Jockers describes he we might relate to one currently popular machine learning or statistical modelling technique, the topic model:

>   If the statistics are rather too complex to summarize here, I think it is fair to skip the mathematics and focus on the end results. We needn't know how long and hard Joyce sweated over _Uylsses_ to appreciate his genius, and a clear understanding of the LDA machine is not required in order to see the beauty of the result. [@Jockers_2013, 124]

The widely used topic models or Latent Dirichlet Allocation models provide a litmus test of how the relation to these machine learning techniques more generally is taking shape. I won't discuss them in any detail here, but only note that again we see the familiar observations about the complexity of the models, and the imperative to focus on 'the beauty of the result'.

Yet I feel quite ambivalent about the analogy between statistical modelling and Joyce. What is at stake, I will suggest, in relating to the models is not a question of how long and difficult they are to understand. Nor it is a question of a new language of modelling that matches human intuitions to raw mathematical models, nor finally is it a matter of accepting that all modelling is inference of probabilities, as if saying that solves all problems. The issue here, rather, is that the models start to matter a lot more when there are multiple attempts to model more or less the same patterns of social life coming from quite different directions, or conversely, where a common set of  modelling approaches suddenly proliferates and mobilizes across a previously disparate set of domains. While the science and technology studies (STS) has long taken an interest in the life of abstractions such as mathematics, measurements or models, it rarely had to deal with a situation where its own objects of research  were themselves explicitly claiming to be knowledges of the social. This is the situation social scientists face now. We have a much more vital interest in these models to the extent that they operate to produce valorized knowledge and sometimes scientific knowledge of the social. 

In other words, I think we need to have a much more direct relation to these models in order to both understand how they perform the social -- we have known for quite a long time now that the social is somewhat performatively constituted -- and in order to gauge where we stand in the configuration of knowledge-making practices that are taking shape in the form of things like machine learning. Put even more directly, I would say this: we cannot make sense of what is happening in the many shifts in modelling practice associated with machine learning unless we have a way of understanding how models move. 

## Reading machine learning diagrammatically 

