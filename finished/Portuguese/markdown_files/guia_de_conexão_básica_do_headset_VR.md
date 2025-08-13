# Guia de Conexão Básica do Headset VR

## Propósito e Contexto
Este guia estabelece a base para todas as tarefas de gerenciamento de arquivos do headset VR. Você conectará seu Meta Quest 2, Quest 3 ou Quest 3s a um computador e acessará os arquivos da aplicação WildXR. Esta conexão é necessária antes de transferir arquivos de mídia, confirmar arquivos de configuração ou localConfiguration, ou solucionar problemas de aplicação.

⚠️ **Meta**: Hardware e software da Meta (incluindo MQDH) estão fora do controle da WPS. Atualizações da Meta podem causar mudanças inesperadas de funcionalidade em sistemas VR. A WPS monitora lançamentos da Meta para informar usuários sobre potenciais impactos e mudanças.

## Pré-requisitos
- Headset VR Meta Quest 2, Quest 3 ou Quest 3s
- Cabo USB-C *(recomendado)* ou cabo USB-C para USB-A
- Computador com File Explorer *(Windows)* ou Finder *(Mac)*
- Baterias AA para controles
- Aplicação WildXR instalada no headset
- Configurações de desenvolvedor habilitadas no headset

## Visão Geral Rápida (para usuários experientes)
1. Ligar headset e garantir que controles tenham baterias
2. Conectar cabo USB e sair do WildXR se executando
3. Habilitar conexão USB através de notificações Quest
4. Navegar para: `Quest` > `Internal shared storage` > `Android` > `data` > `com.wps.wildx` > `files`

## Passos Detalhados

### Configuração Inicial

1. **Instalar baterias dos controles**
   - Tanto Quest 2 quanto Quest 3 usam **baterias AA**
   - Garantir que ambos controles estão ligados

2. **Ligar seu headset**
   - **Quest 2**: Pressionar **botão de energia** no lado direito
   - **Quest 3 & Quest 3s**: Pressionar **botão de energia** no lado esquerdo

3. **Conectar cabo USB**
   - **Quest 2**: Porta USB localizada no lado esquerdo abaixo da têmpora
   - **Quest 3 & Quest 3s**: Porta USB localizada no lado esquerdo na têmpora
<div style="page-break-after: always;"></div>

4. **Identificar controle primário**
   - **Quest 2**: Controle direito tem **botão oval horizontal**
   - **Quest 3 & Quest 3s**: Controle direito tem **botão Meta logo**

### Saindo da Aplicação WildXR

*Se WildXR executar automaticamente, você deve sair para acessar arquivos.*

5. **Tentar abrir menu do sistema**
   - Colocar headset
   - Pressionar e soltar o **botão oval/Meta** no controle direito
   - Se tela **Quit/Resume** aparecer, pular para passo 8

6. **Forçar aparição do menu (se necessário)**
   - Pressionar **botão de energia** para adormecer headset *(tela escurece)*
   - Pressionar **botão de energia** novamente para acordar headset
   - Tentar **botão oval/Meta** novamente
   - Repetir até tela **Quit/Resume** aparecer

7. **Sair do WildXR**
   - Selecionar **"Quit"** usando gatilho do controle
   - *Você deve ver o ambiente home Quest*

### Habilitando Acesso do Computador

8. **Abrir notificações**
   - Mirar ponto de alvo no **ícone do sino** na barra de menu
   - Pressionar **gatilho do controle** *(sob dedo indicador)* para abrir notificações

9. **Habilitar conexão USB**
   - *Você precisará ter habilitado configurações de desenvolvedor no headset*
   - Encontrar notificação **"USB Detected"**
   - Mirar na notificação e pressionar **gatilho do controle**
   - *Isso permite que computador reconheça headset como drive externo*

### Acessando Arquivos no Computador

10. **Abrir navegador de arquivos**
    - **Windows**: Abrir **File Explorer**, clicar **"This PC"**
    - **Mac**: Abrir **Finder**

11. **Navegar para headset**
    - Clicar duas vezes **"Quest 2"**, **"Quest 3"**, ou **"Quest 3s"**
    - Clicar duas vezes **"Internal shared storage"**
<div style="page-break-after: always;"></div>

12. **Navegar para arquivos WildXR**
    - Clicar duas vezes **"Android"**
    - Clicar duas vezes **"data"**
    - Clicar duas vezes **"com.wps.wildx"**
    - Clicar duas vezes **"files"**

*Você agora tem acesso aos arquivos e pastas WildXR.*

## Entendendo arquivos e pastas WildXR

