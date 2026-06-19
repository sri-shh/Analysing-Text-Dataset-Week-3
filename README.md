# Analysing-Text-Dataset-Week-3
TASK 103 (3 business questions answerable from this text data)

1. Does AI-generated content differ from human-written content in length and complexity?
2. Which topics are more commonly covered by AI vs human-written content?
3. Is there a difference in word usage between AI and human text?



TASK 106
1) Does AI-generated content differ from human-written content in length and complexity?
Insight: From the EDA, I found that AI-generated content and human-written content have some differences in length. When I checked the word count column for both labels, AI content seemed to have a more steady length across entries, while human content had more variation: some very short, some longer. So it looks like AI tends to write in a more "fixed pattern" kind of way compared to humans

2) Which topics are more commonly covered by AI vs human-written content?
Insight: For this question, I looked at the topic column split by label (AI vs human). Both AI and human content cover similar topics overall, but some topics show up more often in AI-generated content than human content. So it seems like AI content might be focused around certain common topics, while human content is a bit more spread out across different topics.


3) Is there a difference in word usage between AI and human text?
Insight: For this question, the word frequency results and word cloud showed that AI-generated content repeats some phrases more often, while human-written content used a wider variety of words. This makes sense because AI tends to generate text in a more templated way, while humans naturally use more varied language when writing.


TASK 107

Proposed task:
I propose building a classifier that can predict whether a piece of content is text or code. This would use the content column as input, and the type column (text/code) as the output we’re trying to predict.

Success metric:
I would use accuracy as the success metric here. Since text and code look very different from each other (code has things like brackets, indentation, keywords like "return", while normal text doesn't), this should be a relatively easy task for a model to get right on most examples. Because the classes are also balanced (around 10,000 text entries and 10,000 code entries), accuracy gives a fair and simple way to check how well the model is doing without needing anything more complex.


