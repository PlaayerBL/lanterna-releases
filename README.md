<!-- Equivalente ao LEIA-ME.txt (que vai dentro do zip): mudou um, mude o outro. O teste LeiaMeTests confere seções,
links e textos entre aspas. O workflow "Atualizar README" copia este arquivo para o lanterna-releases. -->

# LANTERNA — assistente de temporada para Torchlight: Infinite

## ⬇️ [Baixar o Lanterna (versão mais nova)](https://github.com/PlaayerBL/lanterna-releases/releases/latest)

Na página que abrir, desça até **Assets** e clique em **Lanterna-X.Y.Z.zip** (o número muda a cada versão). Depois
siga o passo a passo em [Instalar](#instalar).

## O que é

Um overlay que lê a tela do jogo e indica a melhor jogada nas mecânicas de temporada:

- **Mistville** (mapa, Mercador, Alchemy, escolhas, Deduction, Folklore)
- **Canvas** (onde pôr a missão, o baú, qual efeito escolher, passivas da Artistry)
- **Tartarus** (destino da manhã, Consume/Replace/End, qual preso devorar, Instigate ou Bestow na Interrogation Room,
  a cela do Sewer Ratway, a melhor carta na escolha de instrumento e o presente do Warden's Treasure; nos mapas, avisa quando
  o Tartarus está quase cheio, de 45/48, ou cheio)
- **Cubo** (na loja Blessings from Gods, as ofertas que compensam e quando dar Refresh)

Ele **só** lê a tela e desenha as indicações. Não clica, não aperta teclas, não mexe na memória do jogo e não envia
nenhuma informação para a internet. O único contato dele com a internet é para **receber** atualizações (do GitHub).

## Instalar

O pacote completo mais novo (`Lanterna-X.Y.Z.zip`) fica na página de versões:
https://github.com/PlaayerBL/lanterna-releases/releases/latest

1. Extraia o zip inteiro (botão direito > Extrair tudo…) numa pasta como Documentos.
   Não abra de dentro do .zip e não ponha em "Arquivos de Programas".
2. Abra o `Lanterna.exe`.
   - Se o Windows mostrar "O Windows protegeu o computador", clique em "Mais informações" e
     "Executar assim mesmo" (o programa não é assinado, por isso o aviso).
3. Na primeira vez aparece a **verificação do computador**: ela mostra o que o computador tem e, se faltar algo, como
   instalar (há um botão que abre a tela certa do Windows). O que pode faltar:
   - Windows 10 versão 2004 ou mais nova (ou Windows 11), 64 bits.
   - Media Feature Pack, só no Windows "N" (Configurações > Aplicativos > Recursos opcionais).
   - Reconhecimento de texto (OCR) do Windows: o inglês é o recomendado, mas o português (ou espanhol) também serve.
     Sem o inglês, a verificação avisa e tem um botão "Instalar agora" (o Windows pede permissão de administrador). Ou:
     Configurações > Hora e idioma > Idioma e região > Adicionar um idioma > English (United States). Não precisa trocar
     o idioma do Windows. Com uma atualização do Windows esperando reiniciar, a instalação falha (erro 0x800f0950): a
     verificação avisa para reiniciar e terminar as atualizações antes; enquanto isso, o Lanterna usa o que já tem.

   Não precisa instalar .NET nem mais nada: vem tudo na pasta.

## Usar

- O Lanterna fica como um ícone com a letra L na bandeja (perto do relógio).
- Botão direito no ícone > Mecânica: escolha Mistville, Canvas, Tartarus ou Cubo (Blessings from Gods). Só a escolhida roda.
- Botão direito no ícone > Leitura de texto (OCR): automático (inglês se tiver, senão português), inglês, português ou
  inglês + português (o que o inglês não ler, em português).
- Cubo: os preços são os que você digita em bandeja > "Preços do Cubo…" (sem o da Divinity Stone, nada é calculado; itens fora da lista são ignorados).
- **F8** (ou dois cliques no ícone) liga e desliga. O Torchlight roda como administrador, e o Windows esconde as teclas
  dele de programas comuns: para a F8 funcionar com o jogo aberto, abra o Lanterna como administrador
  (bandeja > "Reabrir como administrador", ou botão direito no atalho > Executar como administrador).
- Só quer gravar as suas jogadas, sem indicações? Marque "Só coletar dados" no ícone. Nada aparece na tela, e as
  jogadas continuam sendo gravadas. Desmarque quando quiser as indicações de volta.
- Mistville, primeira vez: abra a grade com o Lanterna ligado; ele se calibra sozinho e guarda.
- Recomendado: jogo em 1920x1080 (outras resoluções 16:9 funcionam).

## Mandar as suas jogadas (arquivo de decisões)

Botão direito no ícone > "Gerar arquivo de decisões (para enviar)". Ele cria um .zip na pasta "para-enviar" (a pasta
abre sozinha) com as suas jogadas, sem imagens da tela. Mande esse .zip para quem te passou o Lanterna. Vai junto: as
decisões e resultados das runs, o histórico, o relatório do computador e o seu apelido. Não vai: senhas, contas, nada
fora da pasta do Lanterna.

Se o Lanterna fechar sozinho, abra de novo e gere esse arquivo: vai junto o registro de erros, com o que o Windows anotou
da queda.

## Atualizar

O Lanterna procura versões novas sozinho, ao abrir e a cada hora (só baixa; não envia nada):

- Ao abrir, se houver versão nova, ele pergunta se quer atualizar.
- Durante o jogo, aparece "Lanterna X.Y.Z disponível" no canto de cima, à direita, por 30 segundos a cada 2 minutos (só
  com as indicações ligadas). Para não ver mais o aviso desta versão: botão direito no ícone > Atualizar > Dispensar o aviso
  na tela.
- Para atualizar a qualquer momento: botão direito no ícone > Atualizar > Pela internet.
- O Lanterna fecha, atualiza e pergunta se abre a versão nova na hora. Configurações, calibração, registros e o que ele
  aprendeu continuam. O programa só aceita atualizações assinadas pelo desenvolvedor.

Sem internet, ou se recebeu um "Lanterna-atualizacao-X.Y.Z.zip":

- Deixe o arquivo em Downloads ou na Área de Trabalho e abra o Lanterna: ele pergunta se quer atualizar. Ou: botão
  direito no ícone > Atualizar > A partir de arquivo… e escolha o zip.
- Versão 1.3.6 ou anterior: o menu é "Atualizar a partir de arquivo…".
- Sem o menu "Atualizar" (versão 1.0.0): feche o Lanterna (bandeja > Sair) e extraia o zip da atualização **por cima**
  da pasta do Lanterna, substituindo os arquivos.

## Mais opções (botão direito no ícone)

- **Modo transmissão**: o overlay aparece no Discord/OBS quando você compartilha a tela. Fora dele, as indicações nunca
  aparecem na live. Sempre começa desligado: ligue de novo a cada vez que quiser mostrar.
- **Pet Mistville Orphan**: marque o nível do pet para ele contar os refreshes grátis.
- **Recalibrar**: se as indicações saírem fora do lugar.
- **Verificar o computador**: mostra de novo a verificação.
- **Log do jogo**: o Lanterna acha sozinho o arquivo de log do Torchlight (Steam) e, com ele, só lê a tela quando um
  minijogo está aberto (gasta menos o computador). Se mostrar "não encontrado", use "Apontar pasta do jogo…" e escolha
  a pasta do Torchlight Infinite. Sem o log, tudo funciona do mesmo jeito, só pela tela.

Os dados ficam todos na pasta do Lanterna (`config.json`, registros, aprendizado). Para começar do zero, apague esses
arquivos com o programa fechado.

A pasta `registros` guarda as imagens das suas jogadas até 1 GB (`LimiteRegistrosBytes` no `config.json`). Passou
disso, o Lanterna apaga as imagens das runs mais antigas. As jogadas em si (o que vai no arquivo de decisões) ficam.
