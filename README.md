# This SCP Does Not Exist 
## (Click [**HERE**](https://lucmaki.github.io/this-scp-does-not-exist/) to check out the demo website)

![Cover image](/readme-img.png)

## TLDR
Fine-tuning GPT-3 for generating SCP articles.
Generating associated images through Stable Diffusion.
Building web-pages from results.

## Features
- **Tabular SCP Article Generation**: SCP articles are generated section by section, with a consistent format that is stored and managed through tables.
- **Decoupled Text Generation**: Article sections are generated seperately. This allows retrying generations by article section, or human input for one section to guide the rest of the generation for other sections.
- **Image Generation**: image prompts are parsed from the article, then generated through a Stable Diffusion model.
- **HTML Building**: pages with the classical SCP article look can be generated from the tabular SCP data.
- **Bulk Features**: articles, images and htmls can be generated in bulk through custom classes.

## What is SCP?
The [**SCP Wiki**](https://scp-wiki.wikidot.com/scp-series) is an online community who writes fiction about a secret organization: the SCP Foundation. They publish stories in the format of top secret documents (often horror themed), describing the containment of supernatural creatures, objects or phenomenon; also known as SCPs. They have published thousands of SCP articles; with a creative range of supernatural concepts and maintain high quality writing through strict moderation.

## Why this project?
SCP's unique horror style and clinical format makes for a unique challenge for creative text generation. Its vast quantity of quality fiction and creative concepts makes for a good training set.

I wanted an AI for brainstorming new ideas... but an issue would be that it would give full SCP articles with no control. This is why I developed it in a way to generate articles sections by section. For example: the article title may be generated, or it may be provided by the user to let the AI generate an article around that idea. This modular approach gives high control.

I hoped to build a website from this, replicating the feeling you get exploring the SCP wiki: seeing a large list of articles with attention grabbing names, and getting inspiration for interesting supernatural concepts after clicking random ones.
