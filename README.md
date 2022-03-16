# Gerador de Senhas

Esse código foi desenvolvido junto com o curso segurança da informação com python da escola Digital Innovation One.

Tentarei criar uma pagina na web para disponibilizar para as pessoas que quiserem criar uma senha segura.

## Explicando o código linha a linha

 `import random, string`

Importa o módulo `random` que implementa geradores de números pseudoaleatórios para várias distribuições. E o módulo `string` para manipulação de strings

`tamanho = int(input("Digite o tamanho de senha que você deseja: " ))`

Pede para o usuário entrar com a quantidade de números inteiros para criar sua senha.

`chars = string.ascii_letters + string.digits + '<>ç!@#$%():_=*&%?'`

Esse método envolve o `uppercase` e o `lowercase` gerando caracteres maiúsculos e minúsculos
`rnd = random.SystemRandom() os.urandom` gera números aleatórios a partir do sistema operacional

`print("".join(rnd.choice(chars) for i in range(tamanho)))`

O `método join()` é um método de string e retorna uma string na qual os elementos da sequência foram unidos por um separador str.
`rnd.choice` gera uma lista com caracteres randômicos
