# Guia de Instalação do WildXR Auto Launch

## Propósito e Contexto
Este guia instala a aplicação WPS Auto Launch que inicia automaticamente o WildXR quando um headset é ligado. O Auto Launch elimina a necessidade de controles manuais em instalações públicas, cria uma experiência de usuário perfeita e permite o monitoramento remoto do tempo de funcionamento do headset. Este processo transforma um headset VR padrão em um sistema pronto para quiosque que requer interação mínima do usuário para começar a experiência de conservação.

⚠️ **Meta**: Hardware e software da Meta (incluindo MQDH) estão fora do controle da WPS. Atualizações da Meta podem causar mudanças inesperadas de funcionalidade em sistemas VR. A WPS monitora lançamentos da Meta para informar usuários sobre potenciais impactos e mudanças.

## Pré-requisitos
- Meta Quest Developer Hub totalmente instalado e configurado com pelo menos um headset conectado e depuração USB autorizada *(veja o Guia de Configuração MQDH)*
- Headset VR com modo Desenvolvedor habilitado tanto no app Oculus quanto nas configurações do headset
- Aplicação WildXR já instalada e executada com sucesso pelo menos uma vez no headset de destino
- Arquivo `autolaunchping_v.1.0.0.apk` *(fornecido pela WPS)*
- Conta Meta com privilégios de desenvolvedor habilitados pela WPS
- Cabo USB para conectar o headset durante a instalação

## Visão Geral Rápida (para usuários experientes)
1. Conectar headset de destino ao computador *(ou verificar conexão MQDH existente)*
2. Acessar gerenciamento de aplicações MQDH e instalar o APK `autolaunchping`
3. Executar aplicação Auto Launch e configurar integração WildXR
4. Testar funcionalidade de inicialização automática

## Passos Detalhados

### Preparando para a Instalação do Auto Launch

1. **Conectar headset para transferência de arquivos**
   - Executar **Meta Quest Developer Hub**
   - Ligar Quest Headset
   - Conectar Headset ao Computador com cabo USB

2. **Verificar conexão do headset**
   - Garantir que seu headset de destino apareça como **"Active"** na lista de dispositivos MQDH
   - *Novos headsets tipicamente requerem o mesmo processo de autorização de depuração USB completado durante a configuração MQDH (veja Guia de Configuração MQDH)*
   - Confirmar que o headset não mostra indicadores de erro ou problemas de conectividade
<div style="page-break-after: always;"></div>

3. **Confirmar prontidão do WildXR**
   - Verificar que WildXR está instalado no headset de destino
   - Garantir que WildXR foi executado com sucesso pelo menos uma vez
   - *Auto Launch não pode registrar aplicações que nunca foram executadas no sistema*
   - Testar inicialização do WildXR manualmente se incerto sobre seu status operacional

### Instalando a Aplicação Auto Launch

4. **Acessar gerenciamento de aplicações**
   - No MQDH, clicar no **ícone da pasta** na barra lateral esquerda
   - *Isso abre a interface de gerenciamento de arquivos e aplicações*
   - Sob a seção **"On Device"**, clicar no ícone da pasta **"Apps"**
   - *Isso exibe aplicações atualmente instaladas em seu headset*

5. **Adicionar a aplicação Auto Launch**
   - Clicar no botão **"Add Build"** no canto superior direito
   - *Navegador de arquivos abre para localizar seu arquivo APK de instalação*
   - Navegar até o local onde você salvou `autolaunchping_v.1.0.0.apk`
   - Selecionar o arquivo APK e clicar **"Open"**

6. **Monitorar progresso da instalação**
   - MQDH exibe indicadores de progresso da instalação
   - Permitir que o arquivo instale completamente antes de prosseguir
   - *Instalação tipicamente leva 30-60 segundos dependendo da performance do sistema*
   - Você deve ver `com.wps.autowildxrping` aparecer em sua lista de aplicações quando completo

### Configurando Integração Auto Launch

7. **Executar aplicação Auto Launch**
   - Localizar `com.wps.autowildxrping` em sua lista de aplicações MQDH
   - Clicar no **ícone de menu de três pontos** à direita do nome da aplicação
   - Selecionar **"Launch App"** do menu dropdown
   - Colocar o headset VR para completar a configuração

8. **Completar configuração Auto Launch**
   - WildXR pode executar imediatamente se Auto Launch detectar configuração existente
   - Se WildXR executar automaticamente, remover headset e reiniciar para testar funcionalidade
   - Se você vir uma janela **"WildXRAutoPing"** em vez disso, continuar com configuração manual
   - *Procurar por um tile parecendo um alienígena ou ícone incomum na barra de menu Quest se a janela não estiver imediatamente visível*
