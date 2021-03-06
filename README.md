# Combinando experimentos e modelagem in silico para inferir o papel da adesão e proliferação na dinâmica coletiva de células


### Este é o repositório de todos os dados e códigos utilizados no artigo [Combining experiments and in silico modeling to infer the role of adhesion and proliferation on the collective dynamics of cells, H. P. M. Melo, F. R. Maia, A. S. Nunes, R. L. Reis, J. M. Oliveira, N. A. M. Araújo. Scientific Reports 11, 19894 (2021)](https://www.nature.com/articles/s41598-021-99390-x)

## Se você usar qualquer dado ou código, considere citar o artigo.

1. A pasta **\images** contém todas as imagens experimentais da proliferação de células GBM em um substrato plano. O nome do arquivo contém os pontos de tempo (2h, 4h, 6h, 8h, 12h e 24h) e o número da amostra;
1. O arquivo **Nucleus_Segmentation.ipynb** é um código Python que lê todas as imagens da pasta **\images** e encontra a localização dos núcleos das células;
2. O arquivo **Mol_Dynamics_Model.cpp** é um código C++ usado para simular o modelo descrito no [artigo](https://www.nature.com/articles/s41598-021-99390-x);
3. Para executar a simulação da Dinâmica Molecular, você primeiro precisa fornecer um conjunto de parâmetros usando o arquivo **data.txt**:
    - Primeira linha: taxa de proliferação <img src = "https://render.githubusercontent.com/render/math?math=\lambda">;
    - Segunda linha: intensidade de adesão <img src = "https://render.githubusercontent.com/render/math?math=\tau">;
    - Terceira linha: semente usada para o gerador de números aleatórios.
