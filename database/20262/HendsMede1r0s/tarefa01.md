# Q1 - Descreva o que é um Banco de Dados e o que é um Sistema Gerenciador de Banco de Dados. Cite exemplos de Bancos de Dados e seus SGBDs.

* Um __Banco de Dados__ é um lugar onde é armazenados dados e informações com um certo propósito.
* Já o __Sistema Gerenciador de Banco de Dados__ é um sistema onde pegamos o banco de dados e fazemos operações de CRUD, como cadastrar, visualizar, excluir ou editar alguma informação do banco de dados.
* Um exemplo de como os dois trabalham juntos pode ser um banco. Cada banco tem sua base de dados de seus clientes, ou seja, suas informações, como seu cpf, nome, contato, senhas, etc. Todas essas informações são guardadas num banco de dados, e com ajuda dos SGBDs os funcionários do banco podem cadastrar um cliente novo ao banco de dados, puxar informações específicas, mudar algum dado de alguém, ou excluir alguma informação do BD.e para fazer esses procesos podem ser usados MySQL, Oracle e outros.



# Q2. Quais os principais problemas de utilizar Sistemas de Arquivos para armazenagem de dados?

* Em um sistemas de arquivo comum, podendo ser sistemas físicos ou digitais, há um grande perigo quando estamos falando de admnistrar esses dados que lá estão nesses sistemas. Pois não há nenhum tipo de proibição ou limite para quem esteja usando, ou seja, uma pessoa pode mexer no que quiser e pode acabar sem querer fazendo operações que danifiquem uma ou mais informação, como a exclusão de informações importantes, adição de informações repetidas e maior probabilidade de corromper os dados que estão naqueles arquivos. Os dados não são protegidos da mesma forma que um Banco de Dados é. Além da baixa proteção dos dados, o Sistema de Arquivos é muitas vezes mais lento que os BDs, pois é tudo feito manualmente, você próprio deve ir no diretório e adicionar linha por linha, caso você esteja cadastrando muitas coisas ao mesmo tempo, isso se tornará muito desgastante, e nada fácil.