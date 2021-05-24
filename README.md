# Hackathon Project - API para ativação dos pipelines

> Parte do trabalho final da disciplina **INFRASTRUCTURE AS CODE (IAC) - HACKATHON EXPERIENCE LAB**

<!-- TODO: o que ele faz? breve descrição... -->

## Instruções

Faça um clone do repositório

```
git clone https://github.com/thalexbr/Hackaton-project-api-pipeline-stack
```

> IMPORTANTE: Você vai precisar ter o framework Serverless para executar os comandos a seguir:

1) Ajuste a linha 13 do arquivo serverless.yml para refletir o conjunto de pipelines criados

```
        - "arn:aws:codepipeline:us-east-1:*:hackathon-CD-*"
```

2) Crie a stack serverless (o nome do stage fica à sua escolha, neste exemplo foi usado o nome _shared_)

```
sls deploy --stage shared
```

3) Utilize a URL gerada pela stack para ativar o pipeline desejado

```
curl -X GET https://<URL_DO_STACK>/activate/<NOME_DO_PIPELINE>
```

4) Acompanhe a execução do pipeline pela console do AWS

> Nota: Não esqueça de remover os recursos após os testes

## Meta

INFRASTRUCTURE AS CODE (IAC) - HACKATHON EXPERIENCE LAB

FIAP (<https://www.fiap.com.br/>)

Turma: 6DVP

Team:

```
Thales Gomes - RM337964
Edilson de Almeida - RM337240
Helton Ribeiro - RM337979
Jailson Silva - RM337212 
```

## Contributing

1. Fork it (<https://github.com/thalexbr/Hackaton-project-api-pipeline-stack/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request
