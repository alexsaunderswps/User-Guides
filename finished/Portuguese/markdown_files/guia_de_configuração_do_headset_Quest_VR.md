# Guia de Configuração do Headset Quest VR

## Propósito e Contexto
Este guia fornece os passos necessários para configurar um headset Quest VR pela primeira vez. 
WPS pode ter criado algumas contas necessárias como parte de seu programa interno de parceria VR. Verificar com equipe WPS se você não tem certeza de quais contas sua organização precisa.
Criação de conta pela WPS é feita para facilitar operação VR suave e aumenta nossa capacidade de fornecer suporte técnico. 
Contas criadas sem a ajuda da equipe WPS não podem ser acessadas pela equipe WPS durante sessões de suporte técnico.

⚠️ **Meta**: Hardware e software da Meta (incluindo MQDH) estão fora do controle da WPS. Atualizações da Meta podem causar mudanças inesperadas de funcionalidade em sistemas VR. A WPS monitora lançamentos da Meta para informar usuários sobre potenciais impactos e mudanças.

## Pré-requisitos
- Uma conexão WiFi com a internet
- Credenciais de conta de email associadas com sua configuração VR *(podem ser fornecidas pela WPS)*
- Smartphone com capacidade de aplicativo 2FA
- Smartphone com aplicação Meta Horizon instalada
- Coordenação inicial com equipe WPS para primeiro login
- Headsets VR

## Visão Geral Rápida (para usuários experientes)
1. Conta Meta é criada para Organização *(pode ser fornecida pela WPS)*
2. Usuário faz login no app Meta Horizon do telefone
3. Modo desenvolvedor é habilitado para headset
4. Configurações recomendadas são aplicadas ao headset
5. WildXR e Auto Launch *(se desejado)* são instalados no headset
6. Headset é registrado com Website WildXR para provisionamento remoto
7. Vídeos são baixados ou carregados lateralmente para melhorar performance WildXR 

## Passos Detalhados

### Criação de Conta Meta

- *Se equipe WPS criou a Conta Meta usada para registrar headsets este passo pode estar completo*

1. **Navegar para Meta**
   - Abrir navegador web e ir para `meta.com`
<div style="page-break-after: always;"></div>

2. **Acessar login**
   - Clicar no **ícone da Conta** *(silhueta de pessoa)* no canto superior direito
   - Selecionar **"Sign up or log into a Meta account"**
   - Escolher **"Continue with email"**

3. **Inserir credenciais**
   - Clicar **Continue with Email**
   - Inserir endereço de Email associado com sua configuração VR
   - Clicar **"Next"**
   - Escolher **"Create new account"**
   - Inserir os detalhes solicitados conforme necessário para criação da conta
   - *Ao adicionar uma data de nascimento - WildXR é recomendado para idades 13+ - inserir uma data que satisfaça este requisito*
   - Escolher uma senha para sua conta *(Equipe WPS não terá acesso à sua senha)*
   - Proteger detalhes de sua conta (email e senha) para uso futuro
   - Clicar **"Next"**

4. **Gerenciar persistência de login (opcional)**
   - Escolher se salvar credenciais de login neste computador
   - *Salvar credenciais armazena apenas informações de email e senha*
   - *Considere implicações de segurança de credenciais salvas em computadores compartilhados*

5. **Verificar detalhes da conta** 
   - Revisar os detalhes da conta conforme inseridos
   - *Desmarcar a caixa de receber emails de marketing*
   - Clicar **"Create account"**

6. **Confirmar criação da conta**
   - Abrir a conta de email associada com sua conta Meta
   - Copiar o código de confirmação do email Meta recente
   - Inserir o código de confirmação na caixa apropriada.
   - Clicar **"Next"**

7. **Acessar painel da conta**
   - Você retornará à página principal `meta.com`
   - Clicar no **ícone da Conta** novamente para acessar funcionalidades da conta *(Ícone agora é um círculo com uma letra ou Logo)*
   - Selecionar **"Accounts Center"** para painel principal
<div style="page-break-after: always;"></div>

### Autenticação de Dois Fatores

- *Agora é um bom momento para configurar autorização de dois fatores pois será necessário mais tarde*
- *Se sua conta foi provisionada pela equipe WPS este passo pode ter sido completado*

8. **Navegar para configurações de segurança**
   - No **Accounts Center**, clicar **"Password and security"**
   - Selecionar **"Two-factor authentication"**
   - Escolher seu perfil
   - Selecionar **"Authentication app"** e continuar para passo 9 *(recomendado)*
   - Selecionar **"SMS or WhatsApp"** e continuar para passo 13

