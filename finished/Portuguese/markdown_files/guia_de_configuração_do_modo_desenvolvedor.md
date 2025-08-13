# Guia de Configuração do Modo Desenvolvedor

## Propósito e Contexto
Este guia fornece os passos necessários para autorizar uma conta Meta e headsets associados a essa conta com credenciais de desenvolvedor. 
Credenciais de desenvolvedor são necessárias para habilitar certas funcionalidades que são necessárias para resolver problemas de conexão, gerenciar configurações do dispositivo ou solucionar problemas de aplicações VR.

⚠️ **Meta**: Hardware e software da Meta (incluindo MQDH) estão fora do controle da WPS. Atualizações da Meta podem causar mudanças inesperadas de funcionalidade em sistemas VR. A WPS monitora lançamentos da Meta para informar usuários sobre potenciais impactos e mudanças.

## Pré-requisitos
- Uma conexão com a internet
- Credenciais de conta de email associadas com sua configuração VR *(podem ser fornecidas pela WPS)*
- Senha da conta Meta *(pode ser fornecida pela WPS)*
- Smartphone com capacidade de aplicativo 2FA
- Smartphone com aplicação Meta Horizon instalada
- Coordenação inicial com equipe WPS para primeiro login
- Headsets VR

## Visão Geral Rápida (para usuários experientes)
1. Conta Meta da Organização é adicionada ao grupo Developer WPS
2. Modo Desenvolvedor ativado para cada dispositivo no app Meta Horizon
3. Modo Desenvolvedor ativado em cada headset via Advanced Settings

## Passos Detalhados

### Autorização Inicial de Desenvolvedor

1. **Solicitar que Equipe WPS adicione a Conta Meta da sua Organização ao grupo Developer WPS**
   - *Se a equipe WPS criou a Conta Meta usada para registrar headsets este passo pode estar completo*
   - *Os seguintes passos são melhor completados durante uma chamada de vídeo*
   - Enviar informações da conta Meta para equipe WPS (**Endereço de Email** ou **Nome de Usuário**) solicitando acesso Developer
   - Equipe WPS irá convidar conta para se juntar à organização como Developer
   - Verificar email para convite ao Meta Quest Developer Dashboard do Meta Horizons

2. **Aceitar convite para se juntar ao grupo Developer WPS**
   - Abrir email de convite
   - Clicar **"View Invitation"** - um link web irá abrir - *(Recomendamos usar navegadores Chrome ou Firefox para este passo)*
<div style="page-break-after: always;"></div>

3. **Inserir credenciais**
   - Clicar **Continue with Email**
   - Inserir endereço de Email associado com sua configuração VR
   - Clicar **"Next"**
   - Escolher **"Enter password instead"** *(mais fácil que código de email)*
   - Inserir sua senha da conta Meta *(pode ser fornecida pela WPS)*
   - Clicar **"Log in"**

4. **Autorização de dois fatores (pode ser necessária)**
   - *Se você não habilitou autorização de dois fatores (2FA) para sua conta Meta você precisará fazer isso agora*
   - *Veja o Guia de Configuração de Acesso e Segurança da Conta Meta para detalhes sobre habilitar 2FA*
   - *Se sua conta foi criada pela equipe WPS você precisará coordenar acesso*

5. **Aceitar convite e verificar autorização** 
   - Aceitar convite no site Meta
   - *Uma caixa de seleção "accept invitation" deve estar visível na página web*
   - Confirmar com equipe WPS que o convite foi aceito e credenciais Developer foram autorizadas

### Conectar Headset ao aplicativo Meta Horizon do telefone

6. **Ligar headset VR**
   - *Os seguintes passos assumem que o headset VR foi configurado inicialmente*
   - *Se este não for o caso - veja **Guia de Configuração Inicial do Headset VR** para passos necessários*
   - Conectar headset VR à internet
   - *É melhor ter apenas um headset ligado de cada vez*

7. **Abrir Opções do Dispositivo**
   - Abrir aplicação Meta Horizon do telefone
   - *A conta usada para o headset VR deve ser a mesma usada para a conta Meta Horizon*
   - O app Meta Horizon mostrará o avatar da conta e um menu hambúrguer *(três barras horizontais)* no lado direito.
   - Abrir o menu hambúrguer
   - Sob **Device Management** clicar **Devices**

