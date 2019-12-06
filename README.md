# Publicando Imagem Laravel 
<h2>by code Education </h2> 
<hr/>

<h3>Tarefa 1</h3>

Configurar um ambiente Laravel utilizando o docker-compose com:
<ul>
<li>Nginx</li>
<li>PHP-FPM</li>
<li>Redis</li>
<li>MySQL</li>
</ul>
<p>Lembrando que o volume do código fonte deve ser compartilhado com a App. </p>
<p>Após realizarmos a clonagem do repositório e executarmos: docker-compose up -d, 
poderemos ver a aplicação Laravel rodando com o erro de autoload na porta: 8000, 
uma vez que o docker-compose não executou o composer install do PHP, logo, não se
preocupe com tal detalhe nesse momento. </p>

<h3>Tarefa 2 </h3> 

<p>Após ter tido sucesso na etapa anterior, faça a configuração do framework Laravel 
seguindo as etapas (dentro do container):</p>
<ul>
<li>execute composer install</li>
<li>crie o arquivo .env baseado no .env.example </li>
<li>execute: php artisan key:generate </li>
<li>execute: php artisan migrate </li>
</ul>

<p>Nesse momento, quando você acessar a aplicação no browser, finalmente, você deverá ver 
a página inicial do Laravel funcionando. </p>

<p>Baseado nessas últimas ações, gere o build da imagem desse container e faça a 
publicação em sua conta no Hub do Docker. Lembre-se: Ao gerar o build da imagem, 
TODO o conteúdo incluindo arquivos como vendor, .env, etc deverão ser incluídos. 
Adicione o endereço da imagem no seu dockerhub no README.md e faça o commit para 
um repositório público do Github. Arquivos e códigos úteis para auxiliar no exercício
incluindo nginx.conf e linha de comando para baixar o composer.</p>
<hr/>

#### Para acessar a imagem criada no docker hub gerada a partir da resolução deste exercício <a href="https://hub.docker.com/r/josimar1000/laravel"> clique aqui. </a>
