# Anotações do Curso - parei no modulo 2

- Jackson-Databind
  - O Jackson Databind é um módulo da biblioteca Jackson que permite a serialização e a desserialização de objetos Java para JSON e vice-versa. No Maven, ele é adicionado como uma dependência para facilitar o mapeamento de dados entre JSON e classes Java de forma automática. 
  - 📌Principais funcionalidades:
    - Conversão de objetos Java para JSON (serialização). 
    - Conversão de JSON para objetos Java (desserialização).
  - O código do Jackson Databind é obtido no MVN Repository
    - Depois inserimos no arquivo "pom.xml" na parte de dependências


### Na classe DadosSerie estamos trazendo informações do arquivo json para o código

- @JsonAlias e @JsonProperty são anotações em Jackson, uma biblioteca Java para processar JSON, 
que ajudam a mapear propriedades de classe para campos JSON.
  - O @JsonAlias é usado para definir um ou mais apelidos para o nome da propriedade JSON associada 
  ao campo Java.
  - O @JsonProperty é usado para definir o nome da propriedade JSON que está associado ao campo Java.
  - O @JsonIgnoreProperties(ignoreUnknown = true) ignora os dados que você não está puxando


### Na interface IConverteDados

- Usamos "< T >" T para dizer que esperamos um tipo genérico
- A classe recebe um json e uma classe e converte op json na classe indicada

### Na classe Dados Temporada

- Utilizamos list < DadosEpisodio > para exibir os dados de todos os episódios usando a classe
DadosEpisodio que pega os detalhes de cada episodio