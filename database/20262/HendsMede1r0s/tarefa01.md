# Q1 - Descreva o que é um Banco de Dados e o que é um Sistema Gerenciador de Banco de Dados. Cite exemplos de Bancos de Dados e seus SGBDs.

* Um __Banco de Dados__ é um lugar onde é armazenados dados e informações com um certo propósito.
* Já o __Sistema Gerenciador de Banco de Dados__ é um sistema onde pegamos o banco de dados e fazemos operações de CRUD, como cadastrar, visualizar, excluir ou editar alguma informação do banco de dados.
* Um exemplo de como os dois trabalham juntos pode ser um banco. Cada banco tem sua base de dados de seus clientes, ou seja, suas informações, como seu cpf, nome, contato, senhas, etc. Todas essas informações são guardadas num banco de dados, e com ajuda dos SGBDs os funcionários do banco podem cadastrar um cliente novo ao banco de dados, puxar informações específicas, mudar algum dado de alguém, ou excluir alguma informação do BD.e para fazer esses procesos podem ser usados MySQL, Oracle e outros.



# Q2. Quais os principais problemas de utilizar Sistemas de Arquivos para armazenagem de dados?

* Em um sistemas de arquivo comum, podendo ser sistemas físicos ou digitais, há um grande perigo quando estamos falando de admnistrar esses dados que lá estão nesses sistemas. Pois não há nenhum tipo de proibição ou limite para quem esteja usando, ou seja, uma pessoa pode mexer no que quiser e pode acabar sem querer fazendo operações que danifiquem uma ou mais informação, como a exclusão de informações importantes, adição de informações repetidas e maior probabilidade de corromper os dados que estão naqueles arquivos. Os dados não são protegidos da mesma forma que um Banco de Dados é. Além da baixa proteção dos dados, o Sistema de Arquivos é muitas vezes mais lento que os BDs, pois é tudo feito manualmente, você próprio deve ir no diretório e adicionar linha por linha, caso você esteja cadastrando muitas coisas ao mesmo tempo, isso se tornará muito desgastante, e nada fácil.

# Q3. Explique as propriedades ACID: atomicidade, consistência, isolamento e durabilidade. Para cada propriedade, descreva um exemplo prático no contexto de uma transferência bancária e explique o que aconteceria se o SGBD não garantisse essa propriedade.

1. __Atomicidade:__ A atomicidade diz que uma operação ou processo só poderá ser finalizada e completa caso nenhum erro aconteça durante. se qualquer erro acontece, o processo será cancelado, e o funcionária terá que refazer a operação para que os dados e informações do BD não sejam corrompidos. Sem a atomicidade os dados seriam corrompidos 
    * __Ex:__ Em um aplicativo de banco, caso um cliente vá fazer um pix, e a internet caia durante a transação, ou o QR-code do pix expira, essa transação será obrigatoriamente cancelada e desfeita. O cliente terá que refazer o pix.

2. __Consistência:__ São as regras dos bancos de dados, cada um tem suas próprias regras que devem ser respeitadas, caso não sejam, a operação é desfeita ou cancelada. Sem essa concistência de regras dados errados ou faltantes entrariam no armazenamneto do banco de dados gerando confusões futuras. 
    * __Ex:__ Se um cliente, em seu cadastro no sistema bancário, não colocar algum dado obrigatório, como cpf, ou pôr um número, sem querer, em algum dado que só pode ter letras, como no nome, o sistema vai dar erro, pedir para ele digitar novamente e corrigir o erro ou desfazer o processo. 

3. __Isolamento:__ Dita que um processo feito ao mesmo tempo por mais de um usuário, deve ser feita isoladamente, sem ter nenhum cruzamento entre elas, evitando a corrupção dos dados. Se são feitas várias operações o sistema deve trata-las como se elas estivessem sendo feitas separadamente, sem mistura-las em momento algum.
    * __Ex:__ Quando vários clientes fazem transações ao mesmo tempo, o sistema isola cada uma para que nenhuma cruze com a outra, sendo possivel vários clientes diferentes fazeram transações em paralelo sem nenhum erro.

4. __Durabilidade:__ Os processos feitos com os dados e informações do banco de dados, se feitos sem nenhum problema, são salvos pra sempre no banco de dados. e mesmo, que depois, ocorra problema de internet ou energia, os dados continuarão salvos no BD. Sem ter o perigo de perda. Sem essa durabilidade, dados e informações importantes seriam perdidos. 
    * __Ex:__ Caso o cliente faça uma transação, e essa transação for completa, o sistema vai cadastrar uma nova transação, no histórico de transações linkada ao perfil daquela pessoa, no banco dados onde esse pagamento do cliente será salvo permanentemente no armazenamento do BD, e mesmo que ocorra erros futuros, esse dado continuará lá sem ser corrompido.