<div style="page-break-after: always;"></div>

9. **Finalizar configuração**
   - Na janela **WildXRAutoPing**, clicar no botão **"Save URL"**
   - *Isso cria a ligação permanente entre Auto Launch e WildXR*
   - WildXR deve executar imediatamente após clicar **Save URL**
   - Remover headset e reiniciar o dispositivo para verificar funcionalidade de inicialização automática

## Entendendo o Propósito da Tecnologia Auto Launch

Antes de começar a instalação, é útil entender o que o Auto Launch realiza e por que requer este processo de instalação especializado. Aplicações VR tradicionais requerem que usuários naveguem manualmente em menus e selecionem aplicações usando controles. Isso funciona bem para uso pessoal, mas cria barreiras em ambientes de conservação públicos onde visitantes podem não estar familiarizados com interfaces VR ou onde controles podem ser perdidos ou danificados.

A aplicação WPS Auto Launch opera no nível do sistema Android, registrando-se para disparar quando o headset completa sua sequência de inicialização. Pense nisso como definir um navegador web padrão em seu computador, exceto que ao invés de lidar com links web, Auto Launch lida com o evento de inicialização do headset. Quando o sistema inicia, Auto Launch imediatamente sinaliza WildXR para começar, criando uma transição perfeita de ligar para conteúdo de conservação.

Esta integração de nível de sistema é por que a instalação requer Meta Quest Developer Hub ao invés de métodos padrão de instalação de aplicações. Estamos essencialmente modificando o comportamento do headset em um nível mais profundo do que aplicações normais acessam.

## Solução de Problemas

**MQDH não mostra dispositivos conectados:**
- Verificar que você completou a configuração completa MQDH incluindo autorização de depuração USB
- Checar que seu headset de destino é o mesmo configurado durante configuração MQDH
- Se usando um headset diferente, ele precisará do mesmo processo de autorização de depuração USB
- Garantir que o headset permaneça ligado e conectado durante toda a instalação

**Instalação Auto Launch falha:**
- Confirmar que WildXR está propriamente instalado e foi executado com sucesso pelo menos uma vez
- Verificar que headset tem espaço de armazenamento suficiente para aplicações adicionais
- Checar que `com.wps.autowildxrping` aparece na lista de aplicações MQDH antes de prosseguir com configuração
- Garantir que o arquivo APK `autolaunchping` não está corrompido tentando instalação em um headset diferente
<div style="page-break-after: always;"></div>

**Funcionalidade Auto Launch não funciona após instalação:**
- Verificar que `com.wps.autowildxrping` aparece como executando no menu de três pontos MQDH
- Confirmar que WildXR executa manualmente para garantir integridade da aplicação
- Testar ciclo de energia completo ao invés de dormir/acordar para verificar comportamento de inicialização
- Checar que **"Save URL"** foi clicado durante configuração e que WildXR executou depois

**Janela WildXRAutoPing não visível:**
- Procurar por um ícone incomum ou parecido com alienígena na barra de menu Quest
- Tentar remover e colocar o headset de volta para atualizar a interface
- Garantir que aplicação Auto Launch foi realmente executada do MQDH ao invés de apenas instalada
- Checar que WildXR foi executado pelo menos uma vez antes da configuração Auto Launch

## Notas Importantes

⚠️ **Requisitos de Conta de Desenvolvedor**: Sua conta Meta deve ter status de desenvolvedor verificado com Wildlife Protection Solutions antes que qualquer instalação de aplicação customizada seja bem-sucedida.

⚠️ **Compatibilidade do Sistema**: Auto Launch requer headsets com modo desenvolvedor propriamente habilitado tanto na aplicação móvel Oculus quanto nas configurações internas do headset sob **Advanced > Developer**.

⚠️ **Correspondência de Conta**: A conta Meta usada para MQDH deve corresponder exatamente à conta usada para configurar o headset. Contas não correspondentes impedirão reconhecimento do dispositivo e instalação da aplicação.

⚠️ **Pré-requisitos WildXR**: WildXR deve estar instalado com sucesso e executado pelo menos uma vez antes da instalação Auto Launch. Auto Launch não pode registrar uma aplicação que o sistema não reconhece.

## Verificação e Teste

Após completar a instalação, verificar funcionalidade Auto Launch através de teste abrangente. Desligar o headset completamente usando o botão de energia, aguardar 30 segundos, então ligar novamente. Auto Launch deve disparar inicialização WildXR sem qualquer intervenção manual ou uso de controle. Se navegação manual ainda for requerida, o processo de registro não foi completado com sucesso e deve ser repetido a partir do passo 5.