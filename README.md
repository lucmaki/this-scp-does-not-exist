# This SCP Does Not Exist (demo website [**here**](https://lucmaki.github.io/this-scp-does-not-exist/))

##TLDR
Fine-tuning GPT-3 for generating SCP articles.
Generating associated images through Stable Diffusion.
Building web-pages from results.

## Features
-**Tabular SCP Article Generation**: SCP articles are generated section by section, with a consistent format that is stored and managed through tables.
-**Decoupled Generation: Article sections are generated seperately. This allows retrying generations by article section, or human input for one section to guide the rest of the generation for other sections.
-**Image Generation**: image prompts are parsed from the article, then generated through a Stable Diffusion model.
-**HTML Building**: pages with the classical SCP article look can be generated from the tabular SCP data.
-**Bulk Features**: articles, images and htmls can be generated in bulk through custom classes.

##What is SCP?
The SCP Foundation is an online community who roleplays as a secret organization. They publish fictional top secret documents (often horror themed), describing the contaiment of supernatural creatures, objects or phenomenon. Thousands of such articles have been published, with very creative supernatural concepts and high quality writing.

##Why this project?
SCP's unique horror style and format makes for a unique challenge for creative text generation. It's large number of quality fiction makes for a good training set.

I wanted an AI for brainstorming new ideas... but an issue would be that it would give full SCP articles with no control. This is why I developed it in a way to generate articles sections by section. For example: the article title may be generated, or it may be provided by the user to let the AI generate an article around that idea. This modular approach gives high control.

I hoped to build a website from this, replicating the feeling you get exploring the SCP wiki: seeing a large list of articles with attention grabbing names, and getting inspiration for interesting supernatural concepts after clicking random ones.
