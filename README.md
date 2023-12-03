# CS4120-final-project
Automatically generate docstrings using small LLMs

# References

This code is largely based on the work of Microsoft's [CodeXGLUE](https://github.com/microsoft/CodeXGLUE/tree/main/Code-Text/code-to-text#readme):

```
@article{husain2019codesearchnet,
  title={Codesearchnet challenge: Evaluating the state of semantic code search},
  author={Husain, Hamel and Wu, Ho-Hsiang and Gazit, Tiferet and Allamanis, Miltiadis and Brockschmidt, Marc},
  journal={arXiv preprint arXiv:1909.09436},
  year={2019}
}
```

and HuggingFace's Seq2Seq example [here](https://huggingface.co/docs/evaluate/transformers_integrations#seq2seqtrainer) and [here](https://colab.research.google.com/github/elsanns/xai-nlp-notebooks/blob/master/fine_tune_bart_summarization_two_langs.ipynb). Our models use [google_blue](https://huggingface.co/spaces/evaluate-metric/google_bleu) scores to calculate performance as they offer better properties on smaller evaluations such as single-sentence (or single docstring) evaluations.