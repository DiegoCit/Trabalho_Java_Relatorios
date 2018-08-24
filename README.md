# Trabalho_Java_Relatorios
Lista de Exercícios

Crie um programa que mostre o seguinte menu ao usuário:
01 – Cadastrar Profissional.
02 – Criar relatório de profissionais ordenada por Nome
03 – Criar relatório de profissionais ordenado por Data de Nascimento
04 – Criar relatório de profissionais ordenado por Estado.
05 – Criar relatório de profissionais ordenado por salário.
06 – Consolidar relatório de profissionais.
07 – Pesquisar dados.
08 – Excluir Profissional.
09 - Sair
Os dados requisitados para cada profissional serão:
- Nome, data de nascimento, endereço (Rua, Cidade e Estado), profissão e salário.
(As profissões estão limitadas a: Advogado, Dentista e Médico).
O profissional deverá ser cadastrado também na base de dados.
Cada categoria de profissional terá um diretório correspondente (escolha um diretório como raiz) na
seguinte estrutura:
#RAIZ#\Advogado\lista-advogados.xt
#RAIZ#\Médico\lista-médicos.txt
#RAIZ#\Dentista\lista-dentista.txt

Os itens 02 a 05 do menu terão as seguintes opções:
01 – Advogado
02 – Dentista
03 – Médico
O padrão de nomenclatura dos arquivos será:
relatorio-#profissão#-ord[nome|dtNasc|End|Sal]-YYYY-MM-DD.txt
Onde YYYY = Ano, MM = Mês, DD = Dia.
O item 06 deve gerar o seguinte arquivo: #RAIZ#\Consolidado\lista-profissionais-consolidado-V.txt, com as
seguintes informações: Total de advogados, dentistas e médicos e a soma do salário de todos os
profissionais de cada categoria. (V = Versão do relatório 1, 2, 3 etc)
Ex.:
Advogados: 10
Salário Total: 340.000,00
Dentistas: 30
Salário Total: 145.000,00
Médicos: 52
Salário Total: 680.000,00

Programação Orientada a Objetos II
Professor Marcelo Afanaci Junior
Aula 02 - 03
I/O – JDBC

O item 07 deve oferecer ao usuário 5 opções de pesquisas diferentes, quando o usuário optar por uma
delas, os dados devem ser buscados na base e exibidos em tela.
O item 08 deve excluir o profissional desejado da base de dados. Quando o profissional for excluído, o
arquivo com a lista de profissionais deverá ser sobrescrito com os dados agora sendo buscados da base de
dados.
Lembrem-se: A Todo momento em que um novo profissional for cadastrado, caso um novo relatório seja
gerado, ele deve estar atualizado com o último profissional cadastrado e sobrescrever o anterior. O mesmo
é válido para a exclusão de um funcionário.
No momento em que um novo relatório consolidado é gerado ele deve ser automaticamente incluído na
base.