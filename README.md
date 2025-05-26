
<p align="left">
    <img width="200" src="asset/iniciorapido.jpg">
</p>
<p align="left"><h1> # DIO-Azure-Databricks  </h1></p>
<p align="center"><h1>BootCamp : Azure Databricks </h1></p>


# Projeto : Criando um Monitoramento de Custos no Data Factory


 > **Objetivo:** Este é o repositório desenvolvido durante o curso BootCamp Azure Databricks na plataforma da [DIO](https://dio.me)

Projeto com o objetivo de gerar evidência do conhecimento absorvido no <b>treinamento do módulo:</b>

  ### Explorando o Recursos Azure.
Como referência usaremos o contéudo do tópico  :
* Criando os Recursos com a Estruturação de uma Infra Completa


## 💻 Tecnologias utilizadas no projeto

- [Github] 
- [Azure]

##    Desciption

Entendendo o Desafio
Agora é a sua hora de brilhar e construir um perfil de destaque na DIO! Explore todos os conceitos explorados até aqui e replique (ou melhore, porque não?) este projeto prático. Para isso, crie seu próprio repositório e aumente ainda mais seu portfólio de projetos no GitHub, o qual pode fazer toda diferença em suas entrevistas técnicas 😎

Como entregar esse projeto?
Chegou a hora de você construir um portfólio ainda mais rico e impressionar futuros recrutadores, para isso é sempre importante mostrar os resultados do seu esforço
e como você os obteve deixando claro o seu racional, para isso faça da seguinte maneira:

1. Crie um novo repositório no github com um nome a sua preferência
2. Crie um arquivo chamado readme.md;
3.    Deixe alguns prints ;
4.    Descreva o processo, alguns insights e possibilidades que você aprendeu durante o conteúdo;
5.    Após a IA analisar suas sentenças
6. Compartilhe conosco o link desse repositório através do botão 'entregar projeto'

 
## ✨ Solution

  1) Neste desafio navegamos de forma básica pela interface do Azure.
  2) Não usamos uma conta de estudande, usamos uma contra free por 30 dias.
  3) Veremos os prints de passo a passo de:

     Criação de recursos, como:

        * Grupo de Recurso
            <p> &nbsp;&nbsp;&nbsp; Dedicado ao projeto, que no caso ira demonstrar uma implementacao de arquitetura.</p>

        * Data Factory
            </p> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Contém os recursos de dados e outros que iremos manipular.
            È uma das fontes de entrada</p>
        * Events Hubs
           <p> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  Contém os recursos de dados e outros que iremos manipular.</p>
           <p> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  É uma das fontes de entrada</p>
           <p> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  Pontos de atenção e a parte de segurança e thruput </li></p>

        * Azure Databrikcs Service
          <p> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Iremos manipular os dados e gerar novos ou apenas sanitizar os dados.</p>

        * Data Lake Storage 
           <p> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Pontos importantes:</p>
           <p> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Saber o que será armazenado, pois no campo "primary service" seremos</p>
           <p> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; questionados, com isto e importante ver o que o arquiteto realmente almeja para este recurso. Para este recurso iremos criar um ADLS</p>
            <p> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  Saber o comportamento da rede e um ponto importante, como ficará disponivel o Data Lake.</p>

        * Storage Account
           <p> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Apos a criação iremos configurar:</p>
             <p> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  Controle de Acesso</p>
             <p> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  Quem tem acesso e a que e qual o nivel.</p>
             <p> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Containers ( Pastas) </p>
             <p> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Que irá descrever/informar o status dos dados armazenados. Exemplo bronze, prata, ouro. que segue a linha de um dado sem tratamento, semi tratado e tratado.</p>
             <p> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Filas</p>
             <p> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Emfim a estrutura definida pela arquitetura.</p>

        * Azure Machine Learning
            <p> &nbsp;&nbsp;&nbsp; Que ira processar os nossos dados de entrada de forma a gerar, seja insights</p>
            <p> &nbsp;&nbsp;&nbsp; ou informações relevantes.</p>

        * Kubernets Service
        * Container Apps Enviroments
        * Container Instances
        * SQL Database

    Atenção : A nossa função e de configuração do ambiente com os dados que são fornecidos pela Arquitetura.
    Nos como engenheiro de dados, iremos pegar a definição lógica da arquitetura e implementar no ambiente do Microsoft Azure.
    Iremos usar um
  4) Criação e configuração do Data Fabric
  5) Criação e configuração do Data Lake
   
  6) Criação e configuração do Data Factory
 
     Seguimos a boa pratica descrita em recomendações de abreviações
     <a href="https://learn.microsoft.com/pt-br/azure/cloud-adoption-framework/ready/azure-best-practices/resource-abbreviations" title="Recomendações de Abreviações"> 📕Clique aqui para ler</a>
      <p align="left">
       <img width="400" src="asset/3_DashboardPrincipal_ADF.jpg">
      </p>
	  
  6.1) Vamos ver agora as features do recursos Data Factory.
     Temos a tela principal com um "overview" de todas as possiveis configurações

      <p align="left">
       <img width="400" src="asset/4_adf_recursos_t1.JPG">
      </p>
	  
	 Temos o "log" de atividades.
		Demostra o que está sendo feito, passo a passo.

	  
	 Temos a "Tags" 
		Que da suporte a gestão de custos dos recursos utilizados

      <p align="left">
       <img width="400" src="asset/5_adf_recursos_t2_Tags.JPG">
      </p>
	  
	 Temos o "Monitoring"
		Que no da informações e configurações de alertas, metricas, diagnosticos e logs de acoes de monitoramento.

     Temos o "Settings"
		Aqui podemos configurar as propriedades do recurso:
		  Configuração de Rede
		  Credenciais (Manage Identies)
		  Propriedades 
			Que contem :
			Managed Identity Application ID
			Managed Identity Tenant
			Managed Identity Object ID
			Resource ID
			Resource group
			Subscription (assinatura)
			Tipo recurso e nome
			Localização
		  Locks
		    Que cria acesso ou locks para algumas funcionalidades do recurso.
      <p align="left">
       <img width="400" src="asset/6_adf_recursos_t3_Settings_Properties.JPG">
      </p>
	  
  
  14) O que vimos nesta introdução ao Microsoft Azure e como é o processo de configuração dos recursos e suas propriedades.
	 Podemos constatar a gama bem diversificada e robusta da solução de nuvem publica que e o Microsoft Azure.
	 Iremos explorar um pouco mais de configurações nas próximas atuaizações.
     
## 👨‍💻 Desenvolvedor

<p>
    <p>&nbsp&nbsp&nbspAlvaro Monteiro<br>
    &nbsp&nbsp&nbsp
    <a href="https://github.com/Alvaro-MSJR">
    GitHub</a>&nbsp;|&nbsp;
    <a href="www.linkedin.com/in/alvaro-monteiro-silva">LinkedIn</a>
&nbsp;|&nbsp;</p>
</p>
<br/><br/>
<p>

---
⌨️ conteúdo por [Alvaro Monteiro](https://github.com/Alvaro-MSJR)