### 2FA via App de Autenticação

9. **Instalar app autenticador (Recomendado)**
   - Uma aplicação autenticadora permite gerenciamento por múltiplas pessoas
   - Baixar Google Authenticator (recomendado) ou Authy
   - Disponível tanto no iOS quanto Android
   - Múltipla equipe pode usar mesmo autenticador para conta compartilhada
   - Autenticação SMS ou WhatsApp está disponível para apenas um número de telefone

10. **Adicionar novo dispositivo**
    - Clicar botão **"Add"**
    - *Código QR e chave de configuração aparecerão*
    - *Mudar para seu telefone para próximos passos*

11. **Configurar app autenticador**
    - Abrir app autenticador no telefone
    - Adicionar nova conta *(ícone +)*
    - Escolher **"Scan QR code"** ou **"Enter setup key"**
    - Escanear código QR do site Meta

12. **Completar configuração**
    - Inserir nome descritivo para este dispositivo *(ex WPSVR GAuth ou GAuth do Alex)*
    - Inserir código de 6 dígitos do app autenticador
    - Clicar **"Done"**
    - *Dispositivo agora aparece na lista de dispositivos 2FA*
<div style="page-break-after: always;"></div>

### 2FA via SMS ou WhatsApp

- *Apenas um número de telefone é permitido para 2FA via SMS ou WhatsApp*
- *Isso restringirá a capacidade de solucionar certos problemas caso surjam*

13. **Adicionar Número de Telefone**
    - Mudar código do País se necessário *(padrão é Estados Unidos)*
    - Inserir Número de Telefone
    - Clicar **"Next"**
    - Inserir o código de 6 dígitos enviado para o dispositivo
    - Clicar **"Done"**

### Provisionamento do app Meta Horizon

14. **Abrir aplicação Meta Horizon do telefone**
    - Escolher **Continue with email**
    - Inserir o email usado para criar a conta Meta da Organização *(Pode ser fornecido pela WPS)*
    - Clicar **"Next"**
    - Escolher **"Enter password instead"** *(mais fácil que código de email)*
    - Inserir sua senha da conta Meta *(pode ser fornecida pela WPS)*

15. **Verificar conta via 2FA *(pode ser necessário)***
    - Selecionar método 2FA do dropdown
    - Clicar **"Next"**
    - Abrir aplicação autenticadora ou procurar por mensagem SMS/WhatsApp
    - Inserir código de 6 dígitos
    - Clicar **"Next"**

16. **Gerenciar persistência de login (opcional)**
    - Escolher se salvar credenciais de login neste computador
    - *Salvar credenciais armazena apenas informações de email e senha*
    - *Considere implicações de segurança de credenciais salvas em computadores compartilhados*
  
### Configurar conta Meta Horizon

- *A conta Meta Horizon é usada exclusivamente para o espaço VR da Meta*
- *Algumas opções serão visíveis para outros usuários Meta Horizon*

17. **Escolher um nome de usuário Meta Horizon**
    - *Este nome de usuário será visível para outros usuários Meta Horizon*
    - Inserir um nome de usuário aceito *(uma marca de verificação verde indicará que o nome de usuário é válido)*
    - Clicar **"Continue"**
    - Você será levado ao painel Meta Horizon
<div style="page-break-after: always;"></div>

### Configuração do headset

18. **Ligar headset**
    - Remover material de embalagem do headset
    - Remover economizadores de bateria dos controles manuais
    - **Quest 2**: Pressionar **botão de energia** no lado direito
    - **Quest 3 & Quest 3s**: Pressionar **botão de energia** no lado esquerdo
    - Colocar o headset VR

19. **Introdução inicial e conectar ao WiFi**
    - Seguir os prompts na tela no Headset VR
    - *Ocasionalmente controles manuais instalarão uma atualização que os torna inoperáveis por um breve período*
    - Conectar seu headset à sua conexão WiFi de internet
    - *WPS recomenda inserir os detalhes WiFi em seu headset*
    - *Se sua rede WiFi estiver oculta vá para Passo #20*
    - Seu headset pode aplicar atualizações de firmware
    - Deixar seu headset conectado enquanto atualizações são baixadas
    - *Seu headset pode indicar que você pode continuar configuração no app Meta Horizon do telefone*
    - ⚠️ **WPS não recomenda que você faça isso e sugere esperar até o headset exibir seu código de pareamento**

