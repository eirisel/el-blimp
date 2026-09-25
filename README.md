# el-blimp
el-BLiMP: A Minimal-Pair Benchmark for Targeted Grammatical Evaluation of Language Models in Modern Greek.

This thesis introduces el-BLiMP, a BLiMP-style benchmark of linguistic minimal
pairs for the Modern Greek language. The benchmark consists of 600 minimal
pairs organised into 6 grammatical phenomena, with 100 pairs for each phenomenon.
Each pair includes one well-formed and one ill-formed sentence that
differ minimally from each other. The sentences were generated using three
different methods: template-based generation, LLM-assisted generation, and
internet-extracted sentences. We use human acceptability judgements to assess
the grammaticality of a random sample of the sentences, with the help of 77
native Greek speakers who scored an overall agreement of 99.13%. We then
evaluate 11 pretrained models (8 autoregressive and 3 masked) on this benchmark,
and additionally use prompting to evaluate 4 instruction-tuned models
as a supplementary comparison. A separate model was trained from scratch
specifically on Greek data and evaluated on the benchmark at increasing data
sizes. The results indicate that pretraining and fine-tuning on Greek data matter
more for overall model performance than model size, while prompting appears
to be a less reliable method for evaluating a model’s grammatical knowledge
than log-probability-based scoring. Future work will expand the number of
phenomena and models evaluated.
