# Estufa Automatizada para Estudos de Potenciais Elétricos em Plantas


# 1.Descrição do Projeto

Este projeto visa a criação de uma estufa automatizada para estudar potenciais bioelétricos em plantas, como os Potenciais de Ação (PAs) e Potenciais de Variação (PVs), sob condições ambientais controladas.

A estufa foi desenvolvida a partir de materiais reciclados (como um rack de servidor) e equipada com sensores e atuadores controlados por microcontroladores Arduino. Ela possibilita o controle e a medição de variáveis ambientais como:

Luminosidade
Temperatura
Umidade do solo 
Além disso, um sistema de aquisição de dados monitora sinais bioelétricos em tempo real, possibilitando análises detalhadas das interações planta-ambiente.


# 2.Tecnologias Utilizadas

Hardware:
Arduino Uno R3 e Arduino Nano
Amplificador EI-1040

![image](https://github.com/user-attachments/assets/e11fc0ac-b948-4402-9d5e-4e8e0ffed1e6)


Sensores:
LDR para medição de luminosidade
DHT11 para umidade e temperatura
Higrômetro para umidade do solo

Atuadores:
Coolers para ventilação
Lâmpada incandescente para ajuste de luz
Bomba d’água para irrigação

![image](https://github.com/user-attachments/assets/cb835207-1656-4c52-b5fc-b3c4ead1beed)


Software:
C++ (Arduino IDE)
Python para processamento de dados
Flask para a criação de APIs
HTML/CSS/JavaScript para interface web

![image](https://github.com/user-attachments/assets/4c68402f-fe2b-4ea9-a7e3-f3971d7ff9b7)


# 4.Instalação e Configuração

Clone o repositório do projeto:

git clone https://github.com/seu-usuario/Projeto_Estufa.git
cd Projeto_Estufa

Carregue o Código Arduino

Acesse a pasta Estufa_arduino.
Abra o arquivo Estufa_arduino.ino no Arduino IDE.
Conecte o Arduino Uno ao computador via cabo USB.
Carregue o código para o microcontrolador.

Configuração do Flask

Certifique-se de que o Python está instalado (recomendado: versão 3.8 ou superior).
Instale as dependências necessárias usando pip:

pip install flask

Execute o servidor Flask com o arquivo app.py:

python app.py

O servidor será iniciado e ficará disponível em http://127.0.0.1:5000/.

Estrutura de Arquivos

1-Estufa_arduino/Estufa_arduino.ino: Código para controlar os sensores e atuadores via Arduino.

2-static/: Pasta que contém as imagens utilizadas no projeto (1.png a 8.png).

3-templates/index.html: Interface web para monitorar as variáveis ambientais em tempo real.

4-app.py: Backend Flask que gerencia as rotas e conecta o sistema com o Arduino.

5-README.md: Arquivo de documentação do projeto.

Acesse a Interface Web
Abra o navegador e acesse http://127.0.0.1:5000/ para visualizar a interface que exibe as variáveis da estufa em tempo real.

