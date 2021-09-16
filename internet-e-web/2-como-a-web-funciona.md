## Como a web funciona 



Você já se perguntou ou teve curiosidade em saber o que acontece por trás das cortinas quando você acessa um site pelo navegador ? Eu tentarei mostrar de uma forma simplificada e resumida o que acontece.

leia o texto no qual me baseei e retirei a maioria dos exemplos: [how the web works - mdn docs](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works)  


<details>
 <summary>tipos de computadores 🖥️ </summary>
<br>
Em uma rede de computadores existem diferentes tipos de dispositivos de acordo com a função que eles exercem na rede. Os dois principais são:

* **Clientes**: são os dispositivos que consomem arquivos e serviços presentes em uma rede. Exemplo: computadores de usuários comuns conectados a internet e que acessam um website através do navegador.
* **Servidores**: computadores que fornecem arquivos e serviços web para clientes. Os servidores costumam ser dispositivos com hardware mais robusto com grande capacidade de processamento e memória.  Exemplo: cliente requisita acesso a um website e o servidor envia ao cliente uma copia do site para a maquina local do cliente e assim, a página pode ser exibida pelo navegador.



<div align="center"><img src="./images/cliente-servidor.png" alt="a esquerda simbolo de dois computadores que representam os clientes. Desses símbolos sai uma seta apontando para a direita e escrito requisições. A direita da imagem esta um simbolo de nuvem que representa o servidor. Desse símbolo sai uma seta apontando para a esquerda e escrito respostas." width="650px"></div>

</details>

<details>
 <summary>Outros personagens 🚻 </summary>
<br>

 Além de clientes e servidores existem outros serviços que possibilitam a pesquisa de um site através de um navegador. Imagine a web como uma rua, em uma das pontas fica sua casa e na outro ponta está um shopping onde você deseja fazer compras. Abaixo são apresentados alguns outros serviços que possibilitam essa tarefa/metáfora:

* **Conexão com a Internet** : permiti o trânsito de dados e pacotes, semelhante a rua entre sua casa e o shopping.

* **TCP/IP**: são protocolos de comunicação que determinam a forma como dados e pacotes são encaminhados. Na nossa metáfora seria como escolher ir à pé ou  de carro até o shopping.

* **DNS**: Domain Name Server é um protocolo que se assemelha a um livro de endereços para websites. Quando pesquisamos por um site no navegador, inserimos o domínio(nome) do site, no entanto o navegador não sabe localizar o servidor, onde está armazenado o website, através do nome. Para isso, é necessário o endereço ip do servidor. O papel do DNS é associar esse domínios aos respectivos endereços IPs.

* **HTTP:** Hypertext Transfer Protocol é um protocolo de aplicação. Ele funciona como uma linguagem auxiliando a troca de arquivos multimídias entre o servidor e o cliente.  É como se fosse a linguagem que você usa para se comunicar com o vendedor de uma loja. 

* **Websites:** Sites são feitos por tipos de arquivos. Os dois principais tipos são:

  * arquivos de código: Websites são fundamentalmente construídos por arquivos HTML, CSS e Javascript.

  * assets : todos outros arquivos que compõem um website, como por exemplo: Imagem, vídeos , PDFs, documento Word e etc.

</details>


<details>
<summary>O fluxo do Website ➡️ </summary>
<br>
 O passo-a-passo  quando um site é pesquisado no navegador:



1. O navegador vai até o servidor DNS e pergunta qual é o real endereço ip do domínio que foi pesquisado. Isso é necessário, para que o navegador siaba em qual servidor o website está armazenado.
2. O navegador envia uma requisição HTTP ao servidor , pedindo uma cópia do website para o cliente.
3. Se o servidor aprovar a requisição do cliente , ele enviará uma mensagem com status de : "200 Ok", que significa "Ok, aqui está a cópia do website que vc precisa" . A partir daí os arquivos do site são enviados através de pequenos pedaços chamados de pacotes de dados.
4. O navegador reúne esse pequenos pedaços e carrega o website completo para que você possa visualizar.



<div align="center"><img src="./images/requisitar-website.png"></div>

​																		(imagem retirada do site : [amazon](https://aws.amazon.com/pt/route53/what-is-dns/))



Este foi um breve resumo dos atores/serviços envolvidos na requisição de um website
</details>
