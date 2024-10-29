README - Sistema de Identificação de Peixes com Fala

Descrição

Este projeto é um Sistema de Identificação de Peixes utilizando Machine Learning com a biblioteca Teachable Machine do Google. A aplicação permite identificar diferentes espécies de peixes por meio de uma webcam e, em seguida, anuncia o nome do peixe identificado utilizando a API de Síntese de Fala do navegador.

O modelo é treinado usando o Teachable Machine para classificar diferentes tipos de peixes e é exportado para ser utilizado diretamente em um ambiente web.

Funcionalidades

	•	Reconhecimento de peixes em tempo real utilizando a webcam.
	•	Anúncio do peixe identificado em voz alta, garantindo uma experiência interativa.
	•	Interface amigável para visualização dos resultados.

Tecnologias Utilizadas

	•	HTML5: Estrutura da página.
	•	JavaScript: Lógica de identificação, manipulação do DOM e síntese de fala.
	•	Teachable Machine: Criação e exportação do modelo de reconhecimento.
	•	TensorFlow.js: Para inferência do modelo treinado diretamente no navegador.
	•	API de Síntese de Fala: Para pronunciar o nome do peixe identificado.

Como Funciona

	1.	A aplicação carrega um modelo treinado exportado do Teachable Machine.
	2.	A webcam é configurada e ativada para capturar imagens em tempo real.
	3.	As imagens capturadas são passadas para o modelo, que realiza a classificação do peixe identificado.
	4.	O peixe identificado com a maior probabilidade é mostrado na tela.
	5.	O nome do peixe é anunciado em voz alta, apenas se a identificação for bem-sucedida e diferente da última identificação.

Pré-requisitos

	•	Um modelo treinado utilizando a Teachable Machine e exportado no formato de TensorFlow.js.
	•	Arquivos model.json, metadata.json e weights.bin do modelo exportado.
	•	Um servidor local ou hospedagem que sirva esses arquivos corretamente.

Estrutura de Arquivos

├── index.html             # Página principal do projeto
├── model/                 # Pasta contendo os arquivos do modelo
│   ├── model.json         # Arquivo JSON contendo a definição do modelo
│   ├── metadata.json      # Arquivo JSON contendo os metadados do modelo
│   └── weights.bin        # Arquivo contendo os pesos do modelo

Como Utilizar

	1.	Treine seu modelo utilizando a ferramenta Teachable Machine.
	2.	Exporte o modelo como “TensorFlow.js” e baixe os arquivos.
	3.	Coloque os arquivos exportados na pasta do projeto (model/).
	4.	Configure um servidor local (como o Live Server do VSCode) para servir os arquivos.
	5.	Abra o index.html no navegador e clique em “Iniciar” para começar o reconhecimento.

Exemplo de Uso

	1.	O usuário abre o arquivo index.html no navegador.
	2.	Clica no botão “Iniciar” para ativar a webcam e carregar o modelo.
	3.	A aplicação exibe o nome do peixe identificado no campo de resultado.
	4.	O nome do peixe é pronunciado se for identificado com uma probabilidade suficientemente alta.

Melhorias Futuras

	•	Adicionar um sistema de ajuste de sensibilidade para diferentes níveis de confiança na identificação.
	•	Suporte a múltiplas línguas na pronúncia do nome dos peixes.
	•	Implementar um banco de dados para salvar os registros das identificações.

Contribuições

Contribuições são bem-vindas! Se você deseja melhorar o projeto, sinta-se à vontade para abrir um pull request ou enviar feedback.

Autor

Este projeto foi desenvolvido por Carminati como parte de um sistema interativo de reconhecimento de espécies de peixes.

