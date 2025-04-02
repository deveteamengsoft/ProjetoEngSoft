<h2><a href= "https://www.mackenzie.br">Universidade Presbiteriana Mackenzie</a></h2>
<h3><a href= "https://www.mackenzie.br/graduacao/sao-paulo-higienopolis/sistemas-de-informacao">Sistemas de Informação</a></h3>


<font size="+12"><center>
*&lt;Sistema de Gestão para a Farmácia Vida Saudável&gt;*
</center></font>

>*Observação 1: A estrutura inicial deste documento é só um exemplo. O seu grupo deverá alterar esta estrutura de acordo com o que está sendo solicitado na disciplina.*

>*Observação 2: O índice abaixo não precisa ser editado se você utilizar o Visual Studio Code com a extensão **Markdown All in One**. Essa extensão atualiza o índice automaticamente quando o arquivo é salvo.*

**Conteúdo**

- [Autores](#nome-alunos)
- [Descrição do Projeto](#introdução-do-projeto)
- [Análise de Requisitos Funcionais e Não-Fucionais](#descrição-dos-requisitos)
- [Diagrama de Atividades](#diagrama-de-atividades) 
- [Diagrama de Casos de Uso](#diagrama-de-comportamento-atores)
- [Descrição dos Casos de Uso](#descrição-das-funcões)
- [Diagrama de Senquencia](#diagrama-de-ordem-interações)
- [Diagrama de Classes](#diagrama-orientado-objetos)
- [Diagrama de Estados](#diagrama-estrutura-componente)
- [Diagrama de Implantação](#diagrama-de-hardware-software)
- [Referências](#referências)


# Autores

* Gustavo Braz Frainer - RA: 10386596
* Melissa Rodrigues - RA: 10726749
* Pedro Oficiati - RA: 10723732


# Descrição do Projeto

<p>A Farmácia Vida Saudável é um estabelecimento de pequeno porte localizado
na cidade de Santos-SP. Nos últimos meses, houve o crescimento da
clientela e à necessidade de maior controle sobre seus processos
internos, sendo assim, o proprietário, Sr. Boticário, decidiu modernizar
a farmácia e implementar um sistema informatizado para gestão de vendas,
estoque e clientes.</p>
<br>
<p>Atualmente, a farmácia opera de forma manual, registrando pedidos em
cadernos e utilizando planilhas para controlar o estoque. Isto tem
causado problemas como erros no controle de medicamentos, falta de
registro de clientes e dificuldades na gestão financeira.</p>
<br>
<p>O Sr. Boticário contratou a nossa empresa de desenvolvimento - MACK
Solutions SW - para criar um sistema que otimize a operação da farmácia.
Ele espera um sistema simples e eficiente que facilite as operações
diárias dos funcionários, garantindo maior precisão e rapidez no
atendimento.</p>

# Análise de Requisitos Funcionais e Não-Funcionais
<h3>1. Requisitos Funcionais</h3>
<br>
<h4>Cadastro de Produtos</h4>
<ul>
  <li>O sistema deve permitir que novos produtos e medicamentos sejam cadastrados.</li>
  <li>Cada produto deve ter informações como nome, fabricante, lote, validade, quantidade e preço.</li>
</ul>
<br>
<h4>Cadastro de Clientes</h4>
<h6>Deve ser possível registrar os clientes da farmácia, com informações como:</h6>
<ul>
  <li>Nome</li>
  <li>CPF</li>
  <li>Telefone</li>
  <li>Histórico de compras</li>
</ul>
<br>
<h4>Vendas</h4>
<ul>
  <li>O atendente precisa conseguir pesquisar se o medicamento está disponível no estoque.</li>
  <li>O sistema deve permitir registrar uma venda, vinculando-a ao cliente.</li>
  <li>Assim que a venda for finalizada, o sistema deve gerar um cupom fiscal.</li>
  <li>O estoque precisa ser atualizado automaticamente.</li>
</ul>
<br>
<h4>Controle de Estoque</h4>
<ul>
  <li>Sempre que um produto for vendido, o sistema deve diminuir a quantidade disponível.</li>
  <li>Caso o estoque de um produto esteja baixo, o sistema precisa avisar.</li>
  <li>O administrador deve conseguir visualizar os produtos disponíveis e seus status.</li>
</ul>
<br>
<h4>Relatórios</h4>
<h6>O sistema deve gerar relatórios para ajudar na gestão da farmácia, como:</h6>
<ul>
  <li>Vendas feitas no dia, na semana e no mês.</li>
  <li>Lista dos produtos mais vendidos.</li>
  <li>Clientes que compram com mais frequência.</li>
</ul>
<br>
<h4>Acesso ao Sistema</h4>
<h6>O sistema deve ter login para garantir que só pessoas autorizadas possam usá-lo.</h6>
<h6>Deve haver dois tipos de usuários:</h6>
<ul>
  <li>Atendentes: podem fazer vendas e consultar produtos.</li>
  <li>Administradores: podem cadastrar produtos, ver relatórios e gerenciar estoque.</li>
</ul>
<br>
<h3>2. Requisitos Não-Funcionais</h3>
<br>
<h4>Fácil de Usar</h4>
<ul>
  <li>A interface deve ser simples e intuitiva, para que qualquer pessoa consiga usar sem dificuldades.</li>
  <li>Deve funcionar bem tanto no computador quanto no celular.</li>
</ul>
<br>
<h4>Segurança</h4>
<ul>
  <li>Os dados dos clientes e vendas devem ser protegidos.</li>
  <li>Apenas usuários com login e senha devem ter acesso ao sistema.</li>
  <li>Atendentes e administradores terão permissões diferentes para evitar alterações indevidas.</li>
</ul>
<br>
<h4>Rápido e Eficiente</h4>
<ul>
  <li>O sistema deve responder rápido às buscas e consultas, sem travar.</li>
  <li>As vendas e atualizações de estoque devem acontecer na hora, sem atrasos.</li>
</ul>
<br>
<h4>Acessível para Todos</h4>
<ul>
  <li>O sistema deve funcionar bem em diferentes dispositivos e tamanhos de tela.</li>
  <li>Deve seguir padrões básicos de acessibilidade para que qualquer pessoa possa utilizá-lo.</li>
</ul>
<br>
<h4>Preparado para Crescer</h4>
<ul>
  <li>O sistema deve ser capaz de armazenar mais produtos e clientes conforme a farmácia cresce.</li>
  <li>No futuro, deve permitir novas funções, como vendas online.</li>
</ul>
<br>
<h4>Confiável e Seguro</h4>
<ul>
  <li>O sistema precisa estar disponível sempre que for necessário, sem falhas.</li>
  <li>Deve ter um sistema de backup automático para evitar perda de informações importantes.</li>
</ul>

# Diagrama de Atividades

![diagrama](https://github.com/user-attachments/assets/27685339-917f-47cb-9755-daf5f8543de9)

# Diagrama de Casos de Uso

![Diagrama de caso de uso drawio](https://github.com/user-attachments/assets/c337991a-fbf4-4d14-93f4-13d3d985e3bc)

# Descrição dos Casos de Uso

*&lt;Descrição do comportamento entre os atores/resquisitos&gt;*

# Diagrama de Sequência

*&lt;Diagrama de ordem e interação dos objetos&gt;*

# Diagrama de Classes

*&lt;Diagrama de relacionamento entre classes para os seus atributos e operações&gt;*

# Diagrama de Estados

*&lt;Diagrama para permite modelar o comportamento interno de um determinado objeto, subsistema ou sistema global&gt;*

# Diagrama de Implantação

*&lt;Diagrama para exibir o relacionamento de hardware e software no projeto&gt;*

# Referências

*&lt;Lista de referências&gt;*
