# Generating Drug-like Molecules from Gene Expression Signatures using Transformers

The chemical space of drug-discovery is very large and discrete. Screening through this space for molecules that satisfy biological and pharmacokinetic properties such as stability, solubility, efficacy, affinity and permeability poses a highly complex multiobjective optimization problem. Precisely, our Transformer model with modified encoder architecture is well suited for translating the information contained in high-throughput biological data into instances in the chemical space. 

<img src='/images/Transformer_Architecture.PNG' align="center" width="800" height="450" style="vertical-align:left;margin:0px 30px">

## Key Contributions:
* We show that attention-based sequential prediction performs better and converges faster, by well attending to previously predicted outputs and encoded gene expression signature.
* Moreover, the model automatically learns the structural and chemical characteristics during training, which is evident by visually inspecting the common scaffolds in the generated and the actual compounds.
* By incorporating biological information in the form of altered gene expression, we have outperformed other deep learning based molecular generators in terms of validity, uniqueness and metrics like Synthetic Accessibility score and Tanimoto similarity with the known compound.

Altogether, our method can not only help in accelerating the early stage of drug discovery but can also aid in drug repurposing. This work, done under the guidance of [Prof. Manikandan Narayanan](http://maninarayanan.com/index.html), is accepeted as a poster at 'ML for Computation Biology' track at [ISMB22](https://www.iscb.org/ismb2022).

## Dependencies
1. [Installing RDKit](https://www.rdkit.org/docs/GettingStartedInPython.html)
2. python 3.6+
3. tensorflow 2.1+
4. numba v0.52

## Using the code
A single Jupyter notebook `Modified_Transformer.ipynb`, downloads the dataset, evaluation toolkit (`RDKit`), builds, trains and evaluates the transformer model. It can be easily ported to run with public-cloud like GCP, AWS, etc. or `google-colab`.

## Additional resources
1. [Full-paper](https://drive.google.com/file/d/1vX8XD287tBKwLgkcCn0zyrv7pLX4lqhA/view?usp=sharing)
2. [Poster](https://iscb.junolive.co/ismb2022/library/search/ismb2022_poster_751)
