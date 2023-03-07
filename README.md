# *Projeto individual final*

Quando nosso grupo se reuniu para idealizar o projeto e debater as ideias, nossa squad 2, teve a sensibilidade de pensar em um conteúdo
que fosse de interesse comum a comunidade, algo que contribuísse, e a certo nível ajudasse a vida cotidiana de qualquer cidadão brasileiro.
Pensamos em criar um aplicativo que fosse simples, objetivo, com uma estética "limpa" e com usabilidade clara e direta. Para que fosse acessível e de
fácil compreensão a todos, mas principalmente aqueles que não tem tanta proximidade com a tecnologia.

Com isso em mente, surgiram as seguintes ideias:


**Yasmim:** Criar uma Api que organizasse em uma só aplicação os dados do cidadão brasileiro em relação ao SUS! Para ter todas as informações em um só lugar como, por exemplo: os dados sobre vacina e as unidades de coleta de sangue.

**Priscila:** Criar uma API que solucionasse a falta de bibliotecas físicas nos bairros. Criando um aplicativo que contivesse livros gratuitos, com a opção de ler online e baixar em pdf.

**Orlando:** Uma aplicação que agrupa os dados em tempo real do transporte público do Rio de Janeiro. Atualmente o aplicativo Moovit permite que o usuário consulte apenas o tempo real dos ônibus, enquanto a SuperVia possui o seu próprio aplicativo que mostra apenas os dados em tempo real dos trens, e o VLT possui o seu próprio aplicativo que faz o mesmo, e só exibe o tempo real do VLT. Dessa maneira, os usuários necessitam de 3 apps em seu telefone para consultar o tempo do transporte público. O intuito da aplicação seria permitir que em um único site todas essas informações fossem exibidas de forma agrupada.

**Thiago:** Criar uma API para fazer uma integração das bibliotecas públicas. Gerar um único banco de dados para pesquisa e localização de livros.
Teria uma relação de autor e título, onde está localizada a obra ou livro científico, separando por município e bairro do Rio de Janeiro.

**Matheus:** O chat em bloco é uma plataforma/aplicativo que permite o armazenamento de diversos arquivos em pastas separadas semelhante ao github!com a possibilidade de armazenar em uma parte separada: videos, audios e arquivos em textos, por se tratar de um bloco de notas também é possível manter os dados e anotações, todos os arquivos ficam salvos em nosso servidor, tendo a opção de salvar em seu dispositivo!além desta capacidade por ser um chat com bloco de notas, obviamente possui um espaço para conversas, não há necessidade de login, apenas para chats privados e pessoais, as conversas são disponibilizadas através de um link pessoal aonde qualquer pessoa pode ter acesso caso entre este link, obviamente existe a possibilidade de manter este link privado, em cada conversa haverá um repositório guardando os arquivos compartilhados pelo chat,lembrando que o repositorio pessoal é separado dos chats que você entrar

**Gabrielly:** 
Crie uma aplicação que permita e facilite que qualquer pessoa possa registrar informações em um 'bloco de notas' voltado para a área da saúde. Além das notas criadas, a aplicação ainda permite que o usuário crie um perfil com o seu 'nome', 'gênero', 'data de nascimento', 'peso', 'altura' e 'tipo sanguíneo'. Também é inserido no perfil o 'IMC', que é gerado automaticamente com base nos dados inseridos. A ideia é que a aplicação auxilie no registro de consultas agendadas, horário de remédios, controle de medicamentos, cronograma de vacinação, e muito mais! (PROPOSTA ESCOLHIDA)

## *Kanban criado após a reunião do squad*
     
     
|    To Do  |  In Progress  |      Done |
| :------------ |      :---------------:|          -----:|
|Validação dos campos da Login |Validação dos campos da Api|Banco de dados |
|Integração do Back end com o Front end |Escolha da paleta de cores    |Escolha da idéia da aplicação |
|Readme com as instruções e informações do projeto |Teste da Api|Estrutura da Api |
|Slide de apresentação |Estrutura do Front end|Divisão das tarefas do squad|



# Caderno da Saúde
(PROPOSTA ESCOLHIDA)
Nossa API é composta por 4 entidades

## Entidades

- 'usuarios'
- 'notas'
- 'perguntas'
- 'comunicados'


## Entidades

