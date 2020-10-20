# Github

-------------------------------------Utilizando o vim--------------------------------------------
No vim aperta "i" para inserir/alterar

Para sair deve apertar "esc" e digitar ":wq"


------------a
Caso arquivo ja tenha sido adicionado uma vez pode fazer a inserção direto no commit utilizando 
$ git commit -am ""
E n apenas git commit -m ""

-------------------------------------Visualizando Logs-------------------------------------------
$ git log //Mostra o commit, com sua data, autor, identificação

$ git log --decorate  //mostra mais informações 

$ git log --author="Vitor" //Vai mostrar todas as alterações que o "Vitor" fez

$ git shorlog //mostra quantas commits cada autor fez e quais foram

$ git shortlog -sn //mostra apenas a quantidade de commits e a pessoa

$ git log --graphic //mostra em graficos

$ git show "identificação" //mostra várias informações

--------------------------------------Diff--------------------------------------------------------
$ git diff //ver exatamente o que foi modificado
$ git diff --name-only //mostra apenas o nome dos arquivos modificados

--------------------------------------Desfazendo Coisas-------------------------------------------
Caso n queira fazer a mudança digitar
$ git checkout Readme.md
E o arquivo voltará para sua versão anterior

Caso ja tenha adicionado só faltando comitar e deseja voltar
$ git reset HEAD Readme.md
Volta para o ponteiro q já está tirando ele 

Caso queira voltar o arquivo, voltando o commit
SEMPRE ESCOLHE UM COMMIT ANTES DO Q SE DESEJA APAGAR
$ git reset --soft // Vai voltar com a modificação pronta para ser comitada
$ git reset --mixed // Volta aos arquivos modified sem ainda ser adicionado
$ git reset --hard // Apaga tudo q foi feito no commit
