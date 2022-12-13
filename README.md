# transformers-for-drug-discovery

The chemical space of drug-discovery is very large and discrete. Screening through this space for molecules that satisfy biological and pharmacokinetic properties such as stability, solubility, efficacy, affinity and permeability poses a highly complex multiobjective optimization problem. Precisely, our Transformer model with modified encoder architecture is well suited for translating the information contained in high-throughput biological data into instances in the chemical space. 


## Key Contributions:
* We show that attention-based sequential prediction performs better and converges faster than by well attending to previously predicted outputs and encoded gene expression signature.
* Moreover, the model automatically learns the structural and chemical characteristics while being trained, which is evident by visually inspecting the common scaffolds in the generated and the actual compounds.
* By incorporating biological information in the form of altered gene expression, we have outperformed other deep learning based molecular generators in terms of validity, uniqueness and metrics like Synthetic Accessibility score and Tanimoto similarity with the known compound

Altogether, our method can not only help in accelerating the early stage of drug discovery but can also aid in drug repurposing.

Find [full-paper](https://drive.google.com/file/d/1vX8XD287tBKwLgkcCn0zyrv7pLX4lqhA/view?usp=sharing), [poster](https://iscb.junolive.co/ismb2022/library/search/ismb2022_poster_751).