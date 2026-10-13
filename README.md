# Transformer Training 06 — Initialisation, Normalisation and µP

Whether the signal and the gradient survive many layers depends on the scale of the initial weights and on where the LayerNorms sit. Pre-LN against post-LN through depth and in training, RMSNorm, and the maximal update parameterisation that lets one learning rate serve every width.

**Live site:** https://brendanjameslynskey.github.io/Transformer_Training_06_Init_Norm_and_muP/

Initial weight scale; pre-LN vs post-LN through depth and in training; RMSNorm; why the learning rate does not transfer across width; the µP coordinate check and learning-rate transfer.

## Live, animated companion

This deck is the slide companion to [Training](https://transformer-training-explained.vercel.app/training), the second site of the Foundations track (after Decoder), where the Decoder's model trains in your browser:

- [Chapter 7: Initialisation, normalisation and µP](https://transformer-training-explained.vercel.app/training/07-init-norm-mup)

## Where the numbers come from

Every measured number on these slides comes from the site's [results.md](https://github.com/BrendanJamesLynskey/transformer-explainer/blob/main/results.md) (seeded NumPy reference runs; CI recomputes them), filled in at build time from its `results.json`. Numbers from papers are cited on the slide with a link. The model is tiny (5,376 parameters, one book, a CPU): its runs show mechanisms, not what happens at scale, and the slides say so where it matters. GPU runs of the site's Colab notebooks are pending; no GPU number appears here.

Part of the [Transformer Training sub-hub](https://github.com/BrendanJamesLynskey/LLM_Hub_Transformer_Training) &middot; [LLMs hub](https://github.com/BrendanJamesLynskey/LLMs)
