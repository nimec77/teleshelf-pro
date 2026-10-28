# TeleShelf Pro para Android TV

[English](../README.md) · [Русский](ru.md) · Português (Brasil) · [Español (Latinoamérica)](es-419.md)

Os vídeos dos canais que você segue no Telegram, organizados na TV:
prateleiras, retomada da reprodução, histórico e lista para assistir mais
tarde. Tudo pelo controle remoto. O TeleShelf usa a API do Telegram e é um
aplicativo independente e não oficial, sem vínculo ou endosso do Telegram.

**Favoritos** guarda vídeos para assistir novamente. Escolha **Adicionar aos favoritos** no menu de um vídeo, inclusive durante a reprodução, e abra Favoritos abaixo de Assistir mais tarde no painel lateral. Assistir ao vídeo ou limpar o histórico mantém o favorito; Assistir mais tarde continua sendo uma fila separada.

**Progresso de reprodução:** o vídeo é considerado assistido ao chegar a 90% da duração, mesmo se você sair antes do último quadro. Voltar para antes de 90% permite retomar desse ponto; a reprodução automática ainda espera o vídeo terminar.

**Formatos de vídeo não compatíveis:** quando a TV não consegue decodificar o formato de um vídeo, o player explica a limitação e oferece voltar ao início, sem um botão de tentar de novo que não resolveria o problema. Erros que podem ser temporários ainda permitem tentar novamente.

**Configurações:** controles e opções de idioma e teclado mais claros; confirmação da qualidade e do número de vídeos na reprodução automática; e uma janela para escolher o tamanho do cache com o controle deslizante. Cada seção lembra o foco e a rolagem. Ao restaurar vídeos ou canais ocultos, limpar o cache ou enviar diagnósticos, os erros ficam claros e é possível tentar novamente.

**Teclado da busca:** teclado compacto com inglês e mais um layout selecionado: russo, português do Brasil ou espanhol da América Latina. Acentos e Ё têm teclas próprias, e números e símbolos ficam em uma página separada. Em Configurações → Idioma → Idiomas do teclado, escolha Automático, somente inglês ou inglês com um dos três idiomas. A busca usa a mesma opção e mantém o foco ao digitar e navegar entre buscas recentes e resultados.

**Filtrar canais:** em Canais, abra o filtro acima da grade e digite parte do nome de um canal. Os resultados mudam enquanto você digita, com o mesmo teclado compacto e a mesma opção de idioma da busca. Concluir fecha o editor; limpar o filtro restaura a lista completa.

**Carregamento e foco:** a tela inicial mantém Continuar assistindo disponível e mostra blocos de carregamento enquanto os vídeos dos canais carregam. Se a lista de canais falhar, é possível tentar novamente. Os cartões escurecidos mantêm o contorno de foco.

**Confiabilidade e privacidade:** troca de conta com limpeza isolada e opção de tentar novamente; listas de canais e pesquisa continuam a carregar mesmo com resultados ocultos ou repetidos. Correções de reprodução, controles de fone, reações e Continuar assistindo do launcher. Menos metadados retidos e melhor proteção de backups e diagnósticos.

