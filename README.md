# Estudo de caso

Cenário: Por falta de maiores detalhes, presumo que o cliente tem um datalake na plataforma GCP onde ele faz o upload de seus arquivos para pasta Dados Originais. Eu vou ler esse arquivo do datalake e fazer as análises e alterações que forem necessárias e, por fim, gravar o novo arquivo na pasta Dados Tratados. Acredito que, pelas colunas das tabelas, essas tabelas sejam apenas uma view de uma parte do banco do ERP do cliente.

Ferramentas utilizadas:
MySQL na plataforma GCP: Banco utilizado para consumir as tabelas tratadas do cliente.
Bucket na plataforma GCP: Datalake onde o cliente deve colocar seus dados
DBeaver: Aplicativo para gerenciamento de banco Pode ser obtido em ( https://dbeaver.io/download/ )
Google Colab: serviço em nuvem para programar

Para entender as tabelas e como elas se relacionam, você deve primeiro executar o colab Analise_Rox. A análise consiste em identificar se existe e quais são as Primary Key e Foreing Key e o relacionamento entre as tabelas. Verificar se as colunas estão devidamente formatadas. A modelagem do banco pode ser visto neste colab.

Após a Análise você deve executar o colab Banco_ROX. Neste colab você vai encontrara todas as funções necessárias para criar o banco, criar, popular, alterar e consultar as tabelas. Todas as consultas exigidas estão nesse colab.

Após a inserção dos dados no banco, fiz o download do DBeaver, conectei no banco criado e fiz as mesmas consultas.