**pasta downloads**
- Contém todos os vídeos baixados para a aplicação WildXR
- Arquivos nomeados usando id único universal de 36 caracteres (UUID)
- Todos em formato MP4
- *Esta pasta é onde arquivos de vídeo **carregados lateralmente** serão colocados*

**pasta textures**
- Contém todas as imagens de miniatura baixadas para a aplicação WildXR
- Arquivos nomeados com UUID que corresponde ao UUID do vídeo
- Todos em formato PNG

**pasta temp**
- Contém arquivos temporários necessários pela aplicação WildXR
- Frequentemente conterá arquivos de vídeo que estão sendo baixados pela aplicação WildXR

**pasta Unity**
- Arquivos Unity WildXR
- Nenhum acesso necessário pela maioria dos usuários

**arquivo localConfiguration.json**
- Configurações que são específicas do dispositivo (headset)
- Contém configurações de Device ID, Environment e OfflineMode

**arquivo configuration.json**
- Configurações que controlam a aparência da aplicação WildXR
- Se headset ou computador (dispositivo) estiver registrado através do Portal Web WildXR estas configurações são controladas remotamente
- Se headset ou computador (dispositivo) não estiver registrado através do Portal Web WildXR estas configurações são pré-configuradas pela aplicação WildXR

**metadataDatabase.json**
- Metadados necessários pela aplicação WildXR para funcionamento adequado
<div style="page-break-after: always;"></div>

**DownloadQueue.json**
- Informações para função de download de vídeo na aplicação WildXR
- Pode estar vazio ou ausente se nenhum vídeo estiver na fila para download

**Player.log e Player-prev.log**
- Arquivos de log registrando o comportamento mais recente e anterior da aplicação WildXR
- Importantes para diagnosticar problemas e podem ser solicitados pela equipe WPS para diagnóstico

**youtubeData.json**
- Dados usados para ordenar vídeos em galerias de miniaturas baseado em vários fatores

## Solução de Problemas

**Headset não aparece no navegador de arquivos:**
- Garantir que cabo USB está totalmente conectado
- Tentar uma porta USB diferente no computador
- Verificar que você habilitou conexão USB no passo 9
- Verificar que o cabo USB suporta transferência de dados, não apenas carregamento

**Não consegue sair do WildXR:**
- Remover headset brevemente, então colocar de volta
- Reiniciar headset *Pressionar botão de energia para adormecer headset e então pressionar novamente para acordar*
- Garantir que controles tenham energia de bateria suficiente

**Controles não respondem:**
- Verificar direção da instalação da bateria
- Tentar baterias AA frescas
- Garantir que controles estão pareados *(deve acontecer automaticamente quando headset inicia)*
- Reiniciar controles removendo e reinserindo baterias

**Notificação de conexão USB não aparece:**
- Desconectar e reconectar cabo USB
- Tentar porta USB diferente no computador
- Garantir que headset está totalmente ligado e não em modo sleep
- Verificar se modo desenvolvedor está habilitado nas configurações do headset
- *Você deve aceitar a notificação de conexão USB cada vez que o USB é conectado*

**Arquivos/pastas aparecem vazios ou inacessíveis:**
- Verificar que WildXR foi executado pelo menos uma vez no headset
- Verificar que o caminho correto está sendo seguido: `Android` > `data` > `com.wps.wildx` > `files`
- Garantir que permissões de depuração USB foram concedidas se solicitado
- Tentar atualizar a visualização do navegador de arquivos
<div style="page-break-after: always;"></div>

## Notas Importantes

⚠️ **Restrição de Edição de Arquivo**: Arquivos como `configuration.json` não podem ser editados diretamente no headset. Você deve:
1. Copiar arquivos para seu computador
2. Editá-los lá
3. Copiar os arquivos modificados de volta para sobrescrever originais
4. Arquivos podem ser abertos para verificar que mudanças foram aplicadas *(veja **Verificação de Transferência de Arquivo** abaixo)*

⚠️ **Recomendação de Backup**: Sempre criar uma cópia de backup de arquivos de configuração antes de editar.

⚠️ **Verificação de Edição de Arquivo**: Sempre verificar que arquivos editados foram transferidos com sucesso para o headset.

⚠️ **Recomendação de Transferência de Arquivo**: Ao carregar lateralmente arquivos de vídeo, verificar que a pasta **downloads** contém o número de vídeos que você tentou carregar lateralmente.

⚠️ **Requisitos do Cabo**: Garantir que seu cabo USB suporta transferência de dados. Alguns cabos são apenas de carregamento e não permitirão acesso a arquivos.

⚠️ **Pré-requisitos WildXR**: WildXR deve estar instalado e executado pelo menos uma vez antes que arquivos sejam acessíveis na estrutura de diretório esperada.