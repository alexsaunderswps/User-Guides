# Configurações Recomendadas do Headset Quest VR

## Propósito e Contexto
Este guia detalha configurações recomendadas para Quest 2, Quest 3 e Quest 3s, para tornar a experiência VR do WildXR consistente e confiável.

⚠️ **Meta**: Hardware e software da Meta (incluindo MQDH) estão fora do controle da WPS. Atualizações da Meta podem causar mudanças inesperadas de funcionalidade em sistemas VR. A WPS monitora lançamentos da Meta para informar usuários sobre potenciais impactos e mudanças.

## Pré-requisitos
- Headset Quest e controles com baterias

## Visão Geral Rápida (para usuários experientes)
1. Entrar no menu **Settings**
2. Mudar configurações de energia para corresponder ao caso de uso desejado
3. Habilitar:
    - **Do Not Disturb**
    - **Developer Mode**
    - **Enable MTP connection**
4. Desabilitar:
    - **Cloud Backup**
    - **Automatic Updates**
    - **Interactive Elements**

## Passos Detalhados

### Acessando o Menu Settings

1. **Sair da Aplicação WildXR (se executando)**
   - Pressionar o **botão Meta-logo** (Quest 3 e Quest 3s) ou o **botão Oval Horizontal** (Quest 2) no controle da mão direita
   - Selecionar **"Quit"** na janela de gerenciamento de App que aparece
   - Se a janela de gerenciamento de App não aparecer:
     - Pressionar o **botão de energia do headset** para adormecer o headset
     - Pressionar o **botão de energia do headset** novamente para acordar o headset
     - Pressionar o **botão Meta-logo** no controle da mão direita
     - Selecionar **"Quit"** na janela de gerenciamento de App

2. **Abrir o Menu Quick Settings**
   - Clicar no **botão que exibe hora, força do WiFi e nível da bateria** na Barra de Menu esquerda
   - *Uma nova janela flutuante deve aparecer exibindo Quick Menu Settings*
<div style="page-break-after: always;"></div>

3. **Abrir o Menu Settings**
   - Clicar **"Settings"** no canto superior direito da exibição Quick Settings Menu
   - *Uma nova janela flutuante deve aparecer exibindo Settings do headset*
   - *Algumas opções não serão visíveis até você rolar a lista do lado esquerdo de categorias de configuração*
   - *Joysticks em qualquer controle permitirão rolar quando o retículo de mira estiver sobre a lista*

### Configurações Gerais

4. **Configurações Software Update**
   - Clicar na aba **"Software Update"**
   - Desativar **todas** as opções:
     - `Software updates`
     - `Security and Critical updates`
     - `Automatically power headset to update`
     - `Update and backup before shutdown`

5. **Configurações Cloud Backup**
   - Clicar na aba **"Cloud Backup"**
   - Desativar `Cloud Backups`

6. **Configurações Power**
   - Clicar na aba **"Power"**
   - Definir **"Display Off"** para **4 hours**
   - Definir **"Auto Sleep Headset"** para **4 hours** *(pode não estar presente em todos os headsets)*
   - Desativar **todas** as opções sob **"Battery"**:
     - `Battery Saver`
     - `Low battery audio alert`
     - `Low battery voice alert`

### Configurações de Notificação

7. **Configurações Notification**
   - Ativar `Do Not Disturb`
   - Selecionar **"Until I turn it off"** das opções que aparecem
   - Clicar **"Done"**

### Configurações de Configuração do Ambiente

8. **Configurações Interactive Objects**
   - Clicar na aba **"Interactive objects"**
   - Desativar **todas** as opções:
     - `Avatar Mirror`
     - `First Encounters`
     - `Portal to Meta Horizon World`
<div style="page-break-after: always;"></div>

### Configurações Avançadas

9. **Configurações Developer**
   - Ativar `Enable Developer Settings`
   - Ativar `Enable MTP Notification`
   - Desativar `Physical Space Features`
   - Desativar `Link Auto-Connect`

### Próximos Passos

10. **Criar PIN do App e bloquear apps**
    - Seguir o guia **Library Management**

## Entendendo Configurações Recomendadas do Headset

**Por que Estas Configurações:**
As configurações recomendadas foram testadas em locais públicos e fornecem a experiência de usuário mais consistente e duradoura até o momento.

