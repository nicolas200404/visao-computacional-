# visao-computacional-
Descrição do Projeto
1. Acesse o Teachable Machine: Vá para o site do Teachable Machine.

2. Crie um Novo Projeto: Clique em "Get Started" ou "Novo Projeto". Escolha o tipo de projeto que melhor se adapta à sua tarefa de classificação de objetos (geralmente "Image Project").

3. Colete seus Dados:

4. Crie Classes: Defina as classes de objetos que você deseja que o modelo aprenda a identificar (por exemplo, "Cachorro", "Gato", "Pássaro").
Adicione Amostras: Para cada classe, colete e carregue várias imagens representativas desses objetos. Quanto mais diversificadas forem as imagens dentro de cada classe (diferentes ângulos, iluminação, tamanhos, etc.), melhor será o desempenho do seu modelo. Você pode fazer upload de arquivos do seu computador ou usar a webcam para capturar imagens.
Treine o Modelo:

5. Clique no botão "Train Your Model".
O Teachable Machine processará as imagens e treinará um modelo de aprendizado de máquina (geralmente uma rede neural) para distinguir entre as classes que você definiu.
Acompanhe o progresso do treinamento. Você poderá ver métricas como a "perda" (loss) diminuindo e a "acurácia" (accuracy) aumentando durante o treinamento.
Visualize e Teste:

6. Após o treinamento, você poderá testar o modelo diretamente na interface do Teachable Machine. Faça upload de novas imagens ou use sua webcam para ver como o modelo as classifica.
Observe a confiança (confidence score) que o modelo atribui a cada classe.
Exporte o Modelo:

7. Clique no botão "Export Model".
Escolha o formato "TensorFlow Lite" (geralmente recomendado para integração em dispositivos e outros ambientes) ou "TensorFlow.js" (para uso em navegadores).
Selecione a opção "Keras" se você deseja obter o modelo em formato H5 para usar com a biblioteca Keras/TensorFlow em Python.
8. Clique em "Download my model". Você geralmente receberá um arquivo ZIP contendo o modelo (model.tflite ou keras_model.h5) e um arquivo de metadados (labels.txt).
Parte 2: Verificar a Acurácia no Código Python

Agora, vamos ao código Python para carregar o modelo treinado e verificar sua acurácia. Para fazer isso de forma precisa, você precisará de um conjunto de dados separado que o modelo nunca viu durante o treinamento. Este conjunto de dados é chamado de conjunto de teste.

Instruções de Instalação 

Python: Certifique-se de ter o Python instalado no seu computador. Recomenda-se usar a versão 3.x. Você pode verificar se o Python está instalado abrindo um terminal ou prompt de comando e digitando:

Instruções de Uso
Treinamento no Teachable Machine:

Acessar o site e criar um projeto de imagem.
Definir as classes dos objetos que você quer identificar.
Coletar e fornecer diversas imagens de exemplo para cada classe.
Treinar o modelo.
Testar o modelo na interface web.
Exportar o modelo, preferencialmente no formato TensorFlow Lite (.tflite) e baixar o arquivo de rótulos (labels.txt).
Verificação da Acurácia em Python:

Instalar as bibliotecas: tensorflow, numpy e Pillow (pip install tensorflow numpy Pillow).
Editar o script Python:
Fornecer os caminhos corretos para o arquivo .tflite e labels.txt.
Se quiser avaliar a acurácia, organizar imagens de teste em uma pasta e atualizar o dicionário ground_truth com os nomes dos arquivos e suas classes verdadeiras.
Executar o script Python: python evaluate_model.py (ou python3).
Interpretar os resultados: O script mostrará as classificações para imagens individuais (se essa parte for usada) ou a acurácia geral do modelo no conjunto de avaliação, indicando a porcentagem de previsões corretas.

Creditos 
Processado no laboratorio da Ufopa
