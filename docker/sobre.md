# Introdução ao Docker

Docker é uma plataforma de código aberto que permite automatizar a implantação de aplicativos dentro de containers de software. Containers são ambientes isolados e portáteis que incluem tudo o que uma aplicação precisa para ser executada, incluindo o código, bibliotecas, dependências e variáveis de ambiente. A principal vantagem de usar containers é que eles garantem que o software funcionará de maneira consistente, independentemente do ambiente onde está sendo executado.

### Por Que Usar Docker?

- **_Portabilidade:_** Containers Docker podem ser executados em qualquer sistema que tenha o Docker instalado, seja em um ambiente de desenvolvimento local, em servidores de produção ou na nuvem. Isso elimina problemas de compatibilidade entre diferentes ambientes.

- **_Isolamento:_** Cada container funciona de forma independente, isolando a aplicação e suas dependências. Isso significa que mudanças em uma aplicação ou biblioteca em um container não afetam outras aplicações que estão sendo executadas em outros containers.

- **_Eficiência:_** Diferente das máquinas virtuais, os containers compartilham o kernel do sistema operacional, o que os torna mais leves e rápidos. Isso permite a execução de muitos containers simultaneamente no mesmo host com uso mínimo de recursos.

- **_Desenvolvimento e Deploy_** Simplificados: Com Docker, você pode garantir que o ambiente de desenvolvimento seja idêntico ao de produção. Isso reduz a probabilidade de problemas relacionados ao ambiente de execução quando a aplicação é implantada.

- **_Ciclo de Desenvolvimento Acelerado:_** Docker permite que os desenvolvedores criem, testem e implantem aplicativos de forma mais rápida e confiável. Com o uso de imagens Docker, que são versões imutáveis de containers, os times de desenvolvimento podem compartilhar e distribuir o ambiente de execução de uma aplicação com facilidade.

### Conceitos Básicos do Docker

- **_Imagem Docker:_** Uma imagem Docker é um pacote leve e independente que inclui tudo que uma aplicação precisa para rodar: código, runtime, bibliotecas, e configurações. As imagens são imutáveis e podem ser versionadas, compartilhadas e reutilizadas.

- **_Container:_** Um container é uma instância de uma imagem Docker. Ele é executado de forma isolada do sistema operacional subjacente, mas ainda pode interagir com ele através de recursos controlados.

- **_Dockerfile:_** Um Dockerfile é um script de instruções para construir uma imagem Docker. Nele, você define as etapas que o Docker deve seguir para criar a imagem, como a base da imagem, a instalação de dependências, a cópia do código, e a configuração do ambiente.

- **_Docker Compose:_** Docker Compose é uma ferramenta que permite definir e gerenciar múltiplos containers como um serviço único. Com o Compose, você pode configurar sua aplicação para rodar com vários containers (como frontend, backend, banco de dados) usando um único arquivo YAML.