**Configurações Software Update**
Desligar todas as configurações de atualização automática previne que um headset fique inesperadamente indisponível durante horários públicos. Também permite que atualizações de software sejam testadas de maneira controlada para prevenir conflitos não antecipados entre WildXR, Auto Launch e software do headset. Meta instituiu atualizações forçadas após 30 - 45 dias de atraso, permitindo à WPS uma janela para verificar atualizações para performance e reagir, quando possível, a conflitos de software. Recomendamos verificar headsets para atualizações pendentes a cada 21 dias como manutenção de rotina e contatar WPS para orientação sobre instalação.

**Configurações Cloud Backup:**
Não há benefício para Cloud Backup na maioria dos casos de uso do usuário final onde WildXR é usado em um ambiente público ou educacional.

**Configurações Power**
Definir **"Display Off"** para **4 hours** permite que headsets usados em um ambiente público ou educacional sejam imediatamente responsivos ao uso. Fazer com que o display se desligue prolongará a vida da bateria, mas pode causar que o headset seja lento para responder ao uso e influenciar a orientação de cenas no WildXR de maneiras inesperadas.

**Configurações Notification**
Notificações podem causar interrupção de experiências de usuário exibindo janelas pop-up dentro da aplicação WildXR.

**Configurações Interactive Objects**
Um usuário pode se encontrar na tela do menu principal Quest se houver um problema inesperado com o programa Auto Launch ou a aplicação WildXR. Usuários familiarizados com headsets VR podem forçar saída do WildXR em certas situações para acessar o menu principal Quest. Ao ocultar objetos interativos podemos prevenir algum comportamento malicioso ou simplesmente curioso de alterar configurações do dispositivo.
<div style="page-break-after: always;"></div>

**Configurações Developer**
Desativar funcionalidades de espaço físico remove a necessidade de definir um limite no headset. Configuração de limite pode interferir com experiência do usuário interrompendo a exibição WildXR se um usuário se mover fora do limite. Limites também são necessários para serem configurados cada vez que um headset é movido qualquer distância e podem causar comportamento inesperado em algumas situações.
Notificações MTP permitem que o headset seja visto como um drive quando conectado a um computador via USB. Isso permite transferência e manipulação de arquivos, necessário em algumas situações de solução de problemas.

## Solução de Problemas

**Seção Developer não visível sob Advanced Settings:**
- Revisar o Guia para habilitar Developer Settings em seu headset
- Garantir que sua conta Meta tem privilégios de desenvolvedor habilitados pela WPS
- Verificar que modo desenvolvedor está habilitado tanto no app Meta Horizon do telefone quanto nas configurações do headset

**Mudanças de configurações não persistem:**
- Garantir que você complete cada seção totalmente antes de mover para a próxima
- Verificar que o headset não está em um modo restrito ou controles parentais
- Verificar que sua conta tem privilégios administrativos no dispositivo

**Não consegue acessar certas opções de configurações:**
- Confirmar que sua conta Meta tem as permissões necessárias
- Verificar se o headset está inscrito em um sistema de gerenciamento organizacional
- Verificar que a versão do software do headset suporta todas as configurações listadas

**Configurações de energia causando comportamento inesperado:**
- Testar **"Display Off"** timing diferente se 4 horas causar problemas
- Monitorar vida da bateria com configurações ajustadas
- Garantir que o headset permanece responsivo durante horários de pico de uso

## Notas Importantes

⚠️ **Aviso de Valores Padrão**: Valores padrão podem prolongar vida da bateria mas podem introduzir comportamento inesperado na aplicação WildXR.

⚠️ **Pré-requisitos Developer**: Se uma seção Developer não estiver visível sob Advanced Settings, revisar o Guia para habilitar Developer Settings em seu headset.

⚠️ **Gerenciamento de Atualização**: Meta instituiu atualizações forçadas após 30-45 dias de atraso. Verificar headsets para atualizações pendentes a cada 21 dias e contatar WPS para orientação.

⚠️ **Privilégios Developer Necessários**: Sua conta Meta deve ter acesso de desenvolvedor concedido pela WPS antes que modificações de configurações avançadas estejam disponíveis.