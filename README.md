# 🚀 SAB BTP S4HANA Lab2learn 🚀

## 📅 Cronograma das Aulas  

| Data       | Conteúdo                                      |
|------------|-----------------------------------------------|
| 04/02/2025 | ENTENDA DE UMA VEZ POR TODAS O SAP BTP!       |
| 05/02/2025 | CRIANDO UM APP FIORI                          |
| 06/02/2025 | INTEGRANDO O SAP BTP COM O S/4HANA            |

---

### SAP - 

### BTP - 

### FUNCIONAL - 

### ABAP - 

---

## Como desenvolver o Projeto!

### Baixe o Aplicativo para testar o Projeto:

📱 Android - [Baixar App](https://play.google.com/store/apps/details?id=com.sap.appgyver.preview.release)

🍏 iPhone - [Baixar App](https://apps.apple.com/us/app/sap-build-apps-preview/id1585856868)

### Passo 1 - Criando conta SAP:

Lembrando que estamos usando uma versão gratuita Trial com duração de 90 dias. Após o término da duração, todos os projetos serão excluídos, então lembre-se de sempre manter uma cópia "local" do projeto!

Acesse o site: [SAP](https://www.sap.com/brazil/index.html?url_id=auto_hp_redirect_brazil)

- Clique no botão de usuário no canto superior direito

  ![image](Readme-Images/1.png)

- Clique em "Crie sua conta SAP"

  ![image](Readme-Images/2.png)

- Preencha todos os campos com suas informações

  ![image](Readme-Images/3.png)

  - Em Empresa, pode colocar um nome à sua escolha
  - Em Departamento, coloque "Educação"
  - Em Relacionamento com a SAP, coloque "Estudante"

- Revise seu e-mail e finalize o cadastro

  ![image](Readme-Images/4.png)

### Passo 2 - Configurando o Ambiente SAP BTP:

- Com a conta SAP registrada e logada, acesse o site: [SAP BTP](https://account.hana.ondemand.com/#/home/welcome)

- Clique em Sign In e logue com sua conta SAP criada no passo 1!

  ![image](Readme-Images/5.png)

- Clique em Trial Home

  ![image](Readme-Images/6.png)

- Utilize o seu número de telefone para receber um código de confirmação. Após confirmar, continue o processo

  > Caso o site ocorra algum erro durante este processo, acesse o site novamente pelo link acima e repita o processo até conseguir confirmar o telefone!

- Escolha a opção "US East(VA) - AWS"

  ![image](Readme-Images/7.png)

- Aguarde até que todas as opções apareçam corretamente!

  ![image](Readme-Images/8.png)

  > Caso alguma das opções acabe falhando, reinicie a página e tente novamente!

### Passo 3 - Configurando BTP Boosters

- Certifique-se de que está dentro de Trial | Global Account (Lembrando que cada um terá um número diferente em Global Account)
- Clique em Boosters no canto esquerdo da tela

  ![image](Readme-Images/9.png)

- Dentro da página Boosters, pesquise por Build
- Selecione "Get Started With SAP Build Apps - Detailed Account Setup"

  ![image](Readme-Images/10.png)

- Clique em "Start"

  ![image](Readme-Images/11.png)

- Aguarde as confirmações e clique em "Next"

  ![image](Readme-Images/12.png)

- Selecione "Select Subaccount", depois clique em "Next"

  ![image](Readme-Images/13.png)

- Clique em "Next"

  ![image](Readme-Images/14.png)

- Clique em "Next"

  ![image](Readme-Images/15.png)

- Aguarde até que todos os serviços apareçam com "DONE" e clique em "Finish"

  ![image](Readme-Images/16.png)

- Certifique-se de que todos os arquivos estão corretos!

  ![image](Readme-Images/17.png)
  ![image](Readme-Images/18.png)

  > Caso não consiga acessar Trial, lembre-se de se adicionar como Administrador clicando na engrenagem ao lado

  ![image](Readme-Images/19.png)

### Passo 4 - Adquirir uma "API Key" de "Sales Order (A2X)"

Acesse o site: [SAP API](https://api.sap.com)

- Clique em "SAP S/4HANA Cloud Private Edition"

  ![image](Readme-Images/20.png)

- Siga os 4 passos para acessar "Sales Order (A2X)"
- Ou acesse o link: [Sales Order API](https://api.sap.com/api/OP_API_SALES_ORDER_SRV_0001/overview)

  - Clique em "APIs"
  - Clique em "All"
  - Pesquise "sales order"
  - Clique em "Sales Order (A2X)"

    ![image](Readme-Images/21.png)

- Clique em "Show API Key"

  ![image](Readme-Images/22.png)

- Guarde esse link para o próximo passo!

### Passo 5 - Criando uma Destination

- Acesse sua "Trial" e clique em "Connectivity" e depois em "Destinations"

  ![image](Readme-Images/23.png)
  ![image](Readme-Images/24.png)

- Clique em "Create Destination" e configure conforme abaixo:

  **Destination Configuration**
  - Name: S4HANA_JORNADA
  - Type: HTTP
  - Description:
  - URL: https://sandbox.api.sap.com/s4hanacloud/sap/opu/odata/sap/API_SALES_ORDER_SRV
  - Proxy Type: Internet
  - Authentication: NoAuthentication

  **Additional Properties**
  - AppgyverEnabled: true
  - HTML5.DynamicDestination: true
  - URL.headers.apikey: Cole aqui a sua "API Key" (Adquirida no passo anterior)
  - WebIDEEnabled: true

  ![image](Readme-Images/25.png)
 
### Passo 6 - SAP Build

- Clique em "Services", depois em "Instances and Subscriptions"

  ![image](Readme-Images/26.png)

- Clique em "SAP Build Apps"

  ![image](Readme-Images/27.png)

- Clique em "Criar"

  ![image](Readme-Images/28.png)

- Clique em "Build an Application"

  ![image](Readme-Images/29.png)

- Clique em "SAP Build Apps"

  ![image](Readme-Images/30.png)

- Clique em "Web & Mobile Application"

  ![image](Readme-Images/31.png)

- Nomeie o seu projeto de "SalesOrderApp" e clique em "Create"

  ![image](Readme-Images/32.png)

---

- Se tudo der certo, você estará nesta página

  ![image](Readme-Images/33.png)

- Caso o app não tenha aberto sozinho, abra-o no menu inicial do SAP Build

  ![image](Readme-Images/34.png)

---

- Troque o modo de visualização para "Mobile"

  ![image](Readme-Images/35.png)

---

### Passo 7 - Adicionar Integração com o S/4HANA

- Clique em "Integrations"

  ![image](Readme-Images/36.png)

- Clique em "ADD INTEGRATION"

  ![image](Readme-Images/37.png)

- Clique em "BTP DESTINATIONS" dentro de SAP Systems

  ![image](Readme-Images/38.png)

- Selecione "S4HANA_JORNADA"

  ![image](Readme-Images/39.png)

- Clique em "Enable Data Entity"

  ![image](Readme-Images/40.png)

### Passo 8 - Editando a Interface do Usuário

- Clique em "User Interface" e edite o título e subtítulo conforme o exemplo:
  - **Título**: Sales Order - Seu Nome
  - **Subtítulo**: Aplicativo de busca de dados de todas as Sales Orders do S/4HANA do Sandbox encontrados no api.sap.com

    ![image](Readme-Images/41.png)

- Adicione um "Button" com o nome de "Buscar Sales Order QrCode"

  > Para adicionar o "Button", arraste-o até onde deseja colocá-lo

  ![image](Readme-Images/42.png)

- Clique em "Core", depois em "MARKETPLACE"

  ![image](Readme-Images/43.png)

- Pesquise "list", depois clique em "Icon list"

  ![image](Readme-Images/44.png)

- Clique em Install

  ![image](Readme-Images/45.png)

- Dentro de "INSTALLED", arraste "Icon list" para cima do "Button"

  ![image](Readme-Images/46.png)

### Passo 9 - Integrando os Dados de Sales Order

- Clique em "Icon list" e depois clique em "Configure"

  ![image](Readme-Images/47.png)

- Clique em "Sales Order"

  ![image](Readme-Images/48.png)

- Arraste e organize de acordo com as instruções:

  | Content  | SalesOrder       |
  |----------|------------------|
  | iconName | Clique no ícone de raio e escreva "" depois aperte em "submit" |
  | id       | SalesOrder       |
  | label    | SalesOrderType   |
  | title    | TotalNetAmount (está mais abaixo da página) |

    ![image](Readme-Images/49.png)
    ![image](Readme-Images/50.png)
    ![image](Readme-Images/51.png)

- Clique em "Properties"

  ![image](Readme-Images/52.png)

- Clique em "OPTIONAL", depois em "Pagination"

  ![image](Readme-Images/53.png)

- Clique em "Object With Properties"

  ![image](Readme-Images/54.png)

- Clique em "Page size", depois em "Static number"

  ![image](Readme-Images/55.png)
  ![image](Readme-Images/56.png)

- Defina "Page size" para 20

  ![image](Readme-Images/57.png)

- Clique em "Include total count", depois em Static true/false

  ![image](Readme-Images/58.png)
  ![image](Readme-Images/59.png)

- Clique em "Save"

  ![image](Readme-Images/60.png)

- Clique em "SAVE AND EXIT"

  ![image](Readme-Images/61.png)

### Passo 10 - Customize do seu jeito explorando as ferramentas do SAP Build Apps
