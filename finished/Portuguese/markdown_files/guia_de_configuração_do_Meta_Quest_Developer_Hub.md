# Guia de Configuração do Meta Quest Developer Hub

## Propósito e Contexto
Este guia estabelece o Meta Quest Developer Hub (MQDH) em seu computador, que serve como base para gerenciamento avançado de headset VR. MQDH permite instalar aplicações customizadas como WPS Auto Launch, gerenciar configurações de desenvolvedor e realizar solução de problemas avançada. Este é um processo de configuração única que cria o ambiente de desenvolvimento necessário para implantações WildXR.

⚠️ **Meta**: Hardware e software da Meta (incluindo MQDH) estão fora do controle da WPS. Atualizações da Meta podem causar mudanças inesperadas de funcionalidade em sistemas VR. A WPS monitora lançamentos da Meta para informar usuários sobre potenciais impactos e mudanças.

## Pré-requisitos
- Computador Windows ou Mac com acesso à internet
- Credenciais da conta Meta para sua configuração VR (incluindo acesso 2FA)
- Direitos administrativos para instalar software em seu computador
- Headset Meta Quest com modo Desenvolvedor habilitado
- Cabo USB compatível com seu headset Quest
- Headset e computador conectados à mesma rede WiFi

## Visão Geral Rápida (para usuários experientes)
1. Baixar MQDH do site de desenvolvedores Meta e instalar
2. Executar MQDH e autenticar com conta Meta
3. Completar configuração inicial e aceitar termos de desenvolvedor
4. Conectar headset e estabelecer autorização de depuração USB
5. Verificar funcionalidade completa com gerenciamento de headset conectado

## Passos Detalhados
*Apenas o sistema operacional Windows será coberto nos seguintes passos.*
*Uma versão Apple iOS do MQDH está disponível seguindo o link abaixo*

### Baixando e Instalando MQDH

1. **Navegar para Downloads de Desenvolvedor Meta**
   - Abrir navegador web e ir para o site de desenvolvedores Meta
   - **Windows**: Visitar https://developers.meta.com/horizon/downloads/package/oculus-developer-hub-win/
   - **Mac**: Visitar https://developers.meta.com/horizon/downloads/package/oculus-developer-hub-mac/
<div style="page-break-after: always;"></div>

2. **Baixar pacote MQDH**
   - Clicar botão "Download" no canto superior direito
   - Aceitar termos de licença quando solicitado
   - Escolher local de download e clicar "Save"
   - Arquivo baixa como "Meta-Quest-Developer-Hub.zip"

3. **Extrair e instalar MQDH**
   - Navegar para local do arquivo zip baixado
   - Clicar com botão direito em "Meta-Quest-Developer-Hub.zip"
   - Selecionar "Extract All" e escolher destino (local padrão funciona bem)
   - Clicar "Extract" para descompactar arquivos
   - Abrir pasta extraída e localizar "Meta-Quest-Developer-Hub.exe"
   - Clicar duas vezes no executável para começar instalação

4. **Completar processo de instalação**
   - Seguir prompts do assistente de instalação
   - Aceitar local de instalação padrão a menos que requisitos específicos existam
   - Quando instalação terminar, marcar caixa de seleção "Run MQDH"
   - Clicar "Finish" para completar instalação e executar aplicação

### Autenticação Inicial MQDH

5. **Começar configuração MQDH**
   - Aplicação abre para tela de boas-vindas
   - Clicar "Continue" no canto inferior direito
   - Selecionar opção "Log in with a Meta account"
   - Sistema abre janela do navegador para autenticação

6. **Autenticar com conta Meta**
   - Navegador redireciona para página de login Meta
   - Escolher opção "Continue with email"
   - Inserir endereço de Email associado com sua configuração VR *(pode ser fornecido pela WPS)*
   - Clicar "Next" para prosseguir

7. **Completar autenticação de senha**
   - Selecionar "Enter password instead" *(mais fácil que código de email)*
   - Inserir sua senha da conta Meta *(pode ser fornecida pela WPS)*
   - Clicar "Log in" para autenticar
<div style="page-break-after: always;"></div>

8. **Lidar com verificação 2FA**
   - Sistema apresenta dropdown de método 2FA
   - Selecionar método especificado pela equipe WPS
   - Clicar "Next" para prosseguir
   - Inserir código de autenticação de 6 dígitos quando solicitado
   - Clicar "Next" para completar verificação 2FA

