## Writing style transfer Proposal (Follow Gray's Criteria)

Same as recently very hot topic **neural style transfer,** I come up with an idea that can we transfer the **writing style** of text. Every writer have their whole writing style, just like every artist have their own style. 

Sometime, we can see some guy write a same meaning sentence to different writing style to make fun, like write to Bible style.

Take a another example from Wikipedia **[Writing Style](https://www.wikiwand.com/en/Writing_style#/CITEREFStrunkWhite1979),**  

> "[These are the times that try men’s souls.](https://www.wikiwand.com/en/The_American_Crisis)" by [Thomas Paine](https://www.wikiwand.com/en/Thomas_Paine). Write it in different ways.
>
> Times like these try men’s souls.
>
> How trying it is to live in these times!
>
> These are trying times for men’s souls.
>
> Soulwise, these are trying times.



### Have Clear Benefit

This topic have clear benefit to many areas, such as News Writing, Translation, and writing assistant.

We know for some kinds of articles, they have their own writing styles. Sometimes it is even very strict rules for these styles, like news and law.  Or more recently, we-media. We can see some we-media they have their onw style to attract people, even it is not a good writing style.

So can we use writing style transfer to transfer the plain text we write to various writing style. Like photo filter in applications, can we make a text filter to transfer our text to other style.

### Be simple to state

This is very clear.

I will claim like "Transfer a particular piece of words from one writing style to other writing style."

I think this is easy to understand.

### Have no obvious solution

Yes, even it is very hard to find article about this topic.

### Have criterion where progress and solutions are testable, and it is possible to break the larger problem down into smaller steps

#### Evaluation

How to evaluate this transfer? I think same as mentioned in [1]. There is no ground ground truth for the problem of style transfer. Because both of them like create of art.

However from [1], we can also use the method they mentioned. Qualitative evaluation and quantitative evaluation.

**Qualitative Evaluation:** require participants to rank the results of different algorithms. However, this result will very depend on the participants. Especially, even more hard than photo style transfer, because reading words is harder than just read picture from intuition.

**Quantitative Evaluation:** Focus on the evaluation index of algorithm, like time complexity.

And from my view, because we can see every writing style as some kind of language model. So we can compare the model we get with the model we already trained on a lot of target style.

We can use, inspired by [2], we can use the way to measure domain similarity.

- Jenson-Shannon Divergence.
- Proxy *A* distance [3]
- or maybe perplexity

#### Break into smaller steps

From Wikipedia, we can divide the elements of writing style to three levels.

1. Choice of words.
2. Choice of sentence structure
3. Choice of paragraph structure

So for our system, we can also divide our task to three steps.

Transfer style in words level: Find research about lexicon, and align words, to get a word level transfer.

Transfer style in sentence level: 

Transfer style in paragraph level:



### Reference

[1] Jing, Yongcheng, et al. "Neural Style Transfer: A Review." *arXiv preprint arXiv:1705.04058* (2017) [Link](https://arxiv.org/abs/1705.04058). 

[2] Ruder, Sebastian, Parsa Ghaffari, and John G. Breslin. "Data Selection Strategies for Multi-Domain Sentiment Analysis." *arXiv preprint arXiv:1702.02426* (2017) [Link](https://arxiv.org/pdf/1702.02426).

[3] Ben-David, Shai, et al. "Analysis of representations for domain adaptation." *Advances in neural information processing systems* 19 (2007): 137 [Link](https://papers.nips.cc/paper/2983-analysis-of-representations-for-domain-adaptation.pdf).
