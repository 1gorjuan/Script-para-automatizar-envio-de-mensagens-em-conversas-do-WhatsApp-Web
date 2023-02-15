# Script para automatizar envio de mensagens em conversas do WhatsApp Web

Este script é projetado para ser executado no console do navegador em uma página do WhatsApp Web. Ele permite que você envie automaticamente uma sequência de mensagens a uma conversa aberta no WhatsApp Web, a partir de um bloco de código inserido no script.

## Como usar
Abra uma conversa no WhatsApp Web.
Abra o console do navegador (geralmente com o atalho F12).
Cole o script na janela do console e pressione Enter.
Insira as mensagens que deseja enviar dentro da chamada sendScript(), na forma de um bloco de código, como no exemplo abaixo:

// o texto será colocado nessa linha, para adcionar mais mensagens só pular a linha

Pressione Enter para executar o script. As mensagens serão enviadas automaticamente na ordem em que aparecem no bloco de código.

## Como funciona
O script usa o método execCommand para inserir o texto em um elemento de edição de texto no WhatsApp Web. Em seguida, ele clica no botão "enviar" para enviar cada mensagem. O script inclui um atraso de 100ms entre o envio de cada mensagem para garantir que o WhatsApp Web não considere os envios em uma sequência rápida como spam. O script também inclui um atraso de 250ms entre cada mensagem, exceto a última, para evitar que o WhatsApp Web trave ou pare de responder durante a execução do script.


## Observações importantes
Esse script pode violar os termos de serviço do WhatsApp, portanto use por sua conta e risco.
Esse script foi testado na versão atual do WhatsApp Web em fevereiro de 2023 e pode não funcionar em versões futuras ou anteriores do WhatsApp Web.
Esse script requer que a conversa esteja aberta e que haja um elemento de edição de texto presente na página para que ele possa funcionar. Se essas condições não forem atendidas, o script lançará um erro.