![ENTIDADE_USUARIOS](https://raw.githubusercontent.com/Opseua/M5-GRU_FINAL_Case-2-Site-do-Meu-app/BRANCH_Orlando/src/views/login/ENTIDADE_USUARIOS.png)

![ENTIDADE_NOTAS](https://raw.githubusercontent.com/Opseua/M5-GRU_FINAL_Case-2-Site-do-Meu-app/BRANCH_Orlando/src/views/login/ENTIDADE_NOTAS.png)

![ENTIDADE_PERGUNTAS](https://raw.githubusercontent.com/Opseua/M5-GRU_FINAL_Case-2-Site-do-Meu-app/BRANCH_Orlando/src/views/login/ENTIDADE_PERGUNTAS.png)

![ENTIDADE_COMUNICADOS](https://raw.githubusercontent.com/Opseua/M5-GRU_FINAL_Case-2-Site-do-Meu-app/BRANCH_Orlando/src/views/login/ENTIDADE_COMUNICADOS.png)


## API Rest

GetAll 'usuarios'

```bash
{
    "data": [
        {
            "usuario_id": 1,
            "usuario_nome": "Orlando",
            "usuario_genero": "Masculino",
            "usuario_nascimento": "2001-01-01T02:00:00.000Z",
            "usuario_peso": "75.2",
            "usuario_altura": "1.85",
            "usuario_tipo_sanguineo": "A+",
            "usuario_imc": "25.41",
            "usuario_email": "orlando@gmail.com",
            "usuario_senha": "d0401f7ad4fc4db75a9c9f76bef3f630946a82e8",
            "usuario_reset_pergunta": "Comida favorita?",
            "usuario_reset_resposta": "maça",
            "usuario_extra": "{\"inf_1\":\"Essa é a informação adicional 1\",\"inf_2\":\"Essa é a informação adicional 2\",\"inf_3\":\"Essa é a informação adicional 3\"}",
            "usuario_status": "on"
        },
        {
            "usuario_id": 2,
            "usuario_nome": "Thiago",
            "usuario_genero": "Masculino",
            "usuario_nascimento": "2002-02-02T02:00:00.000Z",
            "usuario_peso": "80.6",
            "usuario_altura": "1.73",
            "usuario_tipo_sanguineo": "O-",
            "usuario_imc": "35.61",
            "usuario_email": "thiago@gmail.com",
            "usuario_senha": "032c63503cc890b0e5918db424076f8d104a95a7",
            "usuario_reset_pergunta": "Cor favorita?",
            "usuario_reset_resposta": "azul",
            "usuario_extra": "{\"inf_1\":\"Essa é a informação adicional 1\",\"inf_2\":\"Essa é a informação adicional 2\",\"inf_3\":\"Essa é a informação adicional 3\"}",
            "usuario_status": "on"
        }
    ]
}
```
    

GetAll 'notas'

```bash
"data": [
        {
            "nota_id": 1,
            "nota_titulo": "Consultas marcadas",
            "nota_informacao": "15/02/2023 consulta no Centro do RJ com o Dr Marcelo, para checar a minha coluna",
            "nota_ultima_edicao": "2001-01-01T14:27:00.000Z",
            "usuario_id": 1
        },
        {
            "nota_id": 2,
            "nota_titulo": "Remédios para tomar",
            "nota_informacao": "Tomar o remédio para diabetes nesses horários 12:00, 22:00, 04:00",
            "nota_ultima_edicao": "2002-02-02T15:12:00.000Z",
            "usuario_id": 1
        }
    ]
}
```
        


GetAll 'perguntas'

```bash
{
    "data": [
        {
            "pergunta_id": 1,
            "pergunta_pergunta": "Qual seu peso?"
        },
        {
            "pergunta_id": 2,
            "pergunta_pergunta": "Qual sua altura?"
        },
        {
            "pergunta_id": 3,
            "pergunta_pergunta": "Qual seu tipo sanguineo?"
        }
    ]
}
```




GetAll 'comunicados'

```bash
{
    "data": [
        {
            "comunicado_id": 1,
            "comunicado_genero": "Feminino",
            "comunicado_informacao": "você sabe fazer o auto exame?",
            "comunicado_feedback": "beleza!é isso aí, mantenha a saúde em dia!",
            "comunicado_link": "https://www.inca.gov.br/noticias/confira-recomendacoes-do-ministerio-da-saude-para-o-rastreamento-do-cancer-de-mama"
        },
        {
            "comunicado_id": 2,
            "comunicado_genero": "Feminino",
            "comunicado_informacao": "Gostaria de fazer mais sobre o câncer de mama",
            "comunicado_feedback": "Tudo bem! quem sabe no futuro!?",
            "comunicado_link": "https://www.gov.br/inca/pt-br/assuntos/gestor-e-profissional-de-saude/controle-do-cancer-de-mama/dados-e-numeros/mamografias-no-sus"
        }
    ]
}
```




