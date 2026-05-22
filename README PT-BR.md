# Otimização Estrutural de Suporte de Motor Aeroespacial

![Status](https://img.shields.io/badge/Status-Concluído-success)
![CAD](https://img.shields.io/badge/CAD-CATIA_V5-blue)
![CAE](https://img.shields.io/badge/FEA-ANSYS_Workbench-orange)
![Doc](https://img.shields.io/badge/Relatório-LaTeX-008080)

## 🚀 Visão Geral
Este repositório apresenta a engenharia estrutural, a modelagem paramétrica e a Análise por Elementos Finitos (FEA) de um suporte de motor para um foguete de sondagem, projetado para abrigar o motor de propelente sólido **AeroTech M1939W** (98 mm de diâmetro).

Em vez de apresentar apenas a peça final, este projeto documenta uma **jornada de engenharia iterativa**. O objetivo foi encontrar o equilíbrio perfeito entre a redução agressiva de massa e a estabilidade estrutural dinâmica sob severas cargas de lançamento (6750 N).

## 🔄 A Evolução do Design
O processo de engenharia passou por três fases críticas, cada uma analisada utilizando o ANSYS Static Structural:

1. **Iteração 1 (Tubo Sólido e Treliças):** Altamente conservadora. Ótima distribuição de tensão, mas mais pesada que o necessário.
2. **Iteração 2 (Esqueleto de Treliça Aberto):** Máxima redução de massa. Visualmente impressionante e numericamente segura na análise estática, mas descartada devido ao alto risco de flambagem lateral e à falta de contenção contra vibrações para o invólucro do motor.
3. **O Produto Final (Tubo Fendido):** A solução ideal. Ao reintroduzir o tubo central, mas usinando fendas longitudinais, o design alcançou uma leveza incrível enquanto manteve a "espinha dorsal" necessária para evitar a flambagem e fixar o motor com segurança.

## 📊 Resumo do Produto Final
A iteração final prova que a otimização geométrica inteligente pode resultar em um componente estrutural validado e pronto para operação.

* **Massa Final:** 1.35 kg
* **Deformação Total Máxima:** 0.063 mm (Extremamente rígido)
* **Tensão de von Mises Máxima:** 94.31 MPa
* **Fator de Segurança (FoS):** ~2.96 (A meta de projeto era >1.5)

### 🗺️ Análise de Deformação e Tensão (Iteração Final)
![Gráfico de Deformação](<Media/Efficient support 2/deformation support 2.png>)

https://github.com/user-attachments/assets/1e13afab-eef4-4409-8c57-8878d705af8a

*(Gráfico de Deformação Total do design final de tubo fendido, demonstrando deslocamento quase nulo sob uma carga de compressão de 6750 N).*

## 📂 Estrutura do Repositório
* `/CAD_Models`: Arquivos de geometria nativos (.CATPart) e universais (.STEP).
* `/Simulations`: Configurações de projeto e relatórios do ANSYS Workbench.
* `/Media`: Gráficos de FEA em alta resolução.
* `/Report`: Relatório Técnico completo compilado em formato PDF.

## 📄 Mergulhe na Engenharia
Como a malha numérica se comportou? Quais foram as condições de contorno exatas, as propriedades do material e as decisões matemáticas por trás do fator de carga dinâmico? A metodologia completa e o detalhamento das três iterações estão documentados no relatório acadêmico.
