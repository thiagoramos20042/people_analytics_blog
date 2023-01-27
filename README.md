![alt text](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT52Sh9RSf6v2hOEAR5gg_hFMDpRE0Y2Y8EmA&usqp=CAU)

# Como o People Analytics e o Machine Learning estão transformando a gestão de pessoas
People analytics é o uso de dados e análises para entender e melhorar o desempenho e o envolvimento dos funcionários. Isso inclui coletar e analisar dados sobre as habilidades, o desempenho, a satisfação e a rotatividade dos funcionários, bem como dados de recrutamento, treinamento e benefícios. A análise de pessoas permite que as empresas tomem decisões baseadas em dados para melhorar o desempenho e a eficiência, retenção de talentos e satisfação dos funcionários.
Análise de dados é o processo de coletar, limpar, transformar e analisar dados para obter insights e tomar decisões informadas. É uma habilidade crítica em um mundo cada vez mais voltado para dados e é usado em uma variedade de setores, incluindo finanças, saúde, varejo e tecnologia.

Machine learning é uma subárea da inteligência artificial que permite que as máquinas aprendam com os dados sem serem explicitamente programadas. Isso é possível graças a algoritmos de aprendizado automático que são capazes de identificar padrões e tendências nos dados e usá-los para tomar decisões e prever resultados.
People analytics combina essas três áreas para fornecer insights valiosos sobre os funcionários de uma organização. Por exemplo, as empresas podem usar dados de ponto eletrônico, e-mails e mensagens instantâneas para entender como os funcionários passam o seu tempo e identificar quais equipes e indivíduos são mais produtivos. Além disso, as empresas podem usar dados de feedback e avaliações de desempenho para entender como os funcionários se sentem em relação à empresa e ao seu trabalho.
A análise de dados também pode ser usada para identificar tendências e padrões em dados demográficos, como idade, gênero e localização, para entender como esses fatores afetam o desempenho e a satisfação dos funcionários. Além disso, as empresas podem usar dados de turnover para entender por que os funcionários estão deixando a empresa e como evitar futuras perdas de talentos.

No entanto, é importante lembrar que a análise de dados e o machine learning só são valiosos se as empresas sabem como interpretar e agir sobre os insights gerados. É importante ter uma equipe de especialistas em people analytics e machine learning para garantir que os dados sejam coletados, armazenados e analisados ​​de maneira adequada, e que as informações sejam compartilhadas e aplicadas de maneira eficaz.

Em resumo, people analytics é uma área em rápido crescimento que permite que as empresas entendam e melhorem o desempenho e a satisfação dos funcionários. A análise de dados e o machine learning são ferramentas valiosas para fornecer insights e automatizar tarefas, mas é importante ter uma equipe especializada para garantir que os dados sejam coletados e analisados ​​de maneira adequada e que as informações sejam aplicadas eficazmente.
Objetivo do projeto

# Objetivo
Construir uma automatização em python que colete informações do site https://www.myhrfuture.com/blog e as encaminhe para o meu e-mail, com os artigos relacionados ao tema people analytics.

# Explicando o código 
Este código cria uma automatização para coletar dados do site "https://www.myhrfuture.com/blog" e enviá-los por e-mail. Ele faz uso de duas bibliotecas externas: requests e BeautifulSoup.

A biblioteca requests é usada para fazer a requisição HTTP para o site especificado. A resposta dessa requisição é então passada para a biblioteca BeautifulSoup, que é usada para extrair informações específicas da página HTML.

O código começa fazendo uma requisição para a página "https://www.myhrfuture.com/blog" e passando o conteúdo da resposta para o objeto BeautifulSoup. 
Ele então usa o método "find_all" para encontrar todos os elementos "a" com a classe "BlogList-item-title" na página. Esses elementos representam links para artigos no blog.
Para cada link encontrado, o código extrai o título do artigo (texto dentro do elemento "a") e o endereço do link (atributo "href"). Ele então adiciona essas informações a uma lista (output) e junta todas as informações em uma string.

Após isso, o código usa o módulo smtplib para conectar ao servidor de e-mail do remetente, fazer login com suas credenciais, preparar a mensagem (com o conteúdo da variável output) e enviar a mensagem para o e-mail destinatário. Por fim, ele fecha a conexão com o servidor de e-mail.

# Projeto final
Receber um email com o título e link correspondente a cada matéria.
![alt text](https://github.com/thiagoramos20042/people_analytics_blog/blob/main/Captura%20de%20tela%202023-01-27%20143530.png)