8. **Conectar ao dispositivo**
   - *Você pode ver múltiplos dispositivos listados* 
   - Um dispositivo deve mostrar um círculo verde e estar listado como **"Nearby"**
   - Clicar no dispositivo **Nearby**
   - Uma nova tela mostra detalhes do dispositivo e quatro opções **Manage your device**
<div style="page-break-after: always;"></div>

9. **Ativar Modo Desenvolvedor**
    - Clicar em **Headset Settings** - *(pode estar obscurecido por notificação Manage profiles)*
    - Você deve ver várias opções sob **Headset settings**
    - Clicar em **Developer Mode**
    - Ativar o interruptor **Developer Mode**

### Habilitar configurações Developer no headset VR

- *Você estará usando o headset VR para os próximos passos*
- *Para instruções detalhadas sobre acessar o menu Settings veja - **Configurações Recomendadas do Headset***

10. **Abrir o menu Advanced Settings**
    - Abrir o menu **Quick Settings** clicando no display de hora/WiFi/bateria
    - Clicar **Settings** no canto superior direito
    - À esquerda, rolar para baixo para encontrar **Advanced Settings**
    - Clicar na opção **Advanced Setting**

11. **Ativar Modo Desenvolvedor**
    - Rolar para baixo para encontrar seção **Developer**
    - Ativar **Enable Developer Settings**
    - Uma lista adicional de opções deve aparecer
    - Ativar **Enable MTP Notifcation**
    - Desativar **Physical Link Features**
    - Desativar **Link Auto-Connect**

## Solução de Problemas

**Nenhum Email de Convite recebido da WPS**
- Coordenar com equipe WPS antes de enviar email de acompanhamento
- Verificar o endereço de Email enviado para equipe WPS
- Verificar sua pasta de spam

**Incapaz de fazer login na conta Meta**
- Verificar o Email correto para a conta Meta
- Ao fazer login, usar código de email ao invés de senha para confirmar correspondência de conta
- Garantir que senha está correta para a conta 
- Se conta Meta foi criada pela WPS, coordenar solução de problemas adicional com equipe

**Problemas de autorização de dois fatores**
- Se conta foi criada pela WPS, coordenar ou receber acesso 2FA *(geralmente Google Authenticator)*
- Garantir que você está escolhendo o método correto para 2FA *(se múltiplas opções existem)*
- Equipe WPS será incapaz de assistir com 2FA via telefone ou SMS
<div style="page-break-after: always;"></div>

**Incapaz de aceitar convite para se juntar à Organização**
- Garantir que conta Meta corresponde ao endereço de Email no convite
- Tentar aceitar convite usando navegadores Chrome ou Firefox - *(Safari causou problemas no passado)*

**Incapaz de encontrar Dispositivo no app Meta Horizon**
- Garantir que tanto headset VR quanto telefone estão usando a mesma fonte de internet
- Verificar que headset VR e telefone estão logados com a mesma conta Meta
- Reiniciar tanto headset quanto app Meta Horizon
- Para reduzir possível confusão, garantir que apenas um headset VR está ligado

**Múltiplos Dispositivos aparecem como **Nearby** no app Meta Horizon**
- Desligar outros Dispositivos próximos para simplificar configuração
- Combinar números de série *(número de série é encontrado na têmpora esquerda do headset)*
- *Número de série está na parte interna da têmpora esquerda - Quest 3*
- *Número de série está na parte externa da têmpora esquerda, sob a cobertura da alça - Quest 2*

**Modo Desenvolvedor não disponível no app Meta Horizon**
- Garantir que conta Meta foi adicionada à Organização WPS como developer
- Fazer logout do app Meta Horizon e fazer login novamente
- Verificar se a conta Meta correta está sendo usada no app Meta Horizon

**Interruptor do Modo Desenvolvedor não permanece ativado no app Meta Horizon**
- Verificar que conta Meta foi adicionada à Organização WPS como developer
- Garantir que conta Meta correta está sendo usada no app Meta Horizon
- Verificar headset VR para diálogo de aviso ou mensagens de ação

**Configurações Developer não vistas em Advanced Settings no headset**
- Verificar que headset teve Modo Desenvolvedor ativado no app Meta Horizon
- Reiniciar headset VR
- Verificar headset para atualizações pendentes - *(aplicar quaisquer atualizações pendentes)*

## Notas Importantes

⚠️ **Convite da Organização WPS**: Coordenação deste passo é necessária antes de quaisquer configurações de conta Developer adicionais

⚠️ **Consistência de Conta**: Contas Meta devem corresponder entre a aplicação Meta Horizon e o headset VR.