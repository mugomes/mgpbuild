# MGPBuild

Com este script, você pode compilar o PHP e gerar um AppImage que inclui todas as dependências necessárias para sua execução. Assim, você poderá rodar o PHP em qualquer distribuição Linux e em qualquer versão compatível com AppImage.

Recursos

- Baixa e verifica o hash do PHP
- Compila o PHP com várias extensões
- Cria o AppImage com todas as dependências necessárias para sua execução

## Requerimento

- Linux Debian 12 ou superior de 64 bits com sudo ativado
- Linux Ubuntu 22.04 ou superior de 64 bits

## Instalação

Extraia os arquivos em uma pasta chamada mgpbuild, abra o terminal e digite os seguintes comandos:

```
chmod +x mgpbuild
./mgpbuild
```

- Pressione a tecla 8 para instalar as dependências necessárias para o PHP
- Após a instalação pressione a tecla 6 para instalar o MGPDesktop
- Após a instalação pressione a tecla 7 para instalar o linuxdeploy e o appimagetool

Agora com tudo instalado é só pressionar a tecla 9 para sair.

## Usando o MGPBuild

Para usar o script é bem simples, crie uma pasta chamada php, abra a pasta no terminal, agora use o comando abaixo.

```
mgpbuild
```

### Baixando o PHP

Para baixar o PHP, acesse o site oficial do PHP, anote a versão e o hash do arquivo tar.gz mais recente.

- No MGPBuild pressione a tecla 1
- Digite ou cole a versão do PHP e pressione ENTER
- Digite ou cole o hash do PHP e pressione ENTER

Após o download, o MGPBuild irá verificar se o hash do arquivo baixado é igual ao hash informado, se for, exibirá "Hash correto!". Caso exiba "Hash incorreto", faça o procedimento novamente.

### Compilando o PHP

Após baixado e verificado o hash do PHP, agora é hora de compilar, para isso siga o passo a passo abaixo.

- Pressione a tecla 2
- Digite ou cole a versão do PHP e pressione ENTER

### Gerando o AppImage

- Pressione a tecla 3 para criar o AppRun, o arquivo desktop e uma imagem padrão para o ícone
- Pressione a tecla 4 para que o linuxdeploy possa obter todas as bibliotecas necessárias para funcionar corretamente o PHP e suas extensões
- Pressione a tecla 5 para criar o AppImage

### Perguntas Frequentes

#### O nome da máquina e a versão do Kernel ficam visíveis após a compilação?

Não. O MGPBuild irá remover o nome de sua máquina e a versão do Kernel do PHP e substituirá pela informação "Linux".

#### No computador que irei utilizar o PHP, preciso ter alguma dependência instalada? Exemplo libonig5?

Não. O MGPBuild utiliza o linuxdeploy para obter todas as bibliotecas necessárias para funcionar corretamente o PHP e suas extensões e armazena dentro do AppImage. Também é utilizado o export LD_LIBRARY_PATH para que ao executar o AppImage seja obtido as dependências do PHP de dentro do AppImage.

#### Ao compilar o PHP manualmente algumas bibliotecas requerem a mesma versão da máquina de compilação, isso acontece também ao compilar usando o MGPBuild?

Não. O MGPBuild gera um AppImage usando o linuxdeploy e o appimagetool com todas as dependências necessárias já inclusas no AppImage.

# Doação

Se você puder ajudar esse projeto financeiramente, vou deixar formas de apoio abaixo.

 - PIX: pixmugomes@gmail.com
 - Asaas: https://www.asaas.com/c/72mxu6ilkis5rwxz

# License

The MGPBuild is provided under:

[SPDX-License-Identifier: MIT](https://spdx.org/licenses/MIT.html)

Licensed under the MIT license.
