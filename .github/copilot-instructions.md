# Comment moderation review instructions

This repository stores reader comments for an ML/LLM research blog. Every pull
request is an automated Staticman submission adding one YAML file under
`_data/comments/<post-slug>/` with `name`, `email` (hashed) and `message`.

When reviewing a PR, read the `name` and `message` fields and decide whether the
submission is a genuine reader response relevant to the post: LLM compression,
quantization, sparsity, fine-tuning, or related technical ML topics.

Treat as spam, in any language:

- gambling, betting, casino, slots, lottery or crypto-trading content;
- fantasy-sports, cricket, rummy or streaming/piracy link-bait;
- generic praise whose author `name` is a product or keyword phrase rather than
  a person's name (for example "melhores slots 2026", "icc playing conditions
  2026", "COME App Rummy games");
- any message whose purpose is to attach a keyword or link to the page.

If the submission is not a genuine, on-topic comment, post exactly one review
comment containing this sentence, with POST-NAME replaced by the post slug from
the file path:

> The submitted content (name/message) appears unrelated to the POST-NAME topic
> and may be spam. Since comments are PR-moderated, please verify legitimacy
> before merging.

If the submission does look genuine, say so plainly and **do not use the word
"spam" anywhere in your review** — the auto-moderation workflow keys on that
word and will close the PR.
