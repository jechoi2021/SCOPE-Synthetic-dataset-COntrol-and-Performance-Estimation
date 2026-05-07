

# Supplementary Materials

TODO:
- add dataset
- add details to analysis pipeline

## Details to Reference Dataset
The following shows the age distribution of each reference dataset used.


<p align="center">
<img width="2042" height="339" alt="dataset scope overview 2" src="https://github.com/user-attachments/assets/c96f42e4-7fe5-4f77-b689-0b1709dc4ace" />
<img
  alt="dataset scope overview"
  src="https://github.com/user-attachments/assets/e63158a0-32f1-42cf-a721-2c3c2d90c64a"
  style="width:50%;"
/>
</p>

## Details to Synthetic Dataset

## Full Discussion and Limitation/Future Work Section

### Discussion
This study demonstrates that even a focus on a single feature type, like readability, can yield valuable insights into the characteristics of real and synthetic datasets. Our analysis highlights differences in alignment across datasets and the ability of synthetic texts to partially capture age-specific patterns. Extending this approach to additional features, more datasets, and complementary validation methods will strengthen the framework and provide a more comprehensive tool for evaluating synthetic data quality and alignment.

One notable observation is that the real predator dataset, $D_{pj}$, is indeed distinct from the other real-world datasets, whereas this might be due to the domain-differences. Yet, it still shows the potential to identify predator-specific patterns in advance. Additionally, despite using the same prompts, LLM-generated outputs displayed varying degrees of alignment with real-world datasets, highlighting differences in model behavior.

Finally, the SCOPE framework offers a promising approach for overcoming privacy constraints. In cases where real-world datasets cannot be shared due to privacy concerns, practitioners could provide derived features—such as readability scores—which can then be used by researchers to conduct meaningful analyses. This approach can increase the develoment of high-quality synthetic datasets, ultimately supporting the development of countermeasures against cybergrooming.

### Limitations and Future Work

While this study demonstrates the feasibility of the SCOPE framework for measuring alignment using readability features, it does not evaluate the framework on a downstream task. In particular, we did not assess whether higher alignment scores translate into improved performance in real-world applications. Rather than directly applying the framework to cybergrooming detection, a natural next step would be to use the most aligned synthetic datasets to train an age classification model and evaluate their performance on real-world data. If alignment is meaningful, classifiers trained on better-aligned datasets should demonstrate improved generalization. Such an experiment would provide a more conclusive validation of the SCOPE alignment framework.

However, as outlined earlier, the framework’s effectiveness depends not only on the alignment methodology itself but also on the selection of features and datasets. In this study, we focused exclusively on readability features and a limited set of datasets. A comprehensive validation of SCOPE therefore requires a broader range of linguistic features and a more diverse collection of real and synthetic datasets to ensure robustness and generalizability.

As this work primarily aims to introduce the SCOPE framework, our focus was on demonstrating that the proposed alignment measures reveal interpretable patterns and meaningful differences across datasets. The results indicate that readability-based alignment is capable of differentiating datasets and uncovering meaningful synthetic to real relationships. 

Future work will therefore extend this proof-of-concept by incorporating downstream evaluation, including training classifiers for age classification as a subtask of cybergrooming detection. This will allow us to directly examine whether alignment scores correspond to practical task performance and further validate the effectiveness of the SCOPE framework.

