
## 7.1 Learning Objectives
After completing this chapter, you should be able to do the following: 

1 -Recall major functions of the Media Layer. 

2 -Describe major components of the Media Layer. 

3 - Describe the T-Server.

4 - Describe the SIP Server. 

5 - Describe the Interaction Server. 

6 - Describe attached data.

7- Describe Computer Telephony Integration (CTI).

8- Explain the role of Genesys within CTI.

9- Describe the basic features of Workspace Desktop Edition.

10- Handle an inbound call.

508 / 5.000
Resultados de tradução
7.1 Objetivos de Aprendizagem
Depois de concluir este capítulo, você deve ser capaz de fazer o seguinte:

1 -Recupere as principais funções da camada de mídia.

2 -Descreva os principais componentes da camada de mídia.

3 - Descreva o T-Server.

4 - Descreva o Servidor SIP.

5 - Descreva o Interaction Server.

6 - Descreva os dados anexados.

7- Descrever a Integração Computador Telefonia (CTI).

8- Explicar o papel da Genesys dentro do CTI.

9- Descreva os recursos básicos do Workspace Desktop Edition.

10- Atender uma chamada de entrada.


## 7.2 Review Functions of Media Layer


**Functions of Media Layer**

The Media Layer serves as the center of any Genesys system, receiving and distributing messages as directed by the other components. The Media Layer enables solutions to communicate with a variety of media including traditional telephony systems, voice over IP (VoIP), email, instant messaging, and the Web. This layer also provides the mechanism for attached data distribution within and across solutions.


**External Interfaces**

External interfaces are interfaces to communication media such as voice and multimedia devices.

**Call Tracking**

Call tracking is maintaining the current state of each interaction and all the business data collected about each interaction during the processing stages.

**Attach Data Distribution**

Attach data distribution is the distribution of interaction-related business data within and across solutions. For example, the distributed attached data are sent to all the applications that participate in the interaction processing. 

**Funções da camada de mídia**

A camada de mídia serve como o centro de qualquer sistema Genesys, recebendo e distribuindo mensagens conforme orientado pelos outros componentes. A camada de mídia permite que as soluções se comuniquem com uma variedade de mídias, incluindo sistemas tradicionais de telefonia, voz sobre IP (VoIP), e-mail, mensagens instantâneas e a Web. Essa camada também fornece o mecanismo para distribuição de dados anexados dentro e entre soluções.

**Interfaces externas**

Interfaces externas são interfaces para meios de comunicação, como dispositivos de voz e multimídia.

**Rastreamento de chamadas**

O rastreamento de chamadas mantém o estado atual de cada interação e todos os dados de negócios coletados sobre cada interação durante os estágios de processamento.

**Anexar distribuição de dados**

A distribuição de dados de anexação é a distribuição de dados de negócios relacionados à interação dentro e entre soluções. Por exemplo, os dados anexados distribuídos são enviados para todos os aplicativos que participam do processamento da interação.

## 7.3 The Contact Center and Media Layer

Contact centers manage customer interactions that are made up of a variety of media, such as:
- Traditional voice telephony systems
- VoIP
- Non-voice media such as web chat and email
- Non-voice interactions such as fax

Os contact centers gerenciam as interações com os clientes que são compostas por uma variedade de mídias, como:
- Sistemas tradicionais de telefonia vocal
- VoIP
- Mídia não-voz, como bate-papo na web e e-mail
- Interações sem voz, como fax

