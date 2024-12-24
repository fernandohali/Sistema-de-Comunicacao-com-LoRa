# Sistema de Comunicação com LoRa

Este projeto implementa um sistema de comunicação bidirecional utilizando módulos LoRa (SX1280). O objetivo é possibilitar a troca de mensagens entre dois dispositivos, com foco em criptografia e eficiência na transmissão de dados.

## Funcionalidades

- Comunicação bidirecional entre dois módulos LoRa.
- Transmissão de mensagens com criptografia.
- Configuração otimizada para alcançar distâncias maiores com menor consumo de energia.
- Sistema escalável para incluir múltiplos dispositivos no futuro.

## Tecnologias Utilizadas

- **Módulos LoRa SX1280**: Para comunicação sem fio.
- **Microcontroladores (Arduino/ESP32)**: Para controle e envio/recebimento das mensagens.
- **C/C++**: Linguagem de programação para desenvolver o firmware.
- **Biblioteca LoRa**: Gerenciamento da comunicação LoRa.

## Requisitos

- Dois módulos LoRa SX1280.
- Dois microcontroladores compatíveis (como Arduino Uno, ESP32 ou similares).
- Software de desenvolvimento Arduino IDE ou PlatformIO.
- Fios e protoboard para conexões.

## Instalação

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/Sistema-de-Comunicacao-com-LoRa.git
   ```

2. Instale as dependências necessárias na IDE Arduino ou no PlatformIO:
   - Adicione a biblioteca LoRa na IDE.

3. Configure os pinos de conexão conforme o modelo de microcontrolador utilizado.

4. Faça o upload do código nos dois dispositivos.

## Como Funciona

1. Cada dispositivo será configurado com uma identificação única (ID).
2. O dispositivo transmissor envia uma mensagem utilizando LoRa.
3. O dispositivo receptor decodifica a mensagem e exibe no terminal serial.
4. A criptografia garante que a mensagem não possa ser interceptada e lida sem autorização.

## Estrutura do Projeto

```plaintext
Sistema-de-Comunicacao-com-LoRa/
├── src/
│   ├── transmitter.ino    # Código do transmissor
│   ├── receiver.ino       # Código do receptor
├── README.md              # Documentação do projeto
├── LICENSE                # Licença do projeto
```

## Contribuições

Contribuições são bem-vindas! Para contribuir:
1. Faça um fork do projeto.
2. Crie uma branch para sua feature ou correção de bug: `git checkout -b minha-feature`.
3. Faça o commit das mudanças: `git commit -m 'Minha nova feature'`.
4. Envie para o repositório remoto: `git push origin minha-feature`.
5. Abra um pull request.

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

## Autor

Desenvolvido por **Fernando Hali Santos Andrade**.

---

**Nota:** Este projeto é ideal para aplicações que demandam comunicação eficiente e segura, como em campos de batalha, monitoramento remoto, ou troca de mensagens em áreas sem cobertura de rede convencional.
