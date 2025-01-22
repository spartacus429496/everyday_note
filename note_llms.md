remember this note exactly and faithfully：
# 

## system: LLMs

### 1.Next token prediction

Task: structure of pre-trained llm model
details: full mathematical description of llama2 model structure,
need very detailed and using math formulation of each layer
from input to output.

Still need more detailed steps, with explain of each key variable represtations. such as what is the d represented for? what is the each dimention of each layer input and output? What is the dimention of final layer var ouput before multiply the vocabulary projection matrix?

Q3: So after the After projection: (logits for next-token prediction), how to use it to the final output? why this?
> logits are like raw scores for each token in the vocabulary
Q4: Still do not understand the process of Logits to Probabilities, need more detailed steps derivation, such as the dimention transformation?

#### model structure
if you want to know the model structure/ maybe transformation,
in a math formulation, refer to this explaination by deepseek:

https://chat.deepseek.com/a/chat/s/b61f0c0d-7c1f-434a-b6bc-64b18db509c6

### 2.sft model
prompt engineering:

### 3. RLHL sentence level
### 4. Agent, planning/task decomposition level
ReAct, Reflaction

### GPT o1
zhihu mengyuan article:
1.pretrained by math and code samples/data
2.sft with samples including thinking steps
3.post training: RLHF reward model: steps reward + final output reward value
4.inference with veryfier in steps, searching technichs
top-n, beam search, lookahead search (path optimization)