# JutsuMachine

JutsuMachine é uma aplicação web experimental desenvolvida para estudar a integração entre Inteligência Artificial e desenvolvimento web. O projeto utiliza um modelo treinado com o Google Teachable Machine para reconhecer os seis selos de mão necessários para executar o jutsu Bola de Fogo (*Katon: Gōkakyū no Jutsu*), do anime Naruto.

O sistema utiliza a webcam do usuário para capturar imagens em tempo real, identificar os selos realizados e verificar se a sequência correta foi executada.

## Objetivo

O principal objetivo do projeto é aprender conceitos de:

* Machine Learning aplicado à visão computacional;
* Integração de modelos Teachable Machine em aplicações web;
* Manipulação de webcam com JavaScript;
* Desenvolvimento front-end com HTML, CSS e JavaScript;
* Processamento e validação de sequências de eventos.

## Funcionamento

1. O usuário concede acesso à webcam.
2. O modelo Teachable Machine analisa as imagens capturadas.
3. Cada selo reconhecido gera um identificador interno.
4. Os identificadores são armazenados em uma estrutura JSON.
5. O sistema compara a sequência realizada pelo usuário com a sequência correta do jutsu.
6. Caso a ordem esteja correta, o jutsu é considerado concluído e um efeito sonoro é reproduzido.

## Tecnologias Utilizadas

* HTML5
* CSS3
* JavaScript (ES6+)
* Google Teachable Machine
* TensorFlow.js
* API MediaDevices (Webcam)

## Estrutura do Projeto

```text
JutsuMachine/
│
├── index.html
├── css/
│   └── style.css
│
├── js/
│   └── script.js
│
├── model/
│   ├── model.json
│   ├── metadata.json
│   └── weights.bin
│
├── assets/
│   ├── images/
│   └── sounds/
│
└── README.md
```

## Como Executar

1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/JutsuMachine.git
```

2. Entre na pasta do projeto:

```bash
cd JutsuMachine
```

3. Execute um servidor local.

Exemplo utilizando a extensão **Live Server** do Visual Studio Code.

4. Abra a aplicação no navegador.

5. Permita o acesso à webcam quando solicitado.

## Modelo de Machine Learning

O modelo foi treinado no Google Teachable Machine para reconhecer os seis selos de mão utilizados na execução do jutsu.

Atualmente o modelo alcança aproximadamente **89% de precisão**, podendo ser aprimorado com a adição de novas imagens de treinamento e maior diversidade de amostras.

## Roadmap

* [x] Treinamento do modelo
* [x] Reconhecimento dos selos individuais
* [ ] Captura automática em intervalos de tempo
* [ ] Validação completa da sequência do jutsu
* [ ] Sistema de pontuação
* [ ] Efeitos visuais e sonoros
* [ ] Responsividade para dispositivos móveis
* [ ] Novos jutsus e sequências

## Aviso

Este projeto possui fins educacionais e de aprendizado. Naruto e seus elementos visuais pertencem aos seus respectivos detentores de direitos autorais.

## Autor

Desenvolvido por Gabriel S. Duarte como projeto de estudo sobre Machine Learning e Desenvolvimento Web.
