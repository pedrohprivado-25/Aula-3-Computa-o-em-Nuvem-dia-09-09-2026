# Aula 3 – Computação em Nuvem

Nesta aula estudamos os **modelos de implantação em computação em nuvem** e vimos as principais diferenças entre **nuvem pública, privada e híbrida**.

Além da parte teórica, também fizemos uma atividade prática utilizando o **Killercoda**, o terminal Linux e o Python para criar e testar um servidor HTTP.

## Conteúdo da aula

Durante a aula, foram apresentados três modelos principais de implantação:

* **Nuvem Pública:** os recursos são disponibilizados por um provedor de nuvem e podem ser utilizados por diferentes clientes.
* **Nuvem Privada:** a infraestrutura é destinada a uma única organização, permitindo maior controle sobre os dados e recursos.
* **Nuvem Híbrida:** combina recursos de uma nuvem pública com uma nuvem privada.

Também vimos que a escolha do modelo depende de fatores como **segurança, custo, desempenho, escalabilidade, privacidade e disponibilidade**.

## Atividade prática

Na parte prática, utilizamos o ambiente do Killercoda para criar uma página HTML e executar um servidor Web utilizando o Python.

Primeiro criei uma pasta chamada `aula3` e dentro dela o arquivo `index.html`.

Depois iniciei o servidor com:

```bash
python3 -m http.server 8080
```

O servidor ficou disponível na porta **8080**.

Para testar se estava funcionando, utilizei:

```bash
curl localhost:8080
```

Com isso consegui visualizar no terminal o conteúdo da página HTML que estava sendo servida pelo Python.

## Desafio 1

No primeiro desafio, foi necessário parar o servidor, alterar o arquivo `index.html` e adicionar algumas informações sobre o aluno e a aula.

Foram adicionadas as seguintes informações:

```html
<p>Aluno: Pedro Henrique</p>
<p>Aula 3 - Modelos de Implantacao</p>
```

Depois iniciei novamente o servidor e utilizei o `curl` para verificar se as alterações estavam aparecendo corretamente.

## Desafio 2

No segundo desafio, utilizei alguns comandos do Linux para identificar informações sobre o ambiente utilizado na atividade.

Com o comando:

```bash
hostname
```

foi possível verificar o nome da máquina, que era `ubuntu`.

Também utilizei:

```bash
hostname -I
```

para verificar os endereços IP disponíveis no ambiente.

O arquivo `index.html` estava localizado em:

```text
/root/aula3/index.html
```

O servidor Web estava sendo executado na porta:

```text
8080
```

Não foi necessário instalar o Apache ou o Nginx, pois utilizamos o próprio módulo `http.server` disponível no Python.

## Desafio final – Arquitetos da Nuvem

No desafio final, foi proposta uma situação envolvendo uma universidade que precisava definir onde seus sistemas deveriam ser hospedados.

A solução que desenvolvi foi uma **arquitetura híbrida**, utilizando a nuvem pública para os sistemas que precisam atender muitos usuários e ter acesso mais fácil, e a nuvem privada para informações que precisam de maior controle e segurança.

### Nuvem pública

Coloquei na nuvem pública:

* Portal institucional
* Ambiente do aluno
* Biblioteca digital

Esses sistemas podem ter muitos acessos e precisam estar disponíveis para os usuários em diferentes locais.

### Nuvem privada

Coloquei na nuvem privada:

* Sistema financeiro
* Dados pessoais dos estudantes
* Sistema interno dos professores

Esses sistemas trabalham com informações mais restritas, por isso considerei mais adequado utilizar uma estrutura privada, com maior controle de acesso e segurança.

## O que eu aprendi

Nesta aula consegui entender melhor a diferença entre **nuvem pública, privada e híbrida** e em quais situações cada uma pode ser utilizada.

Na atividade prática também consegui colocar alguns conceitos em prática, principalmente criando um servidor Web com Python, trabalhando com arquivos HTML e fazendo requisições pelo terminal usando o `curl`.

O desafio final também ajudou a entender que não existe um único modelo de nuvem que seja melhor para todos os casos. A escolha depende do tipo de sistema e das necessidades da organização.

## Arquivos desta aula

Neste repositório estão os arquivos que desenvolvi e utilizei durante a Aula 3:

* `ATIVIDADE PRATICA - AULA 3`
* `AULA 3 - COMPUTAÇÃO EM NUVEM - DESAFIO`
* `DESAFIO FINAL – ARQUITETOS DA NUVEM`

## Resumo

A Aula 3 foi focada em **Computação em Nuvem e modelos de implantação**. Além da parte teórica, tivemos uma atividade prática com Linux, HTML, Python e HTTP, e no desafio final desenvolvi uma proposta de arquitetura híbrida para uma universidade.
