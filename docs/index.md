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
<p>- Deve ser possível registrar os clientes da farmácia, com informações como:</p>
<p>- - Nome</p>
<p>- - CPF</p>
<p>- - Telefone</p>
<p>- - Histórico de compras</p>
<br>
<h4>Vendas</h4>
<p>- O atendente precisa conseguir pesquisar se o medicamento está disponível no estoque.</p>
<p>- O sistema deve permitir registrar uma venda, vinculando-a ao cliente.</p>
<p>- Assim que a venda for finalizada, o sistema deve gerar um cupom fiscal.</p>
<p>- O estoque precisa ser atualizado automaticamente.</p>
<br>
<h4>Controle de Estoque</h4>
<p>- Sempre que um produto for vendido, o sistema deve diminuir a quantidade disponível.</p>
<p>- Caso o estoque de um produto esteja baixo, o sistema precisa avisar.</p>
<p>- O administrador deve conseguir visualizar os produtos disponíveis e seus status.</p>
<br>
<h4>Relatórios</h4>
<p>- O sistema deve gerar relatórios para ajudar na gestão da farmácia, como:</p>
<p>- - Vendas feitas no dia, na semana e no mês.</p>
<p>- - Lista dos produtos mais vendidos.</p>
<p>- - Clientes que compram com mais frequência.</p>
<br>
<h4>Acesso ao Sistema</h4>
<p>- O sistema deve ter login para garantir que só pessoas autorizadas possam usá-lo.</p>
<p>- Deve haver dois tipos de usuários:</p>
<p>- - Atendentes: podem fazer vendas e consultar produtos.</p>
<p>- - Administradores: podem cadastrar produtos, ver relatórios e gerenciar estoque.</p>
<br>
<h3>2. Requisitos Não-Funcionais</h3>
<br>
<h4>Fácil de Usar</h4>
<p>- A interface deve ser simples e intuitiva, para que qualquer pessoa consiga usar sem dificuldades.</p>
<p>- Deve funcionar bem tanto no computador quanto no celular.</p>
<br>
<h4>Segurança</h4>
<p>- Os dados dos clientes e vendas devem ser protegidos.</p>
<p>- Apenas usuários com login e senha devem ter acesso ao sistema.</p>
<p>- Atendentes e administradores terão permissões diferentes para evitar alterações indevidas.</p>
<br>
<h4>Rápido e Eficiente</h4>
<p>- O sistema deve responder rápido às buscas e consultas, sem travar.</p>
<p>- As vendas e atualizações de estoque devem acontecer na hora, sem atrasos.</p>
<br>
<h4>Acessível para Todos</h4>
<p>- O sistema deve funcionar bem em diferentes dispositivos e tamanhos de tela.</p>
<p>- Deve seguir padrões básicos de acessibilidade para que qualquer pessoa possa utilizá-lo.</p>
<br>
<h4>Preparado para Crescer</h4>
<p>- O sistema deve ser capaz de armazenar mais produtos e clientes conforme a farmácia cresce.</p>
<p>- No futuro, deve permitir novas funções, como vendas online.</p>
<br>
<h4>Confiável e Seguro</h4>
<p>- O sistema precisa estar disponível sempre que for necessário, sem falhas.</p>
<p>- Deve ter um sistema de backup automático para evitar perda de informações importantes.</p>

# Diagrama de Atividades