### Adicionar uma rede WiFi oculta

20. **Adicionando uma rede oculta ao WiFi**
    - *Você pode precisar de assistência do departamento de TI da sua empresa se você tem um programa robusto de segurança WiFi*
    - Na janela WiFi rolar para baixo até **"+ New Network >"**
    - Clicar para adicionar uma nova rede
    - Clicar **"Advanced"**
    - Sob **"Hidden Network"** mudar valor exibido para **"Yes"**
    - Geralmente os valores padrão para o resto do menu Advanced serão suficientes
    - *Se você continuar tendo problemas conectando a uma rede WiFi oculta você pode precisar contatar o departamento de TI da sua empresa*
    - Clicar **"Confirm"**
    - Se sua rede WiFi tem uma senha, provavelmente usa **WPA/WPA2-Personal** como configuração **"Security"**
    - Inserir os detalhes restantes de sua rede WiFi
    - Clicar **"Connect"** para terminar configuração WiFi e conectar à rede
<div style="page-break-after: always;"></div>

### Parear headset com app Meta Horizon do telefone

21. **Navegar para Devices no app Horizon**
    - Abrir seu app Meta Horizon do telefone
    - O app Meta Horizon mostrará o avatar da conta e um menu hambúrguer *(três barras horizontais)* no lado direito.
    - Abrir o menu hambúrguer
    - Sob **Device Management** clicar **Devices**

22. **Parear headset com app Meta Horizon**
    - Encontrar a opção **Pair New Headset** e clicar nela
    - Selecionar o modelo correto do headset Meta
    - *Você pode ser solicitado a criar um avatar - este passo agora é requerido pela Meta*
    - *Este avatar é visível para outros usuários Meta Horizon*
    - Criar um avatar e clicar **"Continue"**
    - Seu headset deve estar exibindo um código de cinco dígitos
    - Inserir o código de cinco dígitos quando solicitado
    - Clicar **"Continue"** quando a tela de pareamento bem-sucedido for mostrada

### **Aceitar condições da Meta**

23. **Aceitar disclaimers no app Meta Horizon**
    - Clicar **"Continue"** nas diretrizes de segurança
    - Clicar **"Don't Share"** ou **"Share"** na solicitação de compartilhar dados adicionais
    - Clicar **"Not now"** na solicitação Enable hand and body tracking
    - Clicar **"Skip"** na oferta Start 3-month trial *(Esta tela pode ou não estar presente)*
    - Clicar **"Skip"** em Add a payment method
    - Clicar **"Close"** na tela **You're all set!**

### **Finalizar configuração do headset**

24. **Finalizar introdução do Headset**
    - Colocar o headset VR para uma breve introdução ao seu headset da Meta
    - Seguir prompts na tela
    - Participar em tutoriais conforme desejado *(Pular tutoriais não afeta configuração do headset)*
    - *Você deve manter o headset durante a introdução*
    - Após a introdução você será mostrado o painel Horizon

## Próximos Passos

**Habilitar Modo Desenvolvedor**
- Seguir o guia **Developer Mode Setup**
- Modo desenvolvedor é necessário para aplicar algumas configurações recomendadas
- Modo desenvolvedor é necessário para remover o limite de segurança requerido
<div style="page-break-after: always;"></div>

**Aplicar Configurações Recomendadas do Headset**
- Seguir o guia **Recommended Headset Settings**

**Remover Software Desnecessário**
- Seguir o guia **Library Management**

## Solução de Problemas

**Não consegue acessar conta Meta:**
- Verificar se endereço de Email está correto para sua configuração VR *(Se fornecido pela WPS)*
- Contatar WPS para assistência com senha

**Código de confirmação da Meta ausente:**
- Códigos de confirmação podem ser atrasados por conexões de internet lentas ou intermitentes
- Verificar a pasta **Spam** em seu navegador de email
- Garantir que você está olhando na conta de email correta *(conta pode ter sido fornecida pela WPS)*

**Dispositivos 2FA já existem para conta Meta**
- Se sua conta Meta foi criada pela equipe WPS ela será pré-populada com 2 - 3 dispositivos 2FA
- Um destes dispositivos deve corresponder à conta de email provisionada pela WPS
- Outros dispositivos 2FA serão usados pela Equipe WPS para assistir na solução de problemas se problemas surgirem

**Botão "Add" acinzentado para 2FA:**
- Conta pode ter número máximo de dispositivos vinculados
- Contatar WPS para remover dispositivos não utilizados
- Alguns tipos de conta têm limites de dispositivos

