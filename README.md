# VoltBridgeADC ⚡
VoltBridgeADC é um projeto open source que combina eletrônica, programação e design de interface para a criação de um sistema de aquisição de sinais de tensão. Este projeto foi desenvolvido como uma solução simples e prática, ideal para quem deseja aprender ou construir uma base para seu Trabalho de Conclusão de Curso (TCC). O VoltBridgeADC foi projetado para ser adaptável, permitindo que outros desenvolvedores expandam suas funcionalidades ou ajustem o sistema conforme suas necessidades.

Este foi o meu primeiro projeto de PCB e também o meu primeiro trabalho utilizando microcontroladores da STMicroelectronics, uma experiência que me permitiu explorar desde a programação em baixo nível até o desenvolvimento de hardware.

## Sobre o Projeto 🚀
O VoltBridgeADC foi desenvolvido utilizando:

## Microcontrolador
O sistema é baseado no STM32L053R8T6, que oferece baixo consumo de energia e é ideal para aplicações de aquisição de sinais. Toda a programação do microcontrolador foi feita em C, utilizando o STM32CubeIDE, com foco na simplicidade e eficiência para gerenciar a comunicação e a leitura de tensões.

## Interface com o Usuário 💻
A interface foi implementada no LabVIEW, empregando o design pattern Produtor-Consumidor para separar o envio de comandos do processamento dos dados recebidos. O produtor envia comandos de "Start", "Pause" e "Stop", enquanto o consumidor gerencia a comunicação com o microcontrolador e apresenta as leituras de tensão. Apesar de ser simples, a interface é funcional e intuitiva, oferecendo recursos como:

- Seleção da porta USB do microcontrolador.
- Controle da comunicação com botões dedicados.
- Visualização em tempo real da tensão lida.
- Este foi o meu primeiro projeto no LabVIEW, e ele foi uma oportunidade de explorar a integração entre software e hardware.

## Desenvolvimento de PCB 🛠️
A placa do VoltBridgeADC foi projetada no KiCad, com atenção aos detalhes:

- Material: FR-4, garantindo durabilidade e resistência térmica.
- Acabamento: HASL, para melhorar a soldabilidade e reduzir custos.
- Organização lógica dos componentes para facilitar o roteamento.
- Trilhas com ângulos de 45°, priorizando integridade elétrica e redução de ruídos.
- Uso de furos para fixação mecânica, que também servem como pontos de aterramento (GND).
- Dimensões compactas: 68 mm x 99 mm, com bordas arredondadas para um design refinado.
- Os arquivos Gerber para a fabricação da PCB estão disponíveis no repositório, permitindo que qualquer pessoa possa produzir sua própria placa com facilidade.

## Sugestões para Melhorias ✨
Este projeto foi projetado para ser um ponto de partida, e há diversas possibilidades de melhorias:

- Substituição do Microcontrolador: Desenvolvedores podem optar pelo Arduino ou outros microcontroladores mais acessíveis, ajustando o código e o circuito para compatibilidade.
- Melhorias na Interface de Usuário: A interface em LabVIEW pode ser substituída ou aprimorada, utilizando outras linguagens de programação, como Python ou C#, para maior flexibilidade e recursos adicionais.
- Atualização da PCB: Melhorias no layout da placa, otimização do circuito e inclusão de novos recursos podem ser feitas.
- Aprimoramento do Código em C: Refatoração e adição de funcionalidades ao código do microcontrolador para torná-lo mais robusto e versátil.
- Substituição da comunicação serial UART por Bluetooth ou Wi-Fi: Implementar comunicação via Bluetooth ou Wi-Fi pode modernizar o projeto, facilitando a transmissão de dados do microcontrolador para a interface de usuário. Isso também permitiria o acompanhamento da tensão em tempo real diretamente pelo celular do usuário, ao invés de somente pelo PC, oferecendo mais praticidade e conectividade ao sistema.

## Licença 🆓
O VoltBridgeADC é um projeto open source, desenvolvido com o objetivo de compartilhar conhecimento e auxiliar outros entusiastas e estudantes. Sinta-se à vontade para usá-lo em seus próprios projetos ou como base para o seu TCC. Contribuições e melhorias são sempre bem-vindas!

Acesse o projeto, explore os arquivos disponíveis, e contribua com sugestões ou adaptações! 📈
