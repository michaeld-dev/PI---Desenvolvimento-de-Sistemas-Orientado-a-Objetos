# PI---Desenvolvimento-de-Sistemas-Orientado-a-Objetos
Projeto Integrador: Desenvolvimento de Sistemas Orientado a Objetos
# SERVIÇO NACIONAL DE APRENDIZAGEM COMERCIAL (SENAC)
## CURSO DE TECNOLOGIA EM ANÁLISE E DESENVOLVIMENTO DE SISTEMAS
### PROJETO INTEGRADOR: DESENVOLVIMENTO DE SISTEMAS ORIENTADO A OBJETOS

**Integrantes do grupo:**
- ABRAAO JOVENTINO CRISPIANO
- ELLEN CAMARGO CATTANEO
- GUSTAVO YUJI DE ALMEIDA FUJIMOTO
- LUIZ FELIPE NEVES DOS SANTOS SIQUEIRA
- MICHAEL DIONE DA SILVA
- PAULO VITOR FERREIRA GONCALVES PIVOTTO
- THIAGO CAPELOZI VIANA DA SILVA
- VITORIA DA CRUZ DIAS

**EAD - ENSINO À DISTÂNCIA - 2024**

## PROJETO INTEGRADOR: DESENVOLVIMENTO DE SISTEMAS ORIENTADO A OBJETOS
**Professor:** Enoque Felipe dos Santos Leal

**TRABALHO PARA APROVAÇÃO EM DISCIPLINA**

**Tema:** PROCESSO DE MODELAGEM DE PROJETO, VOLTADO A GESTÃO DE DADOS DE UM CENTRO UNIVERSITÁRIO UTILIZANDO OS CONHECIMENTOS UML

# Resumo

O trabalho proposto projeta um Diagrama de Caso de Uso para um Sistema de Gestão Escolar, focando no controle, cadastro e administração de usuários em uma universidade. O documento detalha os cenários principais e alternativos para três interfaces principais: acesso ao sistema, cadastro de usuários e área exclusiva para usuários cadastrados. Cada cenário descreve as interações entre os atores envolvidos (incluindo pessoas físicas e jurídicas, professores, alunos e fornecedores, além do sistema), destacando pré-condições, pós-condições e permissões específicas para cada tipo de usuário. Além disso, o trabalho inclui um diagrama de classe que complementa a descrição dos casos de uso, proporcionando uma visão mais abrangente da estrutura do sistema.

**Palavras-chave:** Sistema de Gestão Escolar; Diagrama de Caso de Uso; Controle de Acesso; Interface de Cadastro; Iteração Usuário-Sistema.
# Sumário

1. Diagrama de casos de uso ............................................................... 

2. Descrição de cenários dos casos de uso .......................................... 

3. Diagrama de classe ........................................................................... 

Conclusão .............................................................................................. 


#  Descrição de cenários dos casos de uso do Sistema de Gestão Escolar

## Interface Primária

### Acesso ao Sistema: Usuário

**Atores:** Pessoas físicas e jurídicas, Professores, Alunos e Fornecedores.

1. **Cenário Principal: Interface de Acesso ao Sistema**
   - O Usuário acessa o sistema e na página de acesso terá as seguintes opções: login e senha/cadastrar/ esqueci a senha / sair.
   - O Usuário já cadastrado tenta acessar a área exclusiva e o usuário novo pode se cadastrar.

2. **Cenário Alternativo: Interface de Acesso ao Sistema (Recuperação de login e senha)**
   - O Usuário tenta acessar o sistema e não lembra o login e senha.
   - O Usuário terá a opção de recuperar seu login e senha, seguindo um passo a passo gerado pelo sistema.

3. **Cenário Alternativo: Interface de Acesso ao Sistema (Erro ao acessar seu cadastro ou sair)**
   - O Usuário poderá sair da página clicando na opção, Sair.
   - O Usuário erra 3 vezes o login e senha, o sistema bloqueia seu acesso e gera uma mensagem. (Entre em contato com o administrador do sistema).

## Interface de Cadastro

### Cadastrar: Usuário

**Atores:** Professores, Alunos, Fornecedores e Pessoas físicas e jurídicas.

**Ator:** Administrador do Sistema.

- **Pré-condição:** Para acessar a Área Exclusiva do Sistema o Usuário precisa fazer um cadastro.
- **Pós-condição:** Após fazer o cadastro o Administrador do Sistema terá acesso a esses dados, os quais serão autenticados e armazenados em um banco de dados conforme o tipo de usuário.

1. **Cenário Principal: Interface de cadastro de um novo Usuário**
   - O Usuário ao aceitar a opção de cadastro terá que preencher um formulário com os seus dados pessoais, tipo de interesse na universidade: Professor, Aluno ou fornecedor.

2. **Cenário Alternativo: (Sair do cadastro)**
   - O Usuário poderá sair a qualquer momento do cadastro, sendo que seus dados preenchidos não serão salvos.

## Interface Área Exclusiva para Usuários Cadastrados

### Acesso à área exclusiva: Usuário já Cadastrado e Autenticado

**Ator:** Alunos.

- **Pré-condição:** O Aluno terá que ter feito o cadastro no Sistema e ter recebido um e-mail de confirmação do cadastro pelo Administrador do Sistema.
- **Pós-condição:** Após receber a confirmação, ele terá acesso à área exclusiva dos alunos.

1. **Cenário principal: Acesso à área dos Alunos**
   - O aluno terá acesso a uma interface com alguns tópicos, sendo eles: materiais didáticos, calendário de aulas e avaliações, marcação de avaliações, consulta de notas, acesso à Coordenação do curso, portal financeiro e de requerimentos e outras opções.
   - O aluno terá acesso às disciplinas correspondentes ao seu Curso e Período.

2. **Cenário Alternativo: Permissões**
   - O Aluno não terá permissão para editar conteúdos como excluir ou manipular arquivos. Essas ações são permitidas apenas a usuários com permissão e autenticação de autorização junto ao sistema.

**Ator:** Professores.

- **Pré-condição:** O Professor terá que ter feito o cadastro no Sistema e ter recebido um e-mail de confirmação do cadastro pelo Administrador do Sistema.
- **Pós-condição:** Após receber a confirmação, ele terá acesso à área exclusiva dos professores.

1. **Cenário principal: Acesso à área dos Professores**
   - O professor terá acesso a uma interface com alguns tópicos, sendo eles: materiais didáticos, frequência dos seus alunos, agenda de aulas, outras opções.
   - O professor terá acesso conforme seu cargo e suas disciplinas.

2. **Cenário Alternativo: Permissões**
   - O Professor terá permissão para editar alguns conteúdos, excluir e manipular arquivos, gerando uma autenticação de autorização junto ao sistema.

**Ator:** Fornecedor.

- **Pré-condição:** O Fornecedor terá que ter feito o cadastro no Sistema e ter recebido um e-mail de confirmação do cadastro pelo Administrador do Sistema.
- **Pós-condição:** Após receber a confirmação, ele terá acesso à área exclusiva dos fornecedores.

1. **Cenário principal: Acesso à área dos Fornecedores**
   - O fornecedor terá uma interface com alguns tópicos, sendo eles: licitações em aberto, edital com as condições dos contratos, condições e prazos de validade das licitações, contato do setor responsável pelas negociações.
   - O fornecedor ganhador das licitações terá acesso a um portal especial.

2. **Cenário Alternativo: Permissões**
   - O Fornecedor não terá permissão para editar conteúdos, excluir e manipular arquivos. Essas ações são permitidas apenas a usuários com permissão e autenticação de autorização junto ao sistema.