**Não consegue encontrar aplicação Meta Horizon:**
- A aplicação Meta Horizon está disponível para download na Apple App store ou Google Play store
- Se você está usando um telefone fornecido pela WPS o app deve estar presente - procurar por Horizon
- O app Meta Horizon pode não estar colocado na primeira página do seu telefone
- Usar a função de busca do telefone para encontrar Meta Horizon e movê-lo para um local óbvio

**Não consegue fazer login no app Meta Horizon**
- Garantir que você está usando a mesma conta que foi usada nos passos de Criação de Conta Meta
- Garantir que você selecionou "Enter Password instead" se você está tentando inserir uma senha
- Verificar novamente sua senha, ela será a senha da Conta Meta, não da conta de email para login Horizon
<div style="page-break-after: always;"></div>

**2FA falha para o app Meta Horizon**
- Garantir que você está usando a conta 2FA correta para autorização
- Se você está usando SMS/WhatsApp para autorização apenas um número de telefone está associado com a conta
- Códigos 2FA são válidos por 30 segundos em média, esperar até um novo código ser gerado e tentar fazer login

**Meta não permite meu nome de usuário desejado**
- Meta restringe o formato de nomes de usuário para enforçar singularidade.
- Editar o nome de usuário para incluir sublinhados ou números
- Lembrar que este nome de usuário pode se tornar visível para outros usuários Meta Horizon

**Headset não reconhece controles manuais**
- Na inicialização inicial de um headset atualizações de firmware podem ser aplicadas aos controles manuais que os tornam temporariamente não-funcionais
- Esperar 2 - 3 minutos antes de tentar usar controles manuais novamente
- Inserir baterias frescas nos controles manuais
- Muito raramente pode haver outros problemas com controles manuais - Agendar uma sessão de ajuda com Equipe WPS para orientação adicional

**Headset incapaz de conectar ao WiFi**
- Garantir que seu departamento de TI permite dispositivos não reconhecidos a conectar ao canal WiFi da sua empresa
- Registrar o dispositivo VR com seu departamento de TI se necessário
- Garantir que você tem a rede WiFi correta e senha inseridas nos campos apropriados
- Se sua rede WiFi está oculta, ir para Passo #20 - *Você pode precisar de assistência do seu departamento de TI com redes ocultas*

**Incapaz de encontrar menu Devices no App Horizon**
- Garantir que você está na página principal do app Meta Horizon - *Você deve ver seu avatar de usuário e nome*
- Fechar o App Horizon e reabrir a aplicação para carregar a página principal
- Identificar o menu hambúrguer no lado direito da aplicação - ícone são três barras horizontais empilhadas
- Abrir o menu hambúrguer e rolar para baixo para ver a seção **"Device management"**
- Verificar se há atualizações pendentes para o app Meta Horizon ou sistema operacional do seu telefone
<div style="page-break-after: always;"></div>

**Forçado a criar um Avatar**
- Meta agora força usuários a criar um Avatar para seu usuário
- Se você desabilitou ou bloqueou a maioria das mídias sociais este avatar será minimamente visível para outros usuários
- Se você quiser verificar suas configurações de privacidade, abrir o menu hambúrguer e rolar para baixo até **"Privacy and security"** para abrir a seção **"Privacy settings"**

**Código de pareamento de 5 dígitos não aceito**
- Pode levar um tempo para pareamento do headset completar dependendo da conectividade da internet
- Garantir que seu telefone e headset estão na mesma rede WiFi
- Verificar novamente o código exibido no headset e conforme inserido no app Meta Horizon

## Notas Importantes

⚠️ **App Meta Horizon**: Meta requer o uso da aplicação do telefone **Meta Horizon** para configurar headsets Quest.

⚠️ **Criação de Avatar**: Meta requer a criação de um avatar virtual. Este avatar é visível em alguns locais através do "metaverso" VR dependendo das configurações de privacidade.

⚠️ **Dificuldade com 2FA**: Quando Meta pede por um método 2FA pode haver múltiplas opções apresentadas. Apenas um número de telefone pode ser usado para alertas SMS/WhatsApp para autenticação. Garantir que você está selecionando a conta correta para 2FA. Códigos 2FA geralmente duram por 30 segundos, se um código está prestes a expirar, esperar por um novo ser gerado.

⚠️ **Redes de internet**: Se seu headset e telefone não estão conectados à mesma rede WiFi pode não ser possível parear seu headset com o app.