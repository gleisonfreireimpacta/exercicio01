# exercicio01
Exercicio aula 2

# Etapa a
# Cria um arquivo 'arquivo.txt' com o conteúdo '01'
echo "01" > arquivo.txt

# Etapa b
# Adiciona 'arquivo.txt' ao staging e verifica o status
git add arquivo.txt
echo "Status após adicionar arquivo.txt ao staging:"
git status

# Etapa c
# Faz o commit do arquivo com a descrição fornecida
git commit -m "git add example - arquivo.txt"
echo "Log após o commit:"
git log --oneline

# Etapa d
# Sobrescreve o conteúdo de 'arquivo.txt' com '02'
echo "02" > arquivo.txt

# Etapa e
# Verifica as diferenças entre o conteúdo atual e o commit anterior
echo "Diffing após sobrescrever com 02:"
git diff arquivo.txt

# Etapa f
# Adiciona 'arquivo.txt' novamente ao staging e verifica o status
git add arquivo.txt
echo "Status após adicionar novamente arquivo.txt ao staging:"
git status

# Etapa g
# Verifica as diferenças entre o conteúdo atual e o staging
echo "Diffing após adicionar ao staging:"
git diff --staged

# Etapa h
# Sobrescreve o conteúdo de 'arquivo.txt' com '03'
echo "03" > arquivo.txt

# Etapa i
# Verifica as diferenças entre o conteúdo atual e o staging
echo "Diffing após sobrescrever com 03:"
git diff arquivo.txt

# Etapa j
# Faz o restore do arquivo da área de staging e verifica o status
git restore --staged arquivo.txt
echo "Status após restore do arquivo da área de staging:"
git status

# Etapa k
# Adiciona 'arquivo.txt' novamente ao staging e verifica o status
git add arquivo.txt
# Realiza o commit do arquivo e verifica o log
git commit -m "Update arquivo.txt to version 03"
echo "Log após o commit:"
git log --oneline

# Etapa l
# Adiciona um arquivo .gitignore com o conteúdo '*.txt'
echo "*.txt" > .gitignore

# Etapa m
# Cria um novo arquivo 'novo.txt' e verifica o status
echo "Novo arquivo criado" > novo.txt
echo "Status após criar novo.txt:"
git status
