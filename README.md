\# Projeto de Reconhecimento de Texto em Imagens (OCR) - Azure AI Vision



Este repositório foi desenvolvido como parte de um exercício prático voltado ao estudo e aplicação de Inteligência Artificial e Visão Computacional, utilizando ferramentas de OCR (Optical Character Recognition) integradas aos ecossistemas de nuvem.



\## 📋 Objetivo do Projeto

O objetivo principal deste laboratório é demonstrar a capacidade de extração automatizada de textos estruturados e não-estruturados a partir de arquivos visuais de diferentes complexidades: um gráfico técnico de análise de mercado e um documento diagramado de grade curricular acadêmica.



\## 📁 Estrutura do Repositório

\- \*\*📁 inputs/\*\*: Contém as imagens originais de entrada submetidas para análise.

\- \*\*📁 output/\*\*: Contém os arquivos de texto (.txt) gerados com as transcrições brutas e os metadados textuais extraídos.

\- \*\*📄 README.md\*\*: Documentação explicativa contendo o processo de desenvolvimento e insights de aprendizado.



\## 🛠️ Processo de Desenvolvimento



\### 1. Preparação e Configuração do Ambiente

\- Criação de uma conta na plataforma Microsoft Azure.

\- Criação e configuração de um Grupo de Recursos isolado chamado `LABAI-900`.

\- Provisionamento de um recurso unificado de IA do Azure (\*\*Azure AI Services\*\*), sob o nome de `LABVISIONAI900`, centralizado na região geográfica \*East US\*.

\- Validação e integração do recurso com os serviços visuais da suíte \*\*Azure Vision Studio\*\*.



\### 2. Análise de Imagens e Extração (OCR)

Foram utilizadas duas amostras de alta complexidade para testar os limites do algoritmo de reconhecimento:



\- \*\*Imagem 1 (Magic Quadrant):\*\* Um infográfico técnico que mistura textos horizontais, verticais e dispersos em quadrantes cartesianos. O algoritmo de detecção mapeou as posições das palavras-chave de performance, as marcas listadas (ex: \*Nutanix\*, \*Microsoft\*, \*Broadcom\*) e as anotações temporais de rodapé.

\- \*\*Imagem 2 (Grade Curricular):\*\* Um documento corporativo textual altamente diagramado, distribuído em blocos de colunas paralelas e variações de cores (Azul para disciplinas obrigatórias e Cinza/Preto para nomes de professores). A extração serializou corretamente os dados sequenciais em formato de listagem lógica.



\## 💡 Insights Obtidos e Possibilidades Práticas



Durante a realização do laboratório e a análise de comportamento do motor de visão computacional, os seguintes aprendizados foram consolidados:



1\. \*\*Separação Estrutural de Dados:\*\* Motores modernos de OCR não executam apenas uma leitura sequencial linear de cima para baixo. Eles conseguem contextualizar a proximidade de blocos estruturais de texto (como tabelas ou grades de colunas em grades curriculares), preservando o agrupamento lógico das ideias.

2\. \*\*Desafios Visuais em Elementos Gráficos:\*\* Em infográficos cartesianos complexos (como o quadrante da Gartner), a rotação de eixos ou textos escritos na vertical (ex: eixos de coordenadas "Ability to Execute") exige maior poder computacional de alinhamento por parte do modelo de IA para não misturar palavras de blocos distintos.

3\. \*\*Casos de Uso no Mundo Real:\*\* 

&#x20;  - \*\*Automação de Backoffice:\*\* Leitura em lote de notas fiscais, contratos digitais e PDFs digitalizados para preenchimento automático de sistemas ERP.

&#x20;  - \*\*Acessibilidade:\*\* Transcrição instantânea de livros e infográficos visuais para leitores de tela voltados a deficientes visuais.

&#x20;  - \*\*Análise de Concorrência e BI:\*\* Extração ágil de informações textuais contidas em relatórios industriais e imagens de mercado para conversão direta em dados tabulares para manipulação em bancos de dados.



