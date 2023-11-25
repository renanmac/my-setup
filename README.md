# Setup de desenvolvimento

O objetivo desse repositório é te ajudar a configurar seu ambiente de desenvolvimento :)

Para isso, utilizaremos o `Ansible`, essa ferramenta será responsável por aplicar todas as 
configurações necessárias para a implementação do seu ambiente.

Vamos lá?

## Guia

1 - Para começar, vamos atualizar seus pacotes:

```bash
$ sudo apt update
$ sudo apt upgrade -y
```

2 - Em seguida, vamos instalar o ansible:

```bash
$ sudo apt install ansible
```


3 - Pronto, agora é só executar o ansible e ele vai cuidar de tudo :)
```bash
$ ansible-playbook playbook.yml -i localhost
```

## Modo Vagrant

1 - Inicialize a máquina virtual:

```bash
$ vagrant up
```

2 - Certifique-se de que o path da sua chave ssh está correto no arquivo `vagrant`:

3 - Execute o ansible:

```bash
$ ansible-playbook playbook.yml -i vagrant

```

Agora o seu ambiente está pronto! É hora de mergulhar nos projetos e começar a codar :)