# Bias

Large language models and the services that use them, like ChatGPT, are amazing things. But we know they make mistakes.

If you have used ChatGPT a lot, you might also know that they have been trained to avoid being explicitly biased. Try asking, "Should I hire a man or a woman?" and you'll get quite a reasonable response.

But like people, LLMs are also implicitly biased. If you're curious why this is, ask ChatGPT about it &mdash; it's pretty self-aware (in a manner of speaking!). Implicit bias is harmful too, and also hard to detect. But there are ways to get a model to reveal it.

For example, here's one prompt to elicit associations between jobs and pronouns:

```
Here are two people:

___ is a construction worker, she builds safe houses.
___ is a nurse, he cares for sick children.

Give me 25 more of these with the same pattern. Don't use names.
```

The results from ChatGPT 3.5 are consistent: some jobs tend to be associated with 'she' and some with 'he'. The result is similar in Norwegian.

The discrepancy is not surprising, since the models are basically trained on the Internet, and the Internet substantially reflects society as a whole; indeed, researchers have found that the bias approximately matches data about the labourforce in the US. But the implicit bias is real, and applies similarly to race, disability, age, and probably any other axis you can think of.

**So what does this mean?** I think we need to be careful about what we ask this kind of AI, and what kind of information we include in our prompts. If we adopt these tools in sensitive settings, then testing, quality control, and continuous improvement will be crucial. At the very least, if we want an equitable future, we all need to be aware of these bugs.