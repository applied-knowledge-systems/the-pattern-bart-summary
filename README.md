---
marp: true
---

# the-pattern-bert-summary
The extension of The Pattern NLP pipeline with T5 based summary
It have two parts:

-  tokenizer_gears_for_sum.py - Redis Gears part running tokenizer on Redis Gears cluster
-  summary_processor_t5.py - Model runner, can be deployed separately on high GPU instance
-  both communicate via Redis instance, IP address hardcoded in above change as required


# Another way to improve:
Capture keymiss event on article_id summary on RedisGears and add article into pipeline: tokenizer -> model.



