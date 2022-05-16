
![TheCodingCabin](https://user-images.githubusercontent.com/105243897/168500365-781b3c68-8832-4607-b317-313f88b51816.jpg)

⛺TheCodingCabin 👋 Vamos conhecer um pouco de Docker.

## História
Docker é um software que roda em diversos sistemas operacionais e é usado para orquestrar e gerenciar containers, o docker foi criado pela empresa Docker Inc, uma empresa de tecnologia de São Francisco.
## Instalação
Para uma instalação correta podemos usar o manual do docker dentro do [site]( https://docs.docker.com/desktop/), assim teremos a instalação de acordo com o sistema operacional.
## Contexto Geral
O Container (Docker) é como as antigas Máquinas Virtuais (VMs),  com a diferença que container é uma abstração da camada do aplicativo em pacotes o código e dependências juntos e vários containers podem  ser executados na mesma máquina e compartilhar o kernel do sistema operacional com outros containers e então cada um é executado como um processo isolado no espaço do usuário. Já as máquinas virtuais(VMs) são abstrações do hardware físico transformando um servidor em vários servidores, e cada um tem uma cópia completa de um sistema operacional.
## Imagens Docker
 Imagens no docker pode ser como definição um objeto com partes de arquivos de SO ou no mundo docker imagens são contêiners parados, já para desenvolvedores imagens podem ser representadas como classes em resumo as imagens no docker são modelos para criação de um ambiente de sua escolha, que pode ser desde um banco de dados até uma aplicação web. Algumas imagens já prontas podem ser adquiridas no [DockerHub](https://hub.docker.com/).
### Comandos (Docker Image).
| Comando                  | Função                                                                                                                                   |
| -----------------------  | -----------------------------------------------------------------------------------------------------------------------------------------|
| docker image pull        | É o comando para baixar imagens. Extraímos imagens de repositórios dentro de registros remotos. Por padrão, as imagens serão extraídas dos repositórios no Docker Hub. Este comando extrairá a imagem marcada como mais recente do repositório alpino no Docker Hub: docker image pull alpine:latest.|
| docker image ls          | Lista todas as imagens armazenadas no cache de imagem local do seu host Docker. Para ver os resumos de imagens SHA256, adicione o sinalizador --digests.|
| docker image inspect     | Fornece todos os detalhes gloriosos de uma imagem - dados de camada e metadados.|
| docker manifest inspec   | Permite inspecionar a lista de manifestos de qualquer imagem armazenada no Docker Hub.|
| docker buildx            | É um plug-in do Docker CLI que estende o Docker CLI para suportar compilações multi-arquitetura.|
| docker image rm          | é o comando para excluir imagens. Este comando mostra como excluir a imagem alpine:latest — docker image rm alpine:latest. Você não pode excluir uma imagem associada a um contêiner nos estados em execução (Ativado) ou interrompido (Sair).|
## Containers Docker 
Um contêiner é a instância de tempo de execução de uma imagem. Os contêineres compartilham o SO/kernel com o host em que estão sendo executados. Também é comum que os containers sejam baseados em imagens minimalistas que incluem apenas softwares e dependências exigidas pela aplicação.
### Comandos (Docker Container).
| Comando                  | Função                                                                                                                                   |
| -----------------------  | -----------------------------------------------------------------------------------------------------------------------------------------|
|  docker container run    | É o comando usado para iniciar novos containers. Na sua forma mais simples, aceita uma image e um comandos como argumentos. a image é usada para criar o contêiner e o comando é o aplicativo que o contêiner executará quando for iniciado.|
|  docker container ls     | Lista todos os containers no estado em execução (UP). Se você adicionar o flag -a, também verá os contêineres no estado parado (saído).|
|  docker container exec   | Executa um novo processo dentro de um container em execução. É útil para anexar o shell do seu host Docker a um terminal dentro de um contêiner em execução. Este comando iniciará um novo shell Bash dentro de um contêiner em execução e se conectará a ele: docker container exec -it <container-name or container-id> bash.|
|  docker container stop   | interromperá um contêiner em execução e o colocará no estado saiu.|
|  docker container start  | Irá iniciar um caintainer parado.|
|  docker container rm     | Excluirá um container parado. Você pode especificar contêineres por nome ou ID. É recomendável interromper um contêiner com o comando docker container stop antes de excluí-lo com docker container rm.|
|  docker container inspect| mostrará a configuração detalhada e informações de tempo de execução sobre um contêiner.|

## Tópicos Avançados.
  Ok… esse foi o resumo do resumo do Docker em um contexto geral, mas vale a pena lembrar que o docker é uma ferramenta incrível que irá fazer parte do seu dia-a-dia, no próximo tópico irei colocar algumas literaturas e vídeos de para contribuir em seu aprendizado assim como fez parte do meu. Com o Docker podemos usar comandos ou flags como (--filter, -it, -a, –format) que irá facilitar na hora de trabalhar em um ambiente empresarial, também podemos contribuir com a comunidade criando imagens docker e enviando no repositório do DockerHub. No contexto de microservicos o Docker Swarm ou o Kubernetes  facilita com a criação de uma rede de containers em que cada um terá nossos módulos de microserviços. O Docker se tornou uma ferramenta poderosa e segura facilitando na criação de chaves de segurança entre nossas redes. Conheça um pouco dessa tecnologia que está revolucionando o mundo do desenvolvimento.  

## Exemplos de imagens:
Acesse o meu [DockerHub](https://hub.docker.com/u/greatdesignersoftware).
#### Branh 01 - Desenvolvendo....
## Literaturas e Vídeos Recomandados.
Vídeos:
  [Mateus Muller](https://lnkd.in/d-uZDZmp). |
  [AmigosCode](https://lnkd.in/dz3Fb2xB). |
  [TechWorld with Nana](https://lnkd.in/dv2A5jYN). |
  [Hora de Codar](https://lnkd.in/dKiQKtyB). |
  Livros:
  [Descomplicando o Docker 2a edição](https://www.amazon.com.br/Descomplicando-Jeferson-Fernando-Noronha-Vitalino-ebook/dp/B07J1L31L4/ref=sr_1_1?__mk_pt_BR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=2L5V9HUY56J4D&keywords=docker&qid=1652710315&s=digital-text&sprefix=docker%2Cdigital-text%2C261&sr=1-1) |
  [Docker Deep Dive: Zero to Docker](https://www.amazon.com.br/Docker-Deep-English-Nigel-Poulton-ebook/dp/B01LXWQUFF/ref=sr_1_7?__mk_pt_BR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=2L5V9HUY56J4D&keywords=docker&qid=1652710315&s=digital-text&sprefix=docker%2Cdigital-text%2C261&sr=1-7) |
  [Containers com Docker: Do desenvolvimento à produção](https://www.amazon.com.br/Containers-com-Docker-desenvolvimento-produ%C3%A7%C3%A3o-ebook/dp/B019NJB50C/ref=sr_1_2?__mk_pt_BR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=2L5V9HUY56J4D&keywords=docker&qid=1652710315&s=digital-text&sprefix=docker%2Cdigital-text%2C261&sr=1-2) |

