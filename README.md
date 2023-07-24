# Megalodon
Sail the Seas of Data and Dive into the Depths of Computation!  
![Megalodon](megaladon.jpeg)

## _Megalodon: The Orca is no match._

Welcome aboard, shipmates! Let Megalodon be your steadfast vessel on the uncharted ocean of Big Data and Machine Learning. With our rich datasets and detailed mathematical models, there's no computational storm we can't weather together! 

> "We didn't name it 'Megalodon' for nothing. It's big, it's powerful, and it's got a heck of a bite when it comes to data crunching!" - Captain Codebeard

## Navigation Chart

```python
Dataset Sample (Row by Row) [Input] --(Feeds into)--> [Model] --(Outputs)--> Dataset Sample (Row by Row)
```

# Deck Logs (Changelog)

- **v2.0.0 - The Leviathan Update** - We've surfaced some serious computational power in this one! Modular integration of HuggingFace and OpenAI models.
- **v1.5.0 - The Kraken Patch** - Tightened up the tentacles of the code. Fewer bugs will be slipping through!
- **v1.0.0 - Maiden Voyage** - Initial launch! The Megalodon sets sail!

# Shipwright's Guide (Installation)

Batten down the hatches and ready your terminal, it's time to summon the Megalodon:

```bash
git clone https://github.com/megalodon-ds/megalodon.git
cd megalodon
pip install -r requirements.txt
```

# Navigational Tools (Usage)

1. **Start your voyage with a good map.** (Load your dataset)

```python
from megalodon import Megalodon

# Using OpenAI model
megalodon = Megalodon(model_id="gpt-3", api_key="your-api-key", dataset="flax-sentence-embeddings/stackexchange_math_jsonl")

# Using Hugging Face model
megalodon = Megalodon(model_id="gpt2", dataset="flax-sentence-embeddings/stackexchange_math_jsonl")
```

2. **Set sail!** (Generate explanations)

```python
explanations = megalodon.run()
```

3. **Return to port.** (Save your results)

```python
megalodon.save_to_huggingface(explanations, 'hf_output_dir')
```

Please replace `"your-api-key"` with your actual OpenAI API key, and `'hf_output_dir'` with your desired output directory for the Hugging Face datasets.

# Lifeboats (Support)

If you find yourself overboard in a sea of confusion, don't panic! Shoot a flare to our issue tracker on Github, and our dedicated crew will row to your rescue. 

[Create New Issue](https://github.com/megalodon-ds/megalodon/issues/new)

# Crow's Nest (Future Plans)

1. **New Species Detection** - We're constantly exploring unknown waters to find and integrate new algorithms and data models into Megalodon. 
2. **Crew Training** - Comprehensive documentation and examples are on the horizon to help you get the most out of your voyage with Megalodon.

Thank you for choosing to sail with Megalodon. May fair winds and calm seas guide your data journey!

Happy Sailing!

The Megalodon Team



# Todo:

* Better prompt
* More seamless model handling, plug and play with any model from OpenAI or HuggingFace.
* Save to HuggingFace after each iteration is labeled
* Potentially use Parquet for optimized storage
* Add in polymorphic or shape shifting preprocessing logic