<mxfile host="app.diagrams.net" agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/134.0.0.0 Safari/537.36" version="26.1.1">
  <diagram name="Página-1" id="EUnatXKg4UHT1Jn5ySwY">
    <mxGraphModel dx="1750" dy="928" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="827" pageHeight="1169" math="0" shadow="0">
      <root>
        <mxCell id="0" />
        <mxCell id="1" parent="0" />
        <mxCell id="OsXEs1ndok8c7S23XYz--21" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;exitX=0.5;exitY=1;exitDx=0;exitDy=0;entryX=0.5;entryY=0;entryDx=0;entryDy=0;" edge="1" parent="1" source="OsXEs1ndok8c7S23XYz--4" target="OsXEs1ndok8c7S23XYz--5">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--4" value="INÍCIO" style="ellipse;whiteSpace=wrap;html=1;fillColor=#d5e8d4;strokeColor=#82b366;" vertex="1" parent="1">
          <mxGeometry x="354" y="10" width="76" height="40" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--24" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;exitX=0.5;exitY=1;exitDx=0;exitDy=0;entryX=0.5;entryY=0;entryDx=0;entryDy=0;" edge="1" parent="1" source="OsXEs1ndok8c7S23XYz--5" target="OsXEs1ndok8c7S23XYz--6">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--5" value="CLIENTE CHEGA Á FARMACIA&amp;nbsp;" style="rounded=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" vertex="1" parent="1">
          <mxGeometry x="287" y="80" width="210" height="40" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--22" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;exitX=0.5;exitY=1;exitDx=0;exitDy=0;entryX=0.5;entryY=0;entryDx=0;entryDy=0;" edge="1" parent="1" source="OsXEs1ndok8c7S23XYz--6" target="OsXEs1ndok8c7S23XYz--7">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--6" value="SOLICITA O MEDICAMENTO&amp;nbsp;" style="rounded=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" vertex="1" parent="1">
          <mxGeometry x="287" y="150" width="210" height="40" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--23" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;exitX=0.5;exitY=1;exitDx=0;exitDy=0;entryX=0.5;entryY=0;entryDx=0;entryDy=0;" edge="1" parent="1" source="OsXEs1ndok8c7S23XYz--7" target="OsXEs1ndok8c7S23XYz--8">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--7" value="ATENDENTE PESQUISA NO SISTEMA&amp;nbsp;" style="rounded=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" vertex="1" parent="1">
          <mxGeometry x="287" y="220" width="210" height="40" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--50" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;exitX=1;exitY=1;exitDx=0;exitDy=0;entryX=0.5;entryY=0;entryDx=0;entryDy=0;" edge="1" parent="1" source="OsXEs1ndok8c7S23XYz--8" target="OsXEs1ndok8c7S23XYz--11">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--51" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;exitX=0;exitY=1;exitDx=0;exitDy=0;entryX=0.5;entryY=0;entryDx=0;entryDy=0;" edge="1" parent="1" source="OsXEs1ndok8c7S23XYz--8" target="OsXEs1ndok8c7S23XYz--12">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--8" value="PRODUTO DISPONIVEL?" style="rhombus;whiteSpace=wrap;html=1;fillColor=#fff2cc;strokeColor=#d6b656;" vertex="1" parent="1">
          <mxGeometry x="250" y="300" width="284" height="60" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--11" value="INFORMA INDISPONIBILIDADE AO CLIENTE&amp;nbsp;" style="rounded=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" vertex="1" parent="1">
          <mxGeometry x="380" y="410" width="256" height="40" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--28" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;exitX=0.5;exitY=1;exitDx=0;exitDy=0;" edge="1" parent="1" source="OsXEs1ndok8c7S23XYz--12" target="OsXEs1ndok8c7S23XYz--15">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--12" value="REGISTRA VENDA ASSOCIADA AO CPF" style="rounded=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" vertex="1" parent="1">
          <mxGeometry x="60" y="410" width="170" height="40" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--29" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;exitX=0.5;exitY=1;exitDx=0;exitDy=0;" edge="1" parent="1" source="OsXEs1ndok8c7S23XYz--15" target="OsXEs1ndok8c7S23XYz--16">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--42" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;exitX=1;exitY=0.5;exitDx=0;exitDy=0;" edge="1" parent="1" source="OsXEs1ndok8c7S23XYz--15" target="OsXEs1ndok8c7S23XYz--43">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="350" y="500.3333333333335" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--15" value="SISTEMA ATUALIZA O ESTOQUE" style="rounded=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" vertex="1" parent="1">
          <mxGeometry x="60" y="490" width="170" height="40" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--30" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;exitX=0.5;exitY=1;exitDx=0;exitDy=0;entryX=0.5;entryY=0;entryDx=0;entryDy=0;" edge="1" parent="1" source="OsXEs1ndok8c7S23XYz--16" target="OsXEs1ndok8c7S23XYz--17">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--16" value="GERA CUPOM FISCAL&amp;nbsp;" style="rounded=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" vertex="1" parent="1">
          <mxGeometry x="60" y="585" width="170" height="40" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--31" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;exitX=0.5;exitY=1;exitDx=0;exitDy=0;" edge="1" parent="1" source="OsXEs1ndok8c7S23XYz--17" target="OsXEs1ndok8c7S23XYz--19">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--17" value="CLIENTE REALIZA PAGAMENTO" style="rounded=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" vertex="1" parent="1">
          <mxGeometry x="60" y="660" width="170" height="40" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--33" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;exitX=1;exitY=1;exitDx=0;exitDy=0;" edge="1" parent="1" source="OsXEs1ndok8c7S23XYz--19" target="OsXEs1ndok8c7S23XYz--20">
          <mxGeometry relative="1" as="geometry">
            <Array as="points">
              <mxPoint x="230" y="790" />
              <mxPoint x="360" y="790" />
            </Array>
          </mxGeometry>
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--19" value="CLIENTE RECEBE PRODUTO&amp;nbsp;" style="rounded=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" vertex="1" parent="1">
          <mxGeometry x="60" y="740" width="170" height="40" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--20" value="FIM" style="ellipse;whiteSpace=wrap;html=1;fillColor=#f8cecc;strokeColor=#b85450;" vertex="1" parent="1">
          <mxGeometry x="300" y="830" width="120" height="50" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--37" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;exitX=0.5;exitY=1;exitDx=0;exitDy=0;entryX=0.5;entryY=0;entryDx=0;entryDy=0;" edge="1" parent="1" source="OsXEs1ndok8c7S23XYz--35" target="OsXEs1ndok8c7S23XYz--36">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--35" value="ADIMINISTRADOR ACESSA O SISTEMA" style="rounded=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" vertex="1" parent="1">
          <mxGeometry x="310" y="650" width="256" height="40" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--38" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;exitX=0.5;exitY=1;exitDx=0;exitDy=0;" edge="1" parent="1" source="OsXEs1ndok8c7S23XYz--36" target="OsXEs1ndok8c7S23XYz--20">
          <mxGeometry relative="1" as="geometry">
            <Array as="points">
              <mxPoint x="438" y="790" />
              <mxPoint x="360" y="790" />
            </Array>
          </mxGeometry>
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--36" value="GERA RELATORIOS DE VENDAS E ESTOQUE&amp;nbsp;" style="rounded=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" vertex="1" parent="1">
          <mxGeometry x="310" y="720" width="256" height="40" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--39" value="SIM" style="text;html=1;align=center;verticalAlign=middle;resizable=0;points=[];autosize=1;strokeColor=none;fillColor=none;" vertex="1" parent="1">
          <mxGeometry x="190" y="350" width="40" height="30" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--40" value="NÃO" style="text;html=1;align=center;verticalAlign=middle;resizable=0;points=[];autosize=1;strokeColor=none;fillColor=none;" vertex="1" parent="1">
          <mxGeometry x="460" y="360" width="50" height="30" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--48" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;exitX=1;exitY=1;exitDx=0;exitDy=0;" edge="1" parent="1" source="OsXEs1ndok8c7S23XYz--43" target="OsXEs1ndok8c7S23XYz--45">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--49" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;exitX=0;exitY=1;exitDx=0;exitDy=0;entryX=0.5;entryY=0;entryDx=0;entryDy=0;" edge="1" parent="1" source="OsXEs1ndok8c7S23XYz--43" target="OsXEs1ndok8c7S23XYz--35">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--43" value="ALERTA ESTOQUE BAIXO?" style="rhombus;whiteSpace=wrap;html=1;fillColor=#fff2cc;strokeColor=#d6b656;" vertex="1" parent="1">
          <mxGeometry x="336" y="480" width="280" height="60" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--45" value="ADIMINISTRADOR ATUALIZA O ESTOQUE" style="rounded=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" vertex="1" parent="1">
          <mxGeometry x="534" y="585" width="256" height="40" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--46" value="SIM" style="text;html=1;align=center;verticalAlign=middle;resizable=0;points=[];autosize=1;strokeColor=none;fillColor=none;" vertex="1" parent="1">
          <mxGeometry x="596" y="540" width="40" height="30" as="geometry" />
        </mxCell>
        <mxCell id="OsXEs1ndok8c7S23XYz--47" value="NÃO" style="text;html=1;align=center;verticalAlign=middle;resizable=0;points=[];autosize=1;strokeColor=none;fillColor=none;" vertex="1" parent="1">
          <mxGeometry x="354" y="555" width="50" height="30" as="geometry" />
        </mxCell>
      </root>
    </mxGraphModel>
  </diagram>
</mxfile>

![diagrama](https://github.com/user-attachments/assets/27685339-917f-47cb-9755-daf5f8543de9)


# Diagrama de Casos de Uso

*&lt;Diagrama para visualizar o comportamento dos atores&gt;*

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
