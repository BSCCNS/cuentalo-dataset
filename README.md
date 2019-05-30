# cuentalo-dataset 

[![DOI](https://zenodo.org/badge/174005042.svg)](https://zenodo.org/badge/latestdoi/174005042)

Dataset used in [proyectocuentalo.org](http://proyectocuentalo.org/).

## Description

The dataset is contained in the CSV file [cuentalo-hand-labeled-dataset.csv](cuentalo-hand-labeled-dataset.csv).
It has the following columns:

- `id`: (integer) Tweet id.
- `WHO`: (integer between 1-5) See [who](#who).
- `WHAT-murder`: (`1` or blank) `1` if the tweet was tagged as **murder**. See [what](#what), **murder**.
- `WHAT-rape`: (`1` or blank) `1` if the tweet was tagged as **rape**. See [what](#what), **rape**.
- `WHAT-sexual_assault`: (`1` or blank) `1` if the tweet was tagged as **sexual assault**. See [what](#what), **sexual assault**.
- `WHAT-abuse`: (`1` or blank) `1` if the tweet was tagged as **abuse**. See [what](#what), **abuse**.
- `WHAT-harassment`: (`1` or blank) `1` if the tweet was tagged as **harassment**. See [what](#what), **harassment**.
- `WHAT-fear`: (`1` or blank) `1` if the tweet was tagged as **fear**. See [what](#what), **fear**.
- `WHAT-disgust/sadness/anger`: (`1` or blank) `1` if the tweet was tagged as **disgust/sadness/anger**. See [what](#what), **disgust/sadness/anger**.

The columns `WHO` and `WHAT-*` correspond to:

### who

(mutually exclusive choices: *1--5*) the writer of the tweet either:

1. tells something about himself/herself.
2. tells something about someone else.
3. tells something supporting the movement.
4. tells something not related to the movement.
5. tells something against the movement.

### what

- **murder**: (*yes=1/no*) the tweet describes a murder.
- **rape**: (*yes=1/no*) the tweet states a rape or attempted rape.
- **sexual assault**: (*yes=1/no*) the tweet describes a sexual assault (but not situations that belongs to the category **rape**).
- **abuse**: (*yes=1/no*) the tweet states abuse.
- **harassment**: (*yes=1/no*) the tweet discusses about a non-physical harassment situation.
- **fear**: (*yes=1/no*) the tweet explicitly describes fear.
- **disgust/sadness/anger**: (*yes=1/no*) the tweet explicitly describes disgust/sadness/anger, only if **who** is different than 4.

The detailed information about the dataset can be found in the [paper](#citing-the-paper).

## Citation

If you use this dataset in a scientific publicaction, we would appreciate citations to the [paper](#citing-the-paper) and the [dataset](#citing-the-dataset):

### Citing the Paper

> Maria Soledad Bucalo, Luz Calvo, Fernando Cucchietti, David Garcia Povedano, Artur Garcia-Sáez, Juan Felipe Gómez, Camilo Arcadio González, Guillermo Marin, Irene Meta, Patricio Reyes, Feliu Serra, and Diana Fernanda Vélez. 2019. [A Constellation of Horrors: Analysis and Visualization of the #Cuéntalo Movement.](https://doi.org/10.1145/3308560.3316459) In Companion Proceedings of The 2019 World Wide Web Conference (WWW '19), Ling Liu and Ryen White (Eds.). ACM, New York, NY, USA, 751-754. DOI: https://doi.org/10.1145/3308560.3316459

Bibtex entry:

```
@inproceedings{cuentalo-laweb_2019,
 author = {Maria Soledad Bucalo and Calvo, Luz and Cucchietti, Fernando and Garcia Povedano, David and Garcia-S\'{a}ez, Artur and Felipe G\'{o}mez, Juan and Arcadio Gonz\'{a}lez, Camilo and Marin, Guillermo and Meta, Irene and Reyes, Patricio and Serra, Feliu and Fernanda V{\'e}lez, Diana},
 title = {A Constellation of Horrors: Analysis and Visualization of the \#Cu{\'e}ntalo Movement},
 booktitle = {Companion Proceedings of The 2019 World Wide Web Conference},
 series = {WWW '19},
 year = {2019},
 isbn = {978-1-4503-6675-5},
 location = {San Francisco, USA},
 pages = {751--754},
 numpages = {4},
 url = {http://doi.acm.org/10.1145/3308560.3316459},
 doi = {10.1145/3308560.3316459},
 acmid = {3316459},
 publisher = {ACM},
 address = {New York, NY, USA},
 keywords = {machine learning, social networks, supervised learning, visualization},
} 

```

### Citing the Dataset

The [*all-versions*](http://help.zenodo.org/#versioning) reference:

> pareyesv. BSCCNS/cuentalo-dataset. Zenodo. http://doi.org/10.5281/zenodo.2585526

```
@misc{cuentalo-dataset_2019,
  author       = {pareyesv},
  title        = {BSCCNS/cuentalo-dataset},
  doi          = {10.5281/zenodo.2585526},
  url          = {https://doi.org/10.5281/zenodo.2585526}
}
```

## References

- [proyectocuentalo.org](http://proyectocuentalo.org)
- [Designing the visualization of #cuentalo](http://www.bsc.es/viz/corner/?p=223)
- [paper](#citing-the-paper)
