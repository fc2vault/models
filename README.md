# models

The Vault scene model, one release per build: tag `vault-r<N>`, asset `vault-r<N>.zip` holding the
folder `vault-r<N>/` (Hugging Face format: config.json, model.safetensors, labels.json, MODEL.md).

Vault downloads the newest release from **Settings → Scene model**; vault-scene-tagger then finds
it on its own. You can also unzip it by hand into the tagger's `models/` folder or point
`--phar-model` at it.

The model is a fine-tune of P-HAR's TimeSformer (Apache-2.0). It is free for personal use with Vault
and vault-scene-tagger; see LICENSE.md in github.com/fc2vault/vault.
