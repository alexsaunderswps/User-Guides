# Guia de Reconexão de Conta Meta do Headset VR

## Propósito e Contexto
Este guia aborda o processo de reconectar um headset VR à sua conta Meta associada quando a ligação foi quebrada ou perdida. Reconexão de conta torna-se necessária quando headsets perdem sua conexão com servidores de autenticação da Meta, o que pode ocorrer após períodos prolongados offline, atualizações do sistema ou mudanças de segurança da conta.

⚠️ **Meta**: Hardware e software da Meta (incluindo MQDH) estão fora do controle da WPS. Atualizações da Meta podem causar mudanças inesperadas de funcionalidade em sistemas VR. A WPS monitora lançamentos da Meta para informar usuários sobre potenciais impactos e mudanças.

## Pré-requisitos
- Conexão estável com a internet para computador e headset VR
- Credenciais de conta de email associadas com sua configuração VR *(podem ser fornecidas pela WPS)*
- Senha da conta Meta *(pode ser fornecida pela WPS)*
- **Se você completou "Guia de Configuração de Acesso e Segurança da Conta Meta":**
  - Smartphone com app autenticador 2FA configurado
  - Acesso ao seu dispositivo de autenticação previamente configurado
- **Se você NÃO completou "Guia de Configuração de Acesso e Segurança da Conta Meta":**
  - Coordenação imediata com equipe WPS para provisão de código 2FA em tempo real
  - Horário agendado com suporte WPS para processo de autenticação guiado

## Visão Geral Rápida (para usuários experientes)
1. Navegar para `meta.com/device` e autenticar com credenciais da conta Meta
2. Completar verificação 2FA usando seu dispositivo configurado ou código fornecido pela WPS
3. Inserir o código de verificação de oito caracteres exibido na interface do headset VR
4. Confirmar reconexão bem-sucedida e testar funcionalidades dependentes da conta

## Passos Detalhados

### Acessando Interface de Gerenciamento de Dispositivos da Meta

1. **Navegar para portal de gerenciamento de dispositivos**
   - Abrir navegador web e ir diretamente para `meta.com/device`
   - *Esta URL especializada leva você diretamente à interface de gerenciamento de dispositivos da Meta*
   - *Evite usar o site geral meta.com pois requer passos de navegação adicionais*

2. **Iniciar autenticação da conta**
   - Selecionar **"Continue with email"** das opções de login disponíveis
   - *Este método fornece o caminho de autenticação mais confiável para tarefas de gerenciamento de conta*
<div style="page-break-after: always;"></div>

3. **Completar autenticação primária**
   - Inserir o endereço de Email associado com sua configuração VR
   - Clicar **"Next"** para prosseguir para verificação de senha
   - Escolher **"Enter password instead"** *(mais fácil que código de email)*
   - Inserir sua senha da conta Meta *(pode ser fornecida pela WPS)*
   - Clicar **"Log in"** para prosseguir para autenticação de dois fatores

### Completando Autenticação de Dois Fatores

4. **Lidar com verificação 2FA**
   - Sistema apresenta menu dropdown para métodos 2FA disponíveis
   - Selecionar o método que você configurou previamente ou conforme direcionado pela equipe WPS
   - Clicar **"Next"** para prosseguir para entrada de código
   - Inserir o código de autenticação de seis dígitos do seu app autenticador
   - *Se você não configurou 2FA pessoal, use o código fornecido pela equipe WPS durante sua sessão de suporte agendada*
   - Clicar **"Next"** para completar autenticação

5. **Gerenciar persistência de login (opcional)**
   - Escolher se salvar credenciais de login neste computador
   - *Salvar credenciais armazena apenas informações de email e senha*
   - *Verificação 2FA ainda será necessária para futuras sessões de login*
   - *Considere implicações de segurança de credenciais salvas em computadores compartilhados*

6. **Localizar código de verificação do headset**
   - Colocar seu headset VR ou verificar seu display
   - *Se um código de reconexão for necessário, geralmente nada mais será mostrado no headset*
   - *Este código é único para esta sessão e expira após um período razoável de tempo*
   - *Note o código cuidadosamente pois é sensível a maiúsculas/minúsculas e deve ser inserido exatamente*

7. **Inserir código de verificação**
   - Retornar à interface de gerenciamento de dispositivos Meta no seu computador
   - Confirmar que as informações corretas da conta Meta estão exibidas
   - Inserir o código de oito caracteres do seu headset no campo designado
   - *Verificar novamente cada caractere antes de prosseguir pois entrada incorreta requer recomeçar*
   - Clicar **"Continue"** para iniciar o processo de reconexão

8. **Verificar conexão bem-sucedida**
   - Sistema deve exibir confirmação de que seu dispositivo foi reconectado
   - O headset deve mostrar informações atualizadas de status da conta
   - Funcionalidades da conta Meta devem ficar disponíveis imediatamente na interface do headset
<div style="page-break-after: always;"></div>

## Solução de Problemas

**Autenticação falha repetidamente:**
- Verificar se endereço Gmail corresponde à conta de configuração VR
- Confirmar precisão da senha com equipe WPS
- Verificar se conta tem privilégios de desenvolvedor habilitados
- Garantir que códigos 2FA estão atuais (expiração de 30 segundos)

**Código de oito caracteres não aceito pela interface Meta:**
- Verificar se contas Meta da web e headset correspondem
- Confirmar que código de oito dígitos foi inserido corretamente
- Reiniciar headset para atualizar código

**Reconexão parece bem-sucedida mas funcionalidades da conta permanecem indisponíveis:**
- Permitir tempo para conta reconectar
- Reiniciar o headset

## Notas Importantes

⚠️ **Coordenação de Senha**: Nunca tente alterar senhas da conta Meta independentemente. Sempre coordene modificações de senha com equipe WPS para prevenir bloqueios de suporte técnico e garantir que todos os sistemas relacionados recebam atualizações necessárias.

⚠️ **Consistência de Conta**: A conta Meta usada para reconexão deve corresponder exatamente à conta originalmente configurada no headset. Usar contas diferentes, mesmo que pertençam à mesma organização, criará problemas persistentes de acesso.

⚠️ **Temporização de Segurança**: Códigos 2FA são sensíveis ao tempo. Códigos 2FA expiram a cada 30 segundos.