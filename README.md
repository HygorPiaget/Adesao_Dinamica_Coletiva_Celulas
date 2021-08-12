# Combinando experimentos e modelagem in silico para inferir o papel da adesão e proliferação na dinâmica coletiva de células


### Este é o repositório de todos os dados e códigos utilizados no artigo [Melo, HPM, Maia, FR, Nunes, AS, Reis, RL, Oliveira, JM, e Araújo, NA. "Combining experiments and in silico modeling to infer the role of adhesion and proliferation on the collective dynamics of cells." bioRxiv (2021)](https://www.biorxiv.org/content/10.1101/2021.03.29.437400v1.abstract)

## Se você usar qualquer dado ou código, considere citar o paper.

1. A pasta **\images** contém todas as imagens experimentais da proliferação de células GBM em um substrato plano. O nome do arquivo contém os pontos de tempo (2h, 4h, 6h, 8h, 12h e 24h) e o número da amostra;
1. O arquivo **Nucleus_Segmentation.ipynb** é um código Python que lê todas as imagens da pasta **\images** e encontra a localização dos núcleos das células;
2. O arquivo **Mol_Dynamics_Model.cpp** é um código C++ usado para simular o modelo descrito no [artigo](https://www.biorxiv.org/content/10.1101/2021.03.29.437400v1.abstract);
3. Para executar a simulação da Dinâmica Molecular, você primeiro precisa fornecer um conjunto de parâmetros usando o arquivo **data.txt**:
    - Primeira linha: taxa de proliferação <img src = "https://render.githubusercontent.com/render/math?math=\lambda">;
    - Segunda linha: intensidade de adesão <img src = "https://render.githubusercontent.com/render/math?math=\tau">;
    - Terceira linha: semente usada para o gerador de números aleatórios.
