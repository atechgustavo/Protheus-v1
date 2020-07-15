# Retornos

Cada API especializada envia suas requisições para o método **SyncMessage** do AtechESB, que representa um túnel para mensagem síncrona.
Em outras palavras, a requisição atravessa a [camada de registro](https://automatech.stoplight.io/docs/AtechESB) -- o que faz com que a comunicação fique registrada -- e chega até a [camada Protheus](https://automatech.stoplight.io/docs/AtechExecAuto).

As respostas voltam do Protheus para o AtechESB e são redirecionadas, sem alteração, para o cliente. Portanto, os retornos recebidos são os mesmos gerados pela [camada Protheus](https://automatech.stoplight.io/docs/AtechExecAuto).

Consulte os possíveis [retornos do AtechExecAuto](https://automatech.stoplight.io/docs/AtechExecAuto/docs/Retornos.md).