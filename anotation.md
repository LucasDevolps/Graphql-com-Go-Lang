inputs = dados de entrada.

type = modelo ou classes.

mutation = onde adiciona ou muda dados | Qualquer tipo de mudança que faça alteração no modelo existente.

query = comando pra execução do graphql | Todos os tipos de consultas solicitadas.


-------------------------

go run github.com/99designs/gqlgen init - Inicia o projeto
go run github.com/99designs/gqlgen generate - Atualiza o projeto com os dados alterados

-------------------------

Exemplo de chamada.:

query nomeQualquerParaQuery
{
	categories - nome do objeto que quero consultar
    {
        id - parametros que quero receber 
        name - parametros que quero receber 
        description - parametros que quero receber 
    }
}