9. **Gerenciar persistência de login (opcional)**
   - Escolher se salvar credenciais de login neste computador
   - *Salvar credenciais armazena apenas informações de email e senha*
   - *Verificação 2FA ainda será necessária para futuras sessões de login*
   - *Considere implicações de segurança de credenciais salvas em computadores compartilhados*

### Completando Configuração MQDH

10. **Aceitar termos de desenvolvedor**
    - MQDH exibe tela Terms and Documents
    - Revisar termos do acordo de desenvolvedor
    - Clicar "Continue" para aceitar e prosseguir

11. **Lidar com aviso de caminho ADB (se aparecer)**
    - Sistema pode exibir aviso sobre múltiplos caminhos ADB
    - Este aviso é tipicamente seguro para dispensar
    - Clicar "Cancel" ou fechar aviso sem modificar configurações ADB
    - MQDH usará padrões apropriados para seu sistema

12. **Verificar instalação bem-sucedida**
    - Interface principal MQDH deve agora estar visível
    - Barra lateral esquerda mostra ícones de gerenciamento de dispositivos
    - Barra de ferramentas superior exibe informações da conta
    - Aplicação está pronta para conexões de headset e gerenciamento de apps

### Conectando Seu Headset e Estabelecendo Depuração USB

13. **Estabelecer conexão física**
    - Ligar seu headset VR completamente
    - Conectar cabo USB entre headset e computador executando MQDH
    - Garantir que conexão do cabo esteja segura em ambas as extremidades
    - Headset deve permanecer ligado durante todo o processo de conexão
<div style="page-break-after: always;"></div>

14. **Verificar reconhecimento automático do dispositivo**
    - No MQDH, clicar no ícone do headset na barra lateral esquerda
    - Procurar por seu dispositivo listado como "Active" na seção Devices
    - Se dispositivo aparecer como Active, prosseguir diretamente para passo 18 para depuração USB
    - Se dispositivo não for mostrado ou aparecer como inativo, continuar com configuração do dispositivo

15. **Iniciar configuração de novo dispositivo (se necessário)**
    - Clicar menu dropdown no canto superior direito do MQDH
    - Selecionar "Set Up New Device" das opções do menu
    - Você pode precisar rolar para baixo para localizar esta opção
    - Clicar "Next" para começar assistente de configuração do dispositivo

16. **Configurar conexão do dispositivo**
    - Selecionar seu modelo específico de headset das opções disponíveis
    - MQDH escaneará por dispositivos compatíveis em sua rede
    - Escolher seu headset da lista "Choose Device" quando aparecer
    - Clicar "Next" para prosseguir com verificação da conta

17. **Completar configuração do dispositivo**
    - Confirmar que conta Meta correta está exibida na página Account
    - Clicar "Next" para prosseguir para configuração de rede
    - Selecionar rede WiFi apropriada para seu ambiente de implantação
    - Clicar "Next" para continuar com verificação do modo desenvolvedor
    - Ativar interruptor "Enable Developer Mode" se não estiver já ativo
    - Clicar "Next" para completar configuração inicial do dispositivo

18. **Autorizar acesso de depuração USB**
    - Colocar o headset VR para ver prompts do sistema
    - Procurar por caixa de diálogo "Allow USB debugging?"
    - Este diálogo autoriza seu computador a instalar aplicações e acessar funções do sistema
    - Você pode precisar olhar ao redor do ambiente virtual para localizar o diálogo

19. **Conceder permissões permanentes de depuração**
    - Clicar botão "Always allow from this computer" no diálogo
    - Este botão pode estar parcialmente obscurecido na parte inferior da janela do diálogo
    - A opção "Always allow" previne solicitações repetidas de autorização
    - Remover headset após confirmar a autorização
<div style="page-break-after: always;"></div>

20. **Completar verificação da configuração**
    - Retornar ao MQDH em seu computador
    - Clicar "Finish" se assistente de configuração do dispositivo ainda estiver aberto
    - Seu headset deve agora aparecer como "Active" na lista de dispositivos
    - Depuração USB está agora permanentemente autorizada para este par computador-headset

## Entendendo Componentes do Developer Hub

**Por que MQDH é Essencial:**
Meta Quest Developer Hub serve como ponte entre seu computador e headsets VR para tarefas de gerenciamento avançado. Enquanto operação básica do headset funciona através do app Meta padrão, MQDH desbloqueia capacidades de desenvolvedor que são essenciais para implantação de aplicações customizadas como WPS Auto Launch. Pense nisso como a diferença entre usar um smartphone como consumidor versus ter acesso de desenvolvedor para instalar apps customizados e modificar comportamento do sistema.