![image](https://user-images.githubusercontent.com/52088444/157725807-e6b938a7-3fac-4e4d-97a3-607516f1f803.png)

If your contact center uses Voice, it will contain the following:
- Phones
- DNs 
-  Switches (PBX) 
- Agents 
- Genesys T-Servers 

If you use VoIP instead of traditional voice, it will contain the following:
-  Soft phones
- Softswitches 
- Agents 
- Genesys SIP Servers instead of T-Servers

If you use Non-Voice such as chat or email, it will contain:

- Corporate email servers 
- Web servers 
- SMS gateway interface 
- Genesys Interaction Servers

Se o seu contact center usar o Voice, ele conterá o seguinte:
- Telefones
- DN
- Comutadores (PBX)
- Agentes
- Genesys T-Servers

Se você usar VoIP em vez de voz tradicional, ele conterá o seguinte:
- Telefones macios
- Softswitches
- Agentes
- Genesys SIP Servers em vez de T-Servers

Se você usar Não-Voz, como bate-papo ou e-mail, ele conterá:

- Servidores de e-mail corporativos
- Servidores Web
- Interface de gateway SMS
- Servidores de Interação Genesys


## 7.4 Genesys Media Layer Applications

Media Servers such as T-Server, Interaction Server, or SIP Server are at the center of any Genesys system, receiving and distributing messages as directed by the other components. 

The Media Layer enables solutions to communicate with a variety of media including traditional telephony systems, VOIP, email, and the Web. 

Servidores de mídia como T-Server, Interaction Server ou SIP Server estão no centro de qualquer sistema Genesys, recebendo e distribuindo mensagens conforme indicado pelos outros componentes.

A camada de mídia permite que as soluções se comuniquem com uma variedade de mídias, incluindo sistemas de telefonia tradicionais, VOIP, e-mail e a Web.

**Traditional/TDM Telephony(Telefonia Tradicional/TDM)**

T-Server—Provides an interface with traditional telephony systems.

T-Server—Fornece uma interface com sistemas de telefonia tradicionais.

**VoIP**

SIP Server—Provides an interface with VoIP telephony systems.

Servidor SIP—Fornece uma interface com sistemas de telefonia VoIP. 

**Multimedia**

Interaction Server—Provides an interface with non-voice media such as Web chat, email, and other non-voice work items.

Interaction Server—Fornece uma interface com mídia sem voz, como bate-papo na Web, e-mail e outros itens de trabalho sem voz.

##  7.5 T-Server, SIP Server, and Interaction Server


T-Server is the heart of the Media Layer—translating the information of the media-device realm into information that Genesys solutions can use. It enables your contact center to handle the computer-based form of the interactions that arrive and translates the information surrounding a customer contact into reportable and actionable data. SIP Server has the same position in the Genesys Media Layer as all Genesys T-Servers. SIP Server is an application server that integrates Genesys telephony-based applications to various SIP-based products.

O T-Server é o coração da camada de mídia — traduzindo as informações do domínio do dispositivo de mídia em informações que as soluções da Genesys podem usar. Ele permite que seu contact center lide com o formulário baseado em computador das interações que chegam e traduz as informações em torno de um contato do cliente em dados relatáveis e acionáveis. O SIP Server tem a mesma posição na Genesys Media Layer que todos os Genesys T-Servers. O SIP Server é um servidor de aplicativos que integra aplicativos baseados em telefonia da Genesys a vários produtos baseados em SIP.

![image](https://user-images.githubusercontent.com/52088444/157728445-24e79114-1432-4a62-8485-d39cdb7ab1f5.png)

## 7.6 Attached Data

SIP Server/T-Server can receive, store, and distribute virtually any kind of data associated with a specific interaction (phone, email, or other media). For example, if a call has been partly handled by one agent and is now being transferred to another, information related to the call can be transferred to the new agent along with the call and can appear on the new agent’s screen the moment the call is answered. 

Business information can be attached to the call. That attached data can be carried with the transaction when it is transferred between agents, between applications, and between sites in a multi-site configuration.

O SIP Server/T-Server pode receber, armazenar e distribuir praticamente qualquer tipo de dado associado a uma interação específica (telefone, e-mail ou outra mídia). Por exemplo, se uma chamada foi parcialmente atendida por um agente e agora está sendo transferida para outro, as informações relacionadas à chamada podem ser transferidas para o novo agente junto com a chamada e podem aparecer na tela do novo agente no momento em que a chamada é respondidas.

As informações comerciais podem ser anexadas à chamada. Esses dados anexados podem ser transportados com a transação quando são transferidos entre agentes, entre aplicativos e entre sites em uma configuração multisite.

![image](https://user-images.githubusercontent.com/52088444/157728755-076aaaec-d006-4121-afa7-803e810a6198.png)

Associating business data with contacts is so powerful because of the following reasons:

-  Screen pops can display pertinent information on the agent’s screen before or during the interaction, which speeds up interaction handling.
- Attached data allows collection of information from customers during a contact.
- Attached data allows intelligent transfers, where the customer information is transferred to the second agent together with the call.
- Interactions can be routed and handled differently depending on the values of attached data.
- You can produce reports based on attached data values

A associação de dados comerciais a contatos é tão poderosa pelos seguintes motivos:

- Os pop-ups de tela podem exibir informações pertinentes na tela do agente antes ou durante a interação, o que acelera o tratamento da interação.
- Dados anexados permitem a coleta de informações dos clientes durante um contato.
- Dados anexados permitem transferências inteligentes, onde as informações do cliente são transferidas para o segundo agente junto com a chamada.
- As interações podem ser roteadas e tratadas de forma diferente dependendo dos valores dos dados anexados.
- Você pode produzir relatórios com base em valores de dados anexados

**Attached Data Format **

Attached data is in a Key-Value Pair (KVP) format. A key-value pair consists of two parts:
- A key indicates a description or label for the value.
- A value indicates the data being attached.

The following are examples of key-values pairs for attached data: 

Account:873212; Name:Mrs. Libora; Language:Spanish; Balance:56063.34

Os dados anexados estão em um formato de par de valores-chave (KVP). Um par chave-valor consiste em duas partes:
- Uma chave indica uma descrição ou rótulo para o valor.
- Um valor indica os dados que estão sendo anexados.

Veja a seguir exemplos de pares de valores-chave para dados anexados:

Conta: 873212; Nome: Sra. Libora; Idioma: Espanhol; Saldo: 56063,34


## 7.7 Computer Telephony Integration Terminology(7.7 Computer Telephony Integration Terminology)

Contact centers have hardware (a switch), software (databases and applications), and human resources (supervisors and agents). Traditionally, the computer functionality in a contact center involved agent representatives receiving and recording the information with no direct relation to the telephone switch.

Computer Telephony Integration (CTI) is the software, hardware, and programming necessary to integrate computers and telephones so they can work together seamlessly and intelligently. This intelligent combination of data with voice systems enhances telephone services.

CTI also means computer control and functionality applied to telephony hardware. In other words, CTI enables computer applications to control phone functionality. In addition, Genesys software uses CTI to provide contact centers with the ability to pass interaction data between agent desktops and to make interaction routing decisions.

Os contact centers possuem hardware (um switch), software (bancos de dados e aplicativos) e recursos humanos (supervisores e agentes). Tradicionalmente, a funcionalidade do computador em um contact center envolvia representantes de agentes recebendo e registrando as informações sem relação direta com a central telefônica.

Computer Telephony Integration (CTI) é o software, hardware e programação necessários para integrar computadores e telefones para que possam trabalhar juntos de forma transparente e inteligente. Essa combinação inteligente de dados com sistemas de voz aprimora os serviços telefônicos.

CTI também significa controle de computador e funcionalidade aplicada ao hardware de telefonia. Em outras palavras, o CTI permite que aplicativos de computador controlem a funcionalidade do telefone. Além disso, o software Genesys usa CTI para fornecer aos contact centers a capacidade de transmitir dados de interação entre desktops de agentes e tomar decisões de roteamento de interação.

Genesys CTI enables the following:
- Screen pop—Displays information on an agent’s computer screen as an interaction is being delivered to the agent
- Intelligent transfers—Displays interaction-related data on the computer screen of an agent receiving a transfer from another agent
- Intelligent routing—Expanded routing capabilities, such as routing to the last agent the customer spoke with or routing based on service levels and agent skills


Genesys CTI enables the following:
- Screen pop—Displays information on an agent’s computer screen as an interaction is being delivered to the agent
- Intelligent transfers—Displays interaction-related data on the computer screen of an agent receiving a transfer from another agent
- Intelligent routing—Expanded routing capabilities, such as routing to the last agent the customer spoke with or routing based on service levels and agent skills

## 7.8 Genesys Voice Scenario(7.8 Genesys Voice Scenario)

he following Genesys voice scenario demonstrates the ability of the system to do the following:
- Use the number of a caller to locate a matching record in a customer database.
- Use the account number in this customer record to do a further lookup of the customer’s information in the billing database.
- Use the last agent information in the matching customer record to instruct the switch to direct the call to the last agent who spoke to the customer.
- Populate a screen on the agent’s workstation with this customer’s information for reference when talking to the customer.

O seguinte cenário de voz da Genesys demonstra a capacidade do sistema de fazer o seguinte:
- Use o número de um chamador para localizar um registro correspondente em um banco de dados de clientes.
- Use o número da conta neste registro de cliente para fazer uma pesquisa adicional das informações do cliente no banco de dados de cobrança.
- Use as informações do último agente no registro do cliente correspondente para instruir a central a direcionar a chamada para o último agente que falou com o cliente.
- Preencha uma tela na estação de trabalho do agente com as informações deste cliente para referência ao falar com o cliente.

![image](https://user-images.githubusercontent.com/52088444/157730014-5abd44a5-0902-4800-a356-3fc824533d42.png)

![image](https://user-images.githubusercontent.com/52088444/157730085-7530d119-0867-45d3-aea2-44b4d72ec431.png)
![image](https://user-images.githubusercontent.com/52088444/157730173-467461ea-7e01-4c96-b85a-e503bedcfab1.png)
![image](https://user-images.githubusercontent.com/52088444/157730242-460e6384-daac-4616-bcff-afc8659509a2.png)
![image](https://user-images.githubusercontent.com/52088444/157730279-af1ede17-433a-4150-aaa1-e08ada3c0a24.png)

![image](https://user-images.githubusercontent.com/52088444/157730428-05ff4e7e-ae2d-464d-bea2-69b394dfd587.png)
![image](https://user-images.githubusercontent.com/52088444/157730461-f28457bd-dcdf-4be7-a95d-291560a4a676.png)

![image](https://user-images.githubusercontent.com/52088444/157730562-bbbd25b2-c29e-45d3-8c0f-9e44a69f2f92.png)
![image](https://user-images.githubusercontent.com/52088444/157730719-e705b75f-a166-4acf-8c08-3757f9a5d914.png)
![image](https://user-images.githubusercontent.com/52088444/157730800-31a36f2e-611d-4df7-ae70-44463dee0168.png)
![image](https://user-images.githubusercontent.com/52088444/157730849-417b68bb-cde1-4739-af4a-b6f17749526a.png)

![image](https://user-images.githubusercontent.com/52088444/157730890-2067d097-a4f2-4a08-a29a-a038cd4badbc.png)



Here is an introduction to the common terms related to telephone activity in a contact center. The diagram below demonstrates Voice architecture.

Aqui está uma introdução aos termos comuns relacionados à atividade telefônica em um contact center. O diagrama abaixo demonstra a arquitetura de voz.

![image](https://user-images.githubusercontent.com/52088444/157731296-db501451-f3fc-43b3-90f6-4682706c6187.png)

## 7.9 Abbreviations and Definitions

The following are the more common CTI abbreviations and definitions that you will need to know and should become familiar with in your contact center.

A seguir estão as abreviações e definições de CTI mais comuns que você precisa conhecer e com as quais deve se familiarizar em seu contact center.

![image](https://user-images.githubusercontent.com/52088444/157735757-fadc67d4-b381-4fb6-8cf5-b618fa5090aa.png)
![image](https://user-images.githubusercontent.com/52088444/157735780-2eb1cfd4-f516-48e1-bcbb-ca77a8714113.png)
![image](https://user-images.githubusercontent.com/52088444/157735836-d95eb11f-1411-4a87-8dfe-2ccf925a12cb.png)

## Voice Over IP Specific Terminology

![image](https://user-images.githubusercontent.com/52088444/157737135-2248a527-d99b-4665-8205-ad0a8d99d175.png)
![image](https://user-images.githubusercontent.com/52088444/157737297-02a4a252-fb80-42a4-979e-688ed06db257.png)

## 7.10 Creating an Interaction

Now that we have a better understanding of the Media layer's components and functionality that enables the entire Genesys Engage Platform, we can test the solution by communicating with a variety of media. In this example, we will be using voice to demonstrate the mechanism for interaction distribution using Agent Desktop.


Agora que entendemos melhor os componentes e a funcionalidade da camada de mídia que habilita toda a plataforma Genesys Engage, podemos testar a solução comunicando-se com uma variedade de mídias. Neste exemplo, usaremos a voz para demonstrar o mecanismo de distribuição de interação usando o Agent Desktop.

![image](https://user-images.githubusercontent.com/52088444/157868346-d18ada13-7ad4-485c-b5d3-783e07f1f0c1.png)


-  An Agent Desktop is a way for the agent to interact with the customer.
- Agent Desktop applications support the Agents interaction with customers.

Genesys developed an Agent Desktop application called Workspace Desktop Edition.

Before we get started with phone calls in this course, we’ll need a way for the agent to interact with the customer.

Customers/Partners can develop their own agent desktop application. 

- Um Agent Desktop é uma forma de o agente interagir com o cliente.
- Os aplicativos do Agent Desktop suportam a interação dos Agentes com os clientes.

A Genesys desenvolveu um aplicativo Agent Desktop chamado Workspace Desktop Edition.

Antes de começarmos com as chamadas telefônicas neste curso, precisaremos de uma maneira de o agente interagir com o cliente.

Os clientes/parceiros podem desenvolver seu próprio aplicativo de desktop de agente.

**Obs: Usaremos um subconjunto muito pequeno de recursos disponíveis com o Workspace para os propósitos desta classe.

Este não é um curso do Workspace. Para obter mais informações sobre o treinamento do Workspace, entre em contato com a equipe de treinamento da Genesys University.**

**Workspace Desktop Edition**

Workspace Desktop Edition (abbreviated as Workspace in this training) enables you to manage customer interactions from your desktop computer. Depending on your contact center, you may use the workspace to handle inbound calls, outbound calls, emails, or chats. Other team members can be used to assist with the interactions through coaching, conferencing, and transferring.

Edição de área de trabalho para desktop

O Workspace Desktop Edition (abreviado como Workspace neste treinamento) permite que você gerencie as interações com o cliente a partir de seu computador desktop. Dependendo do seu contact center, você pode usar o espaço de trabalho para lidar com chamadas recebidas, chamadas de saída, e-mails ou bate-papos. Outros membros da equipe podem ser usados ​​para ajudar nas interações por meio de coaching, conferência e transferência.

![image](https://user-images.githubusercontent.com/52088444/157868676-70733df6-3e20-48b9-80cf-c93fc8ba981f.png)

## 7.11 Logging into Workspace

A shortcut can be used to launch Workspace. In the initial screen, you must enter login credentials for Username and Password before clicking Log In.


Um atalho pode ser usado para iniciar o Workspace. Na tela inicial, você deve inserir as credenciais de login para Nome de usuário e Senha antes de clicar em Login.

![image](https://user-images.githubusercontent.com/52088444/157868787-176550de-26ad-4d92-8a6d-b7b723e88ea4.png)

In the next screen, verify and/or set the name of the Place, Media Type(s) such as voice and email, and optionally Queues. The choices for Media Type and Queue depend on your environment. In addition, you may or may not be able to change your place.

Na próxima tela, verifique e/ou defina o nome do Local, Tipo(s) de Mídia, como voz e e-mail e, opcionalmente, Filas. As opções para Tipo de mídia e Fila dependem de seu ambiente. Além disso, você pode ou não ser capaz de mudar de lugar.

![image](https://user-images.githubusercontent.com/52088444/157868915-6a838830-437e-4c26-96ed-856d87585585.png)

## 7.12 Getting Started with Workspace( Introdução ao Workspace)

Upon logging in to the Workspace, the opening view will look like the following:

Ao fazer login no Workspace, a visualização de abertura terá a seguinte aparência:

![image](https://user-images.githubusercontent.com/52088444/157874222-e09255cf-8faa-4a89-a1bd-f5464ffef1d9.png)


Workspace has two main viewing methods: A standard window-based method and a smaller less-obtrusive gadget-based method. The choice to exit is available from the Gadget and the Main Menu.

O Workspace tem dois métodos de visualização principais: um método padrão baseado em janela e um método menor baseado em gadget menos intrusivo. A opção de sair está disponível no Gadget e no Menu Principal

##  7.13 Status Menu

Hover the mouse over your status to see more details such as your status per media type.

Passe o mouse sobre seu status para ver mais detalhes, como seu status por tipo de mídia.

![image](https://user-images.githubusercontent.com/52088444/157874770-d3fa9be5-96c5-4555-89fb-a17d088970e8.png)

You can set your status for all your channels by clicking on the Status menu icon. Notice the Log Off status. This logs you out of agent functionality which means you can no longer process interactions. It does not log you out of Workspace or close Workspace. There is a separate Exit option to logout and close Workspace. 

Você pode definir seu status para todos os seus canais clicando no ícone do menu Status. Observe o status de Logoff. Isso desconecta você da funcionalidade do agente, o que significa que você não pode mais processar interações. Ele não desconecta você do Workspace nem fecha o Workspace. Há uma opção Sair separada para fazer logout e fechar o Workspace.

## 7.14 Handling an Inbound Call(Lidando com uma chamada de entrada)

The following images present how to handle an inbound voice call.

As imagens a seguir apresentam como lidar com uma chamada de voz de entrada.

![image](https://user-images.githubusercontent.com/52088444/157875861-3fb6cd0d-34df-4d97-a7ee-0371242e2599.png)

The workspace window pops open displaying information about the call.


A janela da área de trabalho é aberta exibindo informações sobre a chamada.


![image](https://user-images.githubusercontent.com/52088444/157876254-5e728f5b-b03c-4362-b850-3f5b29240bcb.png)

Quando terminar sua chamada, clique no botão desligar na parte superior da interface para desconectar a chamada.

![image](https://user-images.githubusercontent.com/52088444/157876599-f94b3e1e-a881-408a-99a3-7e2e33c32c0f.png)

Marque a caixa de seleção para marcar a chamada como concluída e feche a parte da janela que representa a chamada.

##  7.15 Learning Summary

Now that you have completed this chapter, you should be able to do the following: 

1 - Recall major functions of the Media Layer.

2 - Describe major components of the Media Layer.

3 - Describe the T-Server.

4-  Describe the SIP Server.

5 - Describe the Interaction Server. 

6 - Describe attached data.

7 - Describe Computer Telephony Integration (CTI).

8 - Explain the role of Genesys within CTI.

9 - Describe the basic features of Workspace Desktop Edition.

10 - Handle an inbound call.


Agora que você concluiu este capítulo, você deve ser capaz de fazer o seguinte:

1 - Recupere as principais funções da Media Layer.

2 - Descreva os principais componentes da camada de mídia.

3 - Descreva o T-Server.

4- Descreva o Servidor SIP.

5 - Descreva o Interaction Server.

6 - Descreva os dados anexados.

7 - Descrever a Integração Computador Telefonia (CTI).

8 - Explicar o papel da Genesys dentro do CTI.

9 - Descreva os recursos básicos do Workspace Desktop Edition.

10 - Atender uma chamada de entrada.

## 7.16 Learning check

Question
01/05
Which functions apply to the Media Layer? (Select all answers that apply.)

 - Interaction tracking( true)
 - Alarm processing
 - Access control
 - Database connectivity
 - Log events interface
 - External interfaces (true)
 - Dynamic reconfiguration and notification
 - Fault handling
 - Compilation of statistics and object status
 - Attached data distribution(true)
 - Configuration
 - Solution control

Question
02/05
Media Layer controls user access to solution functions and its data.

True

False (verdadeiro)

Question
03/05
Which components in the media layer enable voice for communication (select all that apply)?

Interaction Server 

TServer  (true)

Configuration Server

SIP Server (true)

Question
04/05
In addition to the Agent Status menu, where can you change your status from Not Ready to Ready for inbound calls?

Contact Center Statistics

My Channels(correto)

Main Menu

My Statistics

What would you use to log out of all channels and close Workspace?

![image](https://user-images.githubusercontent.com/52088444/157880315-ecfd6ebb-8a99-427e-b220-5ffbd467663e.png)

A

B

C (true)

D