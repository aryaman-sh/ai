# RNN (recurrent neural networks)

## ::Sequence Modelling::

**Sequence modelling problem** : prediciting the next word in a sentence, how many inputs should we have for predicting the next word in a feed forward network.
To counter some solutions can be:-

1. Only use last two words. However we may not get correct predicitons since it may depend on a word not in the last two.
2. Using entire sequece and as set of couts (bag od words), we input the count of words over a vocabulary however using just the counts we lose all the sequential history of the sentence.
3. Use a large fixed window. however in a feed forward if say a sentence always began with a fixed word and may not be shared in the full network so in the case where this parameter was to appear later will confuse the model.

### Sequence modelling: Design Criteria
1. Handle variable-length sequences
2. Track long-term dependencies
3. Maintain nformation about order
4. Share parameters across the sequence

Hence RNN are an approach to sequence modelling problems.

## ::what is RNN::
Standard neural networs go in one directions and not able to hold sequential information. Rnn have loops.

![alt text] (/images/2.png)