**Integração ADB:**
MQDH se integra com Android Debug Bridge (ADB), que é o protocolo de comunicação subjacente para gerenciar dispositivos baseados em Android. Headsets Meta Quest rodam em um sistema Android modificado, então ADB fornece a base técnica para instalar aplicações customizadas, acessar configurações do sistema e realizar solução de problemas avançada. O aviso ADB que você pode ver durante configuração se relaciona a garantir que MQDH use os caminhos de comunicação corretos.

**Requisitos de Conta:**
Sua conta Meta deve ter privilégios de desenvolvedor habilitados pela WPS antes que MQDH funcione adequadamente. Isso não é algo que você pode habilitar sozinho - requer coordenação com equipe WPS que gerencia as configurações da organização de desenvolvedores. Esta medida de segurança garante que apenas pessoal autorizado possa instalar aplicações customizadas em headsets de implantação WildXR.

## Solução de Problemas

**Download falha ou está corrompido:**
- Verificar conexão estável com internet durante todo o download
- Tentar baixar de navegador diferente ou modo incógnito
- Verificar espaço disponível em disco antes de baixar
- Contatar WPS se download falhar consistentemente

**Processo de instalação para ou falha:**
- Garantir privilégios administrativos no computador
- Desabilitar temporariamente antivírus durante instalação
- Verificar que sistema atende requisitos mínimos
- Reiniciar computador e tentar instalação novamente

**Autenticação falha repetidamente:**
- Verificar se endereço Gmail corresponde à conta de configuração VR
- Confirmar precisão da senha com equipe WPS
- Verificar que conta tem privilégios de desenvolvedor habilitados
- Garantir que códigos 2FA estão atuais (expiração de 30 segundos)

**MQDH não executa após instalação:**
- Verificar quarentena do Windows Defender ou antivírus
- Verificar que instalação foi completada com sucesso
- Tentar executar como administrador
- Reiniciar computador e tentar execução novamente

**Headset não reconhecido pelo MQDH:**
- Verificar que tanto computador quanto headset estão conectados à mesma rede WiFi
- Confirmar que sua conta Meta tem privilégios de desenvolvedor através da WPS
- Verificar que modo desenvolvedor está habilitado tanto no app Oculus do telefone quanto em headset Settings > Advanced > Developer
- Garantir que não existem atualizações pendentes do headset sob Settings > General > Software Update

**Autorização de depuração USB não aparece:**
- Verificar que conexões do cabo USB estão seguras em ambas as extremidades
- Verificar por atualizações pendentes do headset que podem prevenir autorização
- Procurar por atualizações pendentes do MQDH indicadas por banner no topo da aplicação
- Tentar desconectar e reconectar cabo USB após 30 segundos
- Reiniciar o headset completamente e tentar conexão novamente

**Dispositivo aparece conectado mas mostra como inativo:**
- Confirmar que depuração USB foi adequadamente autorizada com opção "Always allow"
- Verificar consistência da conta Meta entre MQDH e headset
- Verificar que modo desenvolvedor permanece habilitado nas configurações do headset
- Tentar remover e re-adicionar o dispositivo através do assistente de configuração MQDH

## Notas Importantes

⚠️ **Privilégios de Desenvolvedor Necessários**: Sua conta Meta deve ter acesso de desenvolvedor concedido pela WPS antes que MQDH funcione adequadamente para instalação de app customizado.

⚠️ **Consistência de Conta**: A conta Meta usada no MQDH deve corresponder exatamente à conta associada com seus headsets VR. Contas mistas impedirão reconhecimento adequado do dispositivo.

⚠️ **Vinculação de Headset**: MQDH requer que headsets tenham ADB habilitado para alguma funcionalidade. Se funcionalidade estiver faltando isso pode ser o problema.

⚠️ **Atualizações de Software**: MQDH está em um estado constante de desenvolvimento e como tal frequentemente requerirá uma atualização. Se possível, sempre atualize MQDH quando solicitado antes de completar outras tarefas no MQDH.
<div style="page-break-after: always;"></div>

## Passos de Verificação

Verificar que sua aplicação MQDH é capaz de reconhecer, conectar e gerenciar headsets VR sem passos de configuração adicionais.

**Verificação de funcionalidade completa:**
- MQDH executa sem erros e exibe informações da conta corretamente
- Pelo menos um headset aparece como "Active" na lista de dispositivos
- Autorização de depuração USB foi concedida e confirmada
- Ícones de gerenciamento de dispositivo são acessíveis e responsivos na barra lateral esquerda
- Você pode acessar o sistema de arquivos do headset e funcionalidades de gerenciamento de aplicações