**[Baixar TeleShelf Pro 0.59.2 · compilação 82](https://github.com/nimec77/teleshelf-pro/releases/latest/download/teleshelf-pro.apk)** · **Código do Downloader: 6320340**

SHA-256 do APK:
```text
0b2ff716c046f7429561a862cbb5aaa946ae64f813371f7bb5a699d2ada2b1cc
```
[Disponibilidade das versões](https://github.com/nimec77/teleshelf-pro/releases) ·
[Teste, compra ou restauração](https://t.me/TeleShelfProBot?start=trial)

## Instalação e acesso

Você precisa de Android TV ou Google TV com Android 8.0 ou posterior,
processador ARM de 32 ou 64 bits, internet, controle remoto e Telegram no
celular. Dispositivos Fire TV baseados em Android podem aceitar o APK;
a compatibilidade ainda será verificada. Este APK não oferece suporte a
Vega OS, Apple TV ou x86.

### Baixar diretamente na TV

Baixe o APK oficial pelo link acima ou use o Downloader na TV.
Instale o aplicativo antes de iniciar o teste.

1. Instale **Downloader by AFTVnews** pela loja compatível com sua TV.
   Veja a [página oficial do Downloader](https://www.aftvnews.com/downloader/).
2. Abra o Downloader, digite **6320340** e carregue o endereço.
3. O arquivo **teleshelf-pro.apk** será baixado. Como alternativa, abra
   [Releases](https://github.com/nimec77/teleshelf-pro/releases) → **Assets** →
   **teleshelf-pro.apk**. ZIP/tar.gz de código-fonte não é um instalador.
4. Se solicitado, permita que o Downloader instale aplicativos. A opção pode
   se chamar **Instalar apps desconhecidos** ou **Fontes desconhecidas**;
   o nome e o local variam conforme a TV. Volte ao APK baixado.
5. Selecione **Instalar** e **Abrir**. Para atualizar, instale por cima do
   TeleShelf existente e mantenha os dados para preservar sessão e histórico.

O código **6320340** aponta para o endereço estável do APK no GitHub. Se o
encurtador estiver indisponível, digite o endereço completo no Downloader:

```text
https://github.com/nimec77/teleshelf-pro/releases/latest/download/teleshelf-pro.apk
```

O aplicativo e o processo de instalação foram testados com sucesso em uma TV
física com Android TV.

### Transferir de um celular Android

Se [LocalSend](https://localsend.org/download) estiver disponível na TV e
for utilizável (talvez com um mouse), instale-o no celular e na TV. Conecte ambos
à mesma rede local. No celular, baixe o APK em **Releases → Assets**, envie
o arquivo pelo LocalSend e aceite na TV. Abra o APK no LocalSend ou no gerenciador
de arquivos da TV, permita a instalação por esse app e selecione **Instalar**.
Também é possível salvar o [documento APK oficial no Telegram](https://t.me/teleshelf_pro/19).
O envio do celular à TV usando apenas o controle não foi verificado; pode exigir um mouse.
Usuários de iPhone devem baixar diretamente pelo Downloader na TV.

### Entrar e verificar o acesso

Abra o TeleShelf e escaneie o QR da TV pelo leitor de conexão de dispositivos
do Telegram no celular. Confirme a conexão; digite na TV a senha de verificação
em duas etapas do Telegram se solicitado. Depois, abra @TeleShelfProBot no
celular com a mesma conta e inicie o teste. Se necessário, selecione
**Verificar acesso** na TV. Para acesso existente, envie `/restore` ao bot.

Baixou um ZIP? Escolha o APK em **Assets**. Instalação bloqueada? Verifique
a permissão do app que abre o APK. Para erro de compatibilidade, confira
Android 8.0+, ARM e o certificado oficial. Envie modelo da TV, versão do
Android e erro exato ao [suporte](https://t.me/TeleShelfSupportBot).

Para atualizar, instale o APK oficial por cima do aplicativo existente,
mantendo os dados para preservar o acesso, o histórico e as configurações.
Não há atualização automática. No primeiro acesso, escaneie o QR da TV com
o Telegram no celular e confirme a conexão do dispositivo.

## Teste de 14 dias e compra

Instale o aplicativo antes de iniciar o teste. No celular, abra
[@TeleShelfProBot](https://t.me/TeleShelfProBot?start=trial) com a mesma conta
do Telegram usada na TV. O prazo começa **somente ao tocar em Start free
trial** no bot. Instalar o APK ou abrir o bot não inicia o prazo. Cada conta
recebe um único teste de 14 dias, inclusive usuários anteriores. Outra TV,
uma reinstalação ou `/restore` mantém a data de término original.

Após o teste, navegar e reproduzir vídeos exige **uma compra única com
Estrelas do Telegram**. Não há assinatura nem modo gratuito permanente.
O bot mostra o preço padrão, **500 Estrelas em todos os países**, antes da confirmação.
Você pode comprar antes do teste. A compra pertence à sua conta do Telegram
e vale até uma revogação assinada, como após um reembolso. Leia `/terms`
no bot Pro antes de comprar; dúvidas de pagamento: `/paysupport` no mesmo bot.

Para restaurar, envie `/restore` ao bot Pro no celular e selecione
**Verificar acesso** na TV, se necessário. A restauração não reinicia o teste.
Suporte, contrato de uso e saída da conta continuam disponíveis com o
conteúdo bloqueado. A TV não envia mensagens ao bot nem gasta Estrelas.

## Arquivos oficiais e ajuda

As versões estão disponíveis no [GitHub Releases](https://github.com/nimec77/teleshelf-pro/releases)
e como documentos APK em [@teleshelf_pro](https://t.me/teleshelf_pro).
Compare o SHA-256 do arquivo com o anúncio da versão. A identificação do
certificado e os comandos estão no [guia principal](../README.md#updates-and-authenticity).

Os vídeos vêm diretamente da sua sessão do Telegram. O bot Pro mantém o id
da conta, as datas originais do teste e registros de compra para acesso e
restauração. Relatórios opcionais ficam desativados até seu consentimento.
[Política de privacidade](https://github.com/nimec77/teleshelf-pro/blob/main/PRIVACY.md)
(versão 1, em vigor desde 18 de outubro de 2026; em inglês). O contrato de uso
está disponível no aplicativo, em Suporte e Sobre.

Suporte do aplicativo: [@TeleShelfSupportBot](https://t.me/TeleShelfSupportBot).
Notícias: [@teleshelf_tv](https://t.me/teleshelf_tv). Idiomas da interface: English, Русский,
Português (Brasil) e Español (Latinoamérica